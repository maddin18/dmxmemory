The goal is a device with DMX in and DMX out, each isolated. It shall have the following operating modes:

  (1) While there is a valid DMX signal on the input, the signal shall be forwarded straight to the DMX output. This can be done by simply setting passthrough_n LOW, so the NAND logic will pass the signal from the input receiver on to the output transmitter.
  
  (2) A valid DMX signal on the input may be stored to the controllers's non volatile memory if a button is pressed during power-on and a valid DMX signal is present.
  
  (3) While there is no valid DMX signal on the input, the stored DMX data shall be sent to the DMX output. passthrough_n must be set to HIGH in order to forward the controller output to the RS485 transmitter.

Two DC/DC converters and isolated RS485 transceivers are used for galvanic isolation. If no isolation is required, the DC/DC converters can be replaced by wires.

This project is yet work in progress. Schematic and board file have been updated. Next step: Implement firmware, preferably using ArduinoIDE.

**CREDITS**\
This project uses the kicad library for the XIAO ESP32-C6 from https://wiki.seeedstudio.com/Seeeduino-XIAO/#resourses 

