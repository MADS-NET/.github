# MADS-NET: Multi-Agent Distributed System

MADS-NET is a simple framework for implementing a network of distributed agents that can exchange information via ZeroMQ.

It is made by a main set of executables available in the [MADS tools collection](https://github.com/pbosetti/MADS) repo, which also provides installers for Linux, MacOS and Windows. 

The MADS tools collection includes a broker and a set of general purpose agents that can act as **sources**, **filters**, or **sinks**. The actual operations performed by agents can be customized either via scripting languages (using simple popen interface), or by implementing dedicated plugins in C++.

Some of the available plugins are:

* [arduino_plugin](https://github.com/MADS-NET/arduino_plugin): reads from a serial connected arduino
* [hpe2D_plugin](https://github.com/MADS-NET/hpe2d_plugin): performs human pose estimation from a camera stream
* [mqtt_plugin](https://github.com/MADS-NET/mqtt_plugin): acts as a bridge with an MQTT network
* [say_plugin](https://github.com/MADS-NET/say_plugin): Text-to-speech of incoming messages
* [ble_plugin](https://github.com/MADS-NET/ble_plugin): Bluetooth Low Energy source plugin
* [tui_plugin](https://github.com/MADS-NET/tui_plugin): Terminal User Interface for sending metadata commands to MADS network
* [lua_plugin](https://github.com/MADS-NET/lua_plugin): Interfacing Lua scripts to the MADS network (useful for prototyping and rapid development)
* [lua_plugin](https://github.com/MADS-NET/python_plugin): Interfacing Python3 scripts to the MADS network (useful for prototyping and rapid development)

