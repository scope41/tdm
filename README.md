# Tasmota Device Manager
GUI application to discover and monitor devices flashed with [Tasmota firmware](https://github.com/arendst/Sonoff-Tasmota)

![image.png](../assets/image.png)

# Features

 - autodetection of devices following the default topic template for Tasmota (%prefix%/%topic%/) and for HomeAssistant Auto Discovery protocol (%topic%/%prefix%/)
 - module and GPIO configuration (see below for more screenshots)
 - rules editor
 - devices with different syntax can be added manually.
 - toggleable active querying of telemetry
 - passive monitoring of state and telemetry (currently supported sensors are listed in "status8.json")
 - clean, readable interface
 - relay control via context menu on device list (all ON/OFF, or individual)
 - clean retained relay topic messages.
 - MQTT console with payload preview (dbl-click an entry to display), sorting and filtering.
 - selectable detail columns in device list
 - BSSID aliasing for larger deployments

# Planned functions
  
 - dynamic and manual grouping of devices: by group topic, module, firmware revision, and more
 - group actions: reset/restart/control power/upgrade
 - console commands with topic and syntax completion 
 - easy access to advanced settings and commands from Tastmota
 - quick settings for common use cases
 - code completion in rule editor
 - built-in OTA server
 - customizable order of detail columns in device list
 - and much more! (you're welcome to post feature requests)

# Requirements

Python 3.5+ [recommended 3.6 or 3.7] (if not already installed on your system, read the python3 installation instructions for your platform)

PyQt5: <pre>pip3 install PyQt5</pre>
paho-mqtt: <pre>pip3 install paho-mqtt</pre>

If you don't have pip3 installed for some weird reason, use <pre>python3 -m pip install \<package\></pre>

Uses free icons from [FatCow](https://www.fatcow.com/free-icons)

# Screenshots

![module.png](../assets/module.png)

![rules.png](../assets/rules.png)

![columns.png](../assets/columns.png)
