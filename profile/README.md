# MADS-NET: Multi-Agent Distributed System

MADS-NET is a simple framework for implementing a network of distributed agents that can exchange information via ZeroMQ.

It is made by a main set of executables available in the [MADS tools collection](https://github.com/pbosetti/MADS) repo, which also provides installers for Linux, MacOS and Windows at <https://git.new/mads>. 

The MADS tools collection includes a broker and a set of general purpose agents that can act as **sources**, **filters**, or **sinks**. The actual operations performed by agents can be customized either via scripting languages (using simple plugin interface), or by implementing dedicated plugins in C++.

The `mads package` command can install pre-compiled binaries of the most common plugins and custom agents, but you can also build and install plugins from source code.

The pre-build bianaries available via `mads package` are:

* `arduino.plugin`: Interfacing with an Arduino via Serial port [repo](https://github.com/MADS-NET/arduino_plugin)
* `arduinoQ.plugin`: Runs on an Arduino Uno Q and directly taps into its MCU [repo](https://github.com/MADS-NET/arduinoQ_plugin)
* `hdf5.plugin`: Dumps data into a HDF5 file [repo](https://github.com/MADS-NET/hdf5_plugin)
* `mads-chat`: Allows to chat with the MADS network [repo](https://github.com/MADS-NET/mads_chat)
* `mads-fmu`: Uses a Functional Mock-up Interface (FMU) as a filter [repo](https://github.com/MADS-NET/FMU_agent)
* `mads-python`: Implements an agent in Python [repo](https://github.com/MADS-NET/python_agent)
* `onnx-agent`: Uses ONNX models as a filter or a source [repo](https://github.com/MADS-NET/onnx_agent)
* `r.plugin`: Implements an agent in R [repo](https://github.com/MADS-NET/r_plugin)
* `rerunner.plugin`: Logs data to the Rerun.io viewer [repo](https://github.com/MADS-NET/rerunner_plugin)
* `tui.plugin`: Terminal User Interface for sending metadata commands to MADS network [repo](https://github.com/MADS-NET/tui_plugin)
* `validator.plugin`: Validates data traffic [repo](https://github.com/MADS-NET/validator_plugin)


Some other available plugins are:

* [hpe2D_plugin](https://github.com/MADS-NET/hpe2d_plugin): performs human pose estimation from a camera stream
* [mqtt_plugin](https://github.com/MADS-NET/mqtt_plugin): acts as a bridge with an MQTT network via two agents: `mqtt2mads.plugin` (source) and `mads2mqtt.plugin` (sink)
* [say_plugin](https://github.com/MADS-NET/say_plugin): Text-to-speech of incoming messages
* [ble_plugin](https://github.com/MADS-NET/ble_plugin): Bluetooth Low Energy source plugin
* [lua_plugin](https://github.com/MADS-NET/lua_plugin): Interfacing Lua scripts to the MADS network (useful for prototyping and rapid development)
* [rpio_plugin](https://github.com/MADS-NET/rpio_plugin): source and sink agents for Raspberry Pi GPIO pins (using `libgpiod` v1.6)
* [agents_status_plugin](https://github.com/MADS-NET/agents_status_plugin): a sink agent that tracks active agents and their status

