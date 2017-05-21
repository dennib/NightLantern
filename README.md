# NightLantern 
##### for Rust


>_This plugin was originally created and developed by me, now is currently mantained and developed by k1lly0u of Oxide community. This GitHub version (1.2.0) refers to last version I uploaded, for last, stable, full functioning version (and its documentation) download latest release [here](http://oxidemod.org/downloads/oxide-for-rust.1659/)_

NightLantern is a C# plugin for Rust, it is meant to be run by Oxide framework.
Rust is PC survival game currently in development by Facepunch Studios.

NightLantern handles automatic ignition and shutown of all lanterns placed in the world. 

It turns on lantern after sunset and off after sunrise.

## Installation
### Requirements
Nightlantern is a plugin for Rust modded server, it needs Oxide mod to be executed. First thing you need to do is download and install Oxide.

You can see all Oxide documentation and download link here:
http://oxidemod.org/downloads/oxide-for-rust.1659/

### Installing NightLantern
Simply download and place NightLantern.cs file into Oxide "Plugins" folder and you will be good to go with defaults configuration.

### Configuration
Dropping NightLantern.cs file into plugin folder will generate the relative 
configuration file into "Config" folder, here are default parameters:

```
{
  "SunriseHour": 7.5, 
  "SunsetHour": 18.5,
  isAutoTurnLanternsEnabled = false,
  includeJackOLanterns = false,
  includeCampfires = false
}
```
You can modify:
- edit **_sunset_** and **_sunrise_** hours
- **_disable automatic_** on/off **_cycle_** (server admin can manually manage ignition and shutdown via chat commands)
- choose whether you want to **_include campfires and Jack-o-Lantern_** in automatic cycle

## Usage
By default automatic cycle is enabled so server admin doesn't need to anything. If automatic automatic cycle is disabled (or a manual touch is needed) _chat command **Lant**_ can be used:

### Chat Command Lant
Server admin can type **_/Lant {param}_** where param can take **_on_** or **_off_** values to manually and instantly handle lanterns (and other deployable included in config file)

