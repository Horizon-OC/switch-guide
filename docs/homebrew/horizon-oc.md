## Horizon OC

Horizon OC is a [sysmodule](index#terminologies) that allows you to overclock the hardware of your Switch. The usage, configuration and clock speed information can be found on the official Github repository [here](https://github.com/Horizon-OC/Horizon-OC)

## Installation requirements:
- An archive manager like [7-Zip](https://www.7-zip.org/)
- The latest release of [Horizon OC](https://github.com/Horizon-OC/Horizon-OC/releases) (the `dist.zip` file)

## Installation instructions:
1. Boot into hekate and go to `Tools` > `USB Tools` > `SD Card`, then plug your Switch into your PC via USB.
1. Your microSD card should now be accessible on your PC, open it.
1. Extract the `.zip` file to a location on your computer.
    - If your archive manager allows for it, you can also simply open the `.zip` file directly.
1. Copy the *contents* of the (extracted) `.zip` file to the root of your microSD card.
1. Edit `hekate_ipl.ini` to include these lines under your boot entries:

   ```
   kip1=atmosphere/kips/hoc.kip
   ```

1. Boot into CFW.
1. Follow the [Erista guide](rentry.co/erista) or [Mariko guide](rentry.co/mariko)

## Basic usage instructions
Open Ultrahand and select Horizon OC Zeus, and configure your settings according to the guide

## Troubleshooting
### My Switch crashes on boot after I installed horizon-oc!:

**Cause:** If your Switch crashes on boot, make sure you're using the latest release of horizon-oc. If it continues to crash afterwards, see the troubleshooting step at the bottom of this page.

## My Switch crashes while using Horizon-OC!:
**Cause:** Your overclock settings may be unstable.
## Horizon-OC isn't working!:

Assuming you've followed the installation instructions successfully, this is probably due to the archive bit being set on one or more folders/files on your microSD card. This is usually the result of copying files to a microSD card via a Mac. If you are experiencing this issue, try running the archive bit fixer utility via hekate for all files.

This can be done by booting into hekate and going to `Tools` > `Arch bit • RCM Touch • Pkg1/2` > `Fix Archive Bit`.
