# KissKONG - Next Generation KISS OSD

This is a written-from-scratch code to communicate with KISS FC and control MAX7456 to disaply OSD GUI

#### Code is currently compatible with MinimOSD hardware and any ATmega328p with MAX7456 on default SPI pins

```KissAndMsp```, ```Tramp``` and ```MAX7456``` are stand-alone libs that can be used in other projects.

To be able to use the menu to change settings, ARM MUST be set to be controlled by a switch!
If setting is not detetcted, only live data and flight statistics will be shown.

### Installing
- Download recent verion of Arduino IDE
- First open ```FontUploadSketch.ino``` in Arduino IDE
- Select board to be "Arduino Pro Mini 5V 16MHz"
- Upload the sketch to MinimOSD to update the font
- Next open ```KissKongOSD.ino``` in Arduino IDE and Upload it as above
- Done

### Controls (Throttle always in center)
* Enter Main Menu -> Yaw Right + Roll Left
* Move Left /Right -> Roll (also Enter/Exit in Menu/Info)
* Move Up/Down ->  Pitch
* Enter/Exit(Add/Substract) -> Yaw

### Menu can be entered ONLY when disarmed

### Tramp VTX Support
Connect Tramp VTX Telemetry wire to the current sensing pin of MicroMinimOSD to control your VTX through the OSD

There are plans to use the built-in Tramp support in Kiss FC when one is not detected on the current pin

![Connections](images/connections.jpg)

## Example Screens

### Armed

![Armed](images/armed.jpg)

### Main Menu

![Menu](images/menu.jpg)

### Settings

![Settings](images/settings.jpg)

### PIDs

![PIDs](images/pids.jpg)

### Rates

![Rates](images/rates.jpg)

### Extra PIDs

![xPIDs](images/xtra.jpg)

### Filters

![Filters](images/filters.jpg)

### Info

![Info](images/info.jpg)

### Flight Statitics

![Stats](images/stats.jpg)

### Tramp VTX

![Stats](images/tramp.jpg)
