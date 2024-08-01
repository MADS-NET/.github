# MADS-NET: Multi-Agent Distributed System

MADS-NET is a simple framework for implementing a network of distributed agents that can exchange information via ZeroMQ.

It is made by a main set of executables available in the [MADS tools collection](https://githib.com/MADS-NET/MADS) repo, which also provides installers for Linux, MacOS and Windows. 

The MADS tools collection includes a broker and a set of general purpose agents that can act as **sources**, **filters**, or **sinks**. The actual operations performed by agents can be customized either via scripting languages (using simple popen interface), or by implementing dedicated plugins in C++.

Some of the available plugins are:

* [arduino_plugin](/MADS-NET/arduino_plugin): reads from a serial connected arduino
* [hpe2D_plugin](/MADS-NET/hpe2d_plugin): performs human pose estimation from a camera stream
* [mqtt_plugin](/MADS-NET/mqtt_plugin): acts as a bridge with an MQTT network

