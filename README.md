#OpenCore EFI for Gigabyte Z390 I AORUS PRO WIFI Mini ITX with i9-9900K and iGPU

## Current State

* MacOS Monterey 12.4
* OpenCore 0.8.1
* i9-9900K's UHD 630 iGPU fully working and with hardware acceleration  
* Audio stopped working with Monterey; will fix next
* Bluetooth fully working
* Power management fully working (though not yet [fine-tuned with CPUFriend](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/pm.html#using-cpu-friend))
* All USB ports working and powered (unused port modes disabled to stay under the MacOS limit)
  * Most ports have USB 2.0 disabled

## Motherboard settings

* Todo

## Notes

* Had a lot of trouble getting around memory allocation issues at boot, but it's fine now
* Removed AWAC
* Replaced EC-USBX with EC from SSDTTime
* Added HPET and patches
* Replaced PLUG
* Had to set `SecureBootMode` to `Disabled` for Monterey installation

## References

* [OpenCore desktop guide](https://dortania.github.io/OpenCore-Desktop-Guide/)
* [Very clear USB map](https://www.tonymacx86.com/threads/success-pynty-mac-i7-8700-z390-i-aorus-pro-wifi-16gb-ram-sapphire-rx-580-mojave-10-14-3.271145/)
* [OpenCore config sanity checker](https://opencore.slowgeek.com)
