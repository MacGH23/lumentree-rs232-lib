# meanwell-can-lib
Tool to control Lumentree inverter 600/1000/2000 with software/PCB from ask4it.de
Should also work with SUN Invertes with Trucki PCB

Tested only with Lumentree 600g2 

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

- All scripts are without any warranty. Use at your own risk
