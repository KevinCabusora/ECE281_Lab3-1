ECE281_Lab3
===========

Elevator Controller Variations

ECE 281, M6 Dr Neebel

Pre-Lab
===========

![Prelab Schematic](https://github.com/KyleJonas/ECE281_Lab3/blob/master/Prelab_Schematic.PNG?raw=true "Image")

[Nexys2_top_shell](https://github.com/KyleJonas/ECE281_Lab3/blob/master/Nexys2_top_shell.vhd)

[Clook_Divider](https://github.com/KyleJonas/ECE281_Lab3/blob/master/Clock_Divider.vhd)

[Nexys2_sseg](https://github.com/KyleJonas/ECE281_Lab3/blob/master/nexys2_sseg.vhd)

[Nibble_to_sseg](https://github.com/KyleJonas/ECE281_Lab3/blob/master/nibble_to_sseg.vhd)

[pinout](https://github.com/KyleJonas/ECE281_CE3/blob/master/MooreElevatorController_Shell.vhd)


Main Lab
===========

Bad Code
===========
I orrigionally did not initialize a value for nibble0 and nibble1. This caused display issues and wouldn't let the code compile correctly. 
```
-- nibble0 <= ;
-- nibble1 <= ;
nibble2 <= "0000";
nibble3 <= "0000";
```

Good Code
===========
By initialize each of the nibbles I was able to assign a variable or a zero to each of the seven segment displays.
```
nibble0 <= floorSignal;
nibble1 <= nextFloor;
nibble2 <= "0000";
nibble3 <= "0000";
```

Demo
===========
Basic
* Moore:
* Mealy:

B Functionality
* More Floors (Prime Numbers):
* Change Inputs (7 Floors):

A Functionality
* Moving Lights: Not Demoed
* Multiple Elevators: Not Demoed


Documentation
===========

I got help from C3C Her to show me where I had an error in the MealyElevatorController_Shell for 7 floors.


