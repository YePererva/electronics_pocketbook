# Drill motor controllers for DIY PCB



## Existing project(s)


### Based on LM2596

Project from channel [Шоу Бородатого Инженера](https://www.youtube.com/watch?v=y-J96j0w_TE). However, the demonstrated in video schematics has error: the LED should be pointing the opposite direction.

![[pwm.png]]

If replicating, consider:
- replace the LDO LM317 with some impulse DC-DC with something alike PT4115
- use 3 inlet screw-terminal (the original author uses transformer, it would be possible to find transformer with middle-point that can be connected to the schematics GND)

Another approach would be as here:

![](images/other/Регулятор%20оборотов%20двигателя%20на%20LM2596T.jpg)
### Based on MC34063

Details are demonstrated [here](https://www.customelectronics.ru/regulyator-oborotov-minidreli/) with demonstration of work on [YouTube](https://www.youtube.com/watch?v=JnkqLATMvT0) 

The web-site shows the following schematics, but part-list implies having one more Schottky diode.
![[Pasted image 20250415105731.png]]
Perhaps, it is used as reverse-polarity protection after the power inlet terminal.

In case of replication, these could be useful upgrades:
- drop the LDO and use some PD boards for stable 12V power input
- use additional switch for manual ON/OFF
	- when incorporated in the actual drill-press it will let motor start only when the drill bit will start  going down
- make outer diameter according to used motor and consider having center hole for motor shaft and mounting holes

## Typical sizes of motors

### 555 motor dimensions
![[Pasted image 20250415105342.png]]

## 755 motor dimensions

![[Pasted image 20250415105404.png]]