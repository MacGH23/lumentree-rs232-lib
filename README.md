# Lumentree / Trucki RS-485 Lib for python
Tool to control Lumentree inverter 600/1000/2000 with software/PCB from ask4it.de
Should also work with SUN Invertes with Trucki PCB RS-485

Tested only with Lumentree device

Lumentree are controlled via RS232 modbus. <br> 
The connector is a D-SUB9 but only uses <br>
PIN2: RX<br>
PIN3: TX<br>
PIN5: GND<br>
PIN9: 12V <br>
This PIN9 with 12V is not RS232 spec conform and can cause communication problems or a defect of RS232 device. <br>
Use only PIN2,3 and GND if possible.<br>
If you use e.g. a USB RS232 adapter remove PIN9 if you have problems<br>

Please note:  
This python lib and tool controls read and write settings to Lumentree devices via RS232 using minimalmodbus
It is not yet complete and also not fully tested. 
Do not use without monitoring the device. 
There is no error handling yet !!!
Use at your own risk !

lt232cmd.py sample application

	   Usage: ./lt232cmd.py parameter value
       To use a standalone cmd to the mw device
	   
       setwatt              -- set WATT outout
       vread                -- read DC voltage
       acvread              -- read AC voltage
       tempread             -- read internal temperature 
       readwatt             -- read WATT outout

- All scripts are without any warranty. Use at your own risk
