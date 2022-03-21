# Modbus-utils-RPC

A command-line tool used for RPC requests to [wb-mqtt-serial](https://github.com/wirenboard/wb-mqtt-serial).

Some use cases:
 - Read coils ***-a 22 -r 10 -c 4 -f 0x01 tcp 4000 127.0.0.1***
 - Read discrete inputs ***-a 22 -r 10 -c 4 -f 0x02 rtu /dev/ttyRS485-1***
 - Write coil ***-a 22 -r 10 -f 0x05 -w "01" tcp 4000 127.0.0.1***
 - write multiple registers ***-a 22 -r 10 -f 0x10 -w "01AB 01D 01DD" rtu /dev/ttyRS485-2***

## External dependencies
 - [mqttrpc](https://github.com/wirenboard/mqtt-rpc) v 1.1.2 
 - [uModbus](https://github.com/wirenboard/uModbus)
 - paho-mqtt v 1.4.0
