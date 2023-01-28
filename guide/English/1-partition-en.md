This step is required so that we make partitions where our Windows installation will be

## Notes:
> **Warning** if you delete any partitions via diskpart later on or now windows will send a ufs command that gets misinterpreted which erase all your ufs
- All your data will be erased! Backup now if needed.
- These commands have been tested.
- Ignore `udevadm` warnings
- Do not run the same command twice
- DO NOT REBOOT YOUR PHONE if you think you made a mistake, ask for help in the [Telegram chat](https://t.me/winonvayu)

#### Boot TWRP recovery through the PC with the command
```cmd
fastboot boot <twrp.img>
```
> If you already have TWRP installed, just hold the power and vol+ buttons at startup

#### Unmount all partitions
Go to TWRP settings and unmount all partitions

## Start the ADB shell
```cmd
adb shell
```

### Start parted
```sh
parted /dev/block/sda
```


### Delete the `userdata` partition
> You can make sure that 18 is the userdata partition number by running
>  `print all`
```sh
rm 18
```

### Create partitions
> If you get any warning message telling you to ignore or cancel, just type i and enter

#### For 64Gb models:

- Create the ESP partition (stores Windows bootloader data and EFI files)
```sh
mkpart esp fat32 11GB 11.4GB
```

- Create the main partition where Windows will be installed to
```sh
mkpart win ntfs 11.4GB 42.4GB
```

- Create Android's data partition
```sh
mkpart userdata ext4 42.4GB 59.4GB
```


#### For 128Gb models:

- Create the ESP partition (stores Windows bootloader data and EFI files)
```sh
mkpart esp fat32 11GB 11.4GB
```

- Create the main partition where Windows will be installed to
```sh
mkpart win ntfs 11.4GB 71.4GB
```

- Create Android's data partition
```sh
mkpart userdata ext4 71.4GB 123GB
```


### Make ESP partiton bootable so the EFI image can detect it
```sh
set 18 esp on
```

### Quit parted
```sh
quit
```

### Reboot to TWRP

### Start the shell again on your PC
```cmd
adb shell
```

### Format partitions
-  Format the ESP partiton as FAT32
```sh
mkfs.fat -F32 -s1 /dev/block/by-name/esp -n ESPVAYU
```

-  Format the Windows partition as NTFS
```sh
mkfs.ntfs -f /dev/block/by-name/win -L WINVAYU
```

- Format data
Go to Wipe menu and press Format Data, 
then type `yes`.

### Check if Android still starts
just restart the phone, and see if Android still works


## [Next step: Install Windows](/guide/English/2-install-en.md)
