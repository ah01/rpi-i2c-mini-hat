# Log of project 

## 0. Idea

I would like to try Autodesk Eagle and Fusion 360 integration for electrical and 3d mechanical design. 

## 1. Requirements

- Add connector for external sensors to my Raspberry Pi
- Must fit into my existing box (**[EM-RasPI B+](https://www.emko.cz/produkty/it-skrine/raspberry-pi/em-raspi-b-silver-h3564)**)
- Expose on connector:
	- 1-Wire
	- I2C
	- 5V and 3.3V power supply for sensor
	- Some GPIO if there are unused pins
- Basic ESD protection

## 2. Components

For 1-Wire interface there is DS2482-100 (1-Wire to I2C bridge), this is more reliable then emulated 1-Wire interface form SW.

Each pin is protected by SP0504S TVS Diode Array.

Main connector was selected from 3M mainly because the have STEP file for it... 

- [BOM](doc/rpi-i2c-bom.csv)

## 3. Schematics

Schematics was design in Autodesk Eagle.

[![Eagle - schematics](doc/screens/01-eagle-sch.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/01-eagle-sch.png)

<center><em>Eagle - schematics</em></center>

- [Schematics (PDF)](https://github.com/ah01/rpi-i2c-mini-hat/raw/master/doc/rpi-i2c-sch.pdf)

## 4. PCB Layout

Schematics was design in Autodesk Eagle.

[![](doc/screens/02-eagle-brd1.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/02-eagle-brd1.png)

<center><em>Eagle - PCB Layout</em></center>

[![](doc/screens/03-eagle-brd2.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/03-eagle-brd2.png)

<center><em>Eagle - PCB preview</em></center>

- [Top](https://github.com/ah01/rpi-i2c-mini-hat/blob/master/doc/rpi-i2c-pcb-top.png)
- [Bottom](https://github.com/ah01/rpi-i2c-mini-hat/blob/master/doc/rpi-i2c-pcb-bottom.png)
- Gerber files are in download section

PCB was order from [AllPCB](https://allpcb.com/) (and delivered in 4 days for 10$ - incredible).

![](doc/photo/pcb.jpg)

## 5. 3D Design

PCB for exported (via Fusion 360 integration in Eagle) to Fusion 360. And then whole box and RPI was build around PCB. RPI model come from [here](https://www.thingiverse.com/thing:2572698).


[![](doc/screens/03-fusion.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/03-fusion.png)

<center><em>Fusion 360 - Home view</em></center>

[![](doc/screens/04-fusion.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/04-fusion.png)

<center><em>Fusion 360 - PCB Detail</em></center>

[![](doc/screens/05-fusion.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/05-fusion.png)

<center><em>Fusion 360 - Just PCB</em></center>

[![](doc/screens/06-fusion.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/screens/06-fusion.png)

<center><em>Fusion 360 - Side panel of box</em></center>

## 6. 3D Print of side panel

Side panel of box need to be replaced by new one with hole for connector.

[![](doc/3d/panel.png)](https://raw.githubusercontent.com/ah01/rpi-i2c-mini-hat/master/doc/3d/panel.png)

- [STL File](panel/panel.stl)

## 7. Final assembly

### Visualization

![](doc/3d/all.png)

![](doc/3d/rpi-hat.png)

![](doc/3d/hat.png)

### Rality

![](doc/rpi.jpg)

### Photos

![](doc/photo/02.jpg)

![](doc/photo/03.jpg)

![](doc/photo/04.jpg)

![](doc/photo/05.jpg)
