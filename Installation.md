# Installation of xdrip+ on Android

Installing xdrip+ is unfortunally more complicated than usual packages. xdrip+ is for several reasons not in Playstore.
If using the G7, we also need to use the latest nightly builds available.

# 1. Install xdrip+ on Android

Before installing xdrip+, make shure the Dexcom app is uninstalled.
Both apps on one phone does not work.

Download the latest nightly build from here onto your Android smart phone:

https://github.com/NightscoutFoundation/xDrip/releases

Go to Downloads folder and install manually from there.
Usually Android will ask you, if you reeeaaaally want and you're shure about the risks. In this case, we want..


# 2. Configure xdrip+ for G7

xdrip+ can be configured using an QR code.
The QR below is a copy from

https://navid200.github.io/xDrip/docs/Dexcom/G7.html.

It serves just as a backup here, so pls visit to this page and check for latest version of the QR code.

![alt text](doc/G7_keks_QR.png)

In xdrip+, go to Settings −> Auto configure to scan the QR code.

You will see a few warnings, if you really want to accept these settings. Pls accept as described there.

As you're now on this webpage, make shure to read it's informations and make shure to bookmark it.
At some point, you may want to re-check later.

Make shure to check your glucose units, mmol/l or mg/dl.

# 3. Setup permissions

xdrip+ needs some permissions to work.
* permission to enable/disable Bluetooth -> xdrip+ needs to communicate every 5 minutes.
* location/GPS -> needed to locate bluetooth devices (G7 is one) every 5 minutes
Set to always, see https://navid200.github.io/xDrip/docs/Location.html
* auto start -> in case the app was closed
* notifications (Android Settings −> Apps & notifications −> Notifications −> xDrip+)
* time and date needs to be updated automatically (-> Settings −> System −> Date & Time -> Automatic date & time)

xdrip+ should never go to sleep, otherwise it cannot alarm you.
* disable any power saving for xDrip+.
* disable any power saving on bluetooth, see https://navid200.github.io/xDrip/docs/BluetoothBatteryOpt.html
