# Running Windows on the Redmi Note 9 Pro

<img align="center" src="https://github.com/Rubanoxd/Port-Windows-11-redmi-note-9_pro/blob/main/miatoll.png" alt="Windows 11 Running On A Poco X3 Pro">

## ⚠️ **Warning**

We're not responsible for bricked devices, missing recovery partitions, dead xiaomi factoryline ~workers~ cowboys, dead microSD cards, dead pmics, dead ram, dead display ics, dead cpus, any xiaomi/poco shenanigans, dead cats or dogs, nuclear wars or you getting fired because you forgot to boot back in to android for the alarm.

This project is in an early stage, all the files here have been contributed by other users, here you will find a guide with the working files we managed to get. This is a delicate process, do it under your own risk and follow all the steps carefully.

**IF YOU AREN'T COMFORTABLE MODDING YOUR PHONE OR ITS PARTITION TABLE OR YOU ARE PARANOID OF BRICKING YOUR DEVICE CLICK AWAY NOW!!! YOU HAVE BEEN WARNED, YOU ARE ON YOUR OWN IF YOU BRICK YOUR DEVICE!!! AGAIN! YOU HAVE BEEN WARNED!!!**

## Project status

Alpha, windows boot but usb without usb

#### Features

- [ ] Audio 
- [ ] Battery status
- [ ] Bluetooth
- [ ] Brightness
- [ ] Camera
- [ ] Charging 
- [x] Display
- [ ] FM
- [ ] GPU
- [ ] LTE 
- [ ] SD 
- [ ] Touchscreen
- [x] UFS
- [ ] USB 
- [ ] Wi-Fi

#### Sensors
- [ ] Accelerometer
- [ ] Fingerprint
- [ ] GPS
- [ ] Gyroscope
- [ ] Light sensor
- [ ] Magnetometer
- [ ] Proximity


## Guides and requirements

<details> 
<summary><strong>Required Tools/Files</strong></summary>

Human:

- Understand English, Spanish or Russian 

- Understand how to use TWRP

- Understand how to use CMD

- Functioning brain

PC:

- [Windows on ARM image](https://uupdump.net/) (Windows 11 is recommended)

- [platform-tools](https://developer.android.com/studio/releases/platform-tools).

- [DriverUpdater](https://github.com/WOA-Project/DriverUpdater/releases/) to install the [drivers](https://github.com/Icesito68/7xx-Drivers)

Phone:
- [UEFI image](soon)

- [TWRP](https://forum.xda-developers.com/t/recovery-3-4-0-14-miatoll-twrp-xiaomi-redmi-note-9s-9-pro-9-pro-max-poco-m2-pro.4125487/)

</details> 

### Windows installation instructions

<details> 

<summary><strong>English</strong></summary>

1 - [Create partitions](guide/English/1-partition-en.md)

2 - [Install Windows](guide/English/2-install-en.md)
  
</details> 
  
<details> 

<summary><strong>Español</strong></summary>

1 - [Crear particiones](guide/Español/1-particiones-es.md)

2 - [Instalar Windows](guide/Español/2-instalacion-es.md)
  
</details> 

### Other guides:

<details> 

<summary><strong>English</strong></summary>

- [If you just want to update the drivers follow these commands](guide/English/update-en.md)
  
</details> 

<details> 

<summary><strong>Español</strong></summary>

- [Si solo quieres actualizar los drivers sigue estos comandos](guide/Español/Actualizar-es.md)
  
</details> 


## Contributors

<details> 

<summary><b><strong>Credits</strong></b></summary>

- [Morc](Https://GitHub.com/themorc) ```Made the vayu images```

- [Icesito68](https://github.com/Icesito68) ```Made Windows partitioning commands and made this repo```

- [Map220v](https://github.com/map220v) ```Provided help and vayu UEFI uses nabu UFS patches and ACPI and also ported mi pad 5 drivers```

- [Degdag](https://github.com/degdag) ```Improves UEFI and ported drivers```

- [halal-beef](https://github.com/halal-beef) ```Built EDK2 and modified it enough to boot Windows, also ported drivers```
  
- [Renegade Project](https://github.com/edk2-porting) ```Making the core of this project```

- [gus33000](https://github.com/gus33000) ```Providing help, also made base install guide, all of the original drivers and the msc script```

- [Renegade Project Discord members](https://discord.gg/XXBWfag) ```Provided Help```
 
- [ArturoGC06](https://github.com/ArturoGC06) ```Helped in the beginning of the project to the translations and gave Windows data```

- [SebastianZSXS](https://github.com/SebastianZSXS) ```Helped to patch Windows PE```

- [MollySophia](https://github.com/MollySophia) ```Helped to fix battery status```

- [haouarihk](https://github.com/haouarihk) ```Great suggestions on the command notes, also made the new guide```

- [bibarub](https://github.com/bibarub) ```Guide improvenents```

- [wormstest](https://github.com/wormstest) ```Russian and Ukrainian translation``` 

- [proganime1200](https://github.com/proganime1200) ```Tremendously helped to make this possible, heavily contirbuted to the old guide by finding bk01-04 partitions and had managed to nearly get winpe booting in the early stages```

</details>  

