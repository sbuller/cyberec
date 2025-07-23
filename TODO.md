Control signals. Can I just wire up the SMB and I2C lines, and send off to a
remote uC? Do I need the interrupt line? Probably... What other lines are
needed? Can I put the uC on the board? It's a little tight, and I'd like to
get this thing shipped already. Still. LDL40 and STM32L431. Then I need to
connect all relevant IO to this board. The backside is available, and I would
like to go to 4-layer for the stackup. Have to reduce size to 50x50 for 4 layer.
Well, it's not mandatory, but desired.

Still need and EC for this EC project.

EC needs to power the RPi. 5.2V, ~2.5A. Probably want an enable/disable.
De-powering the converter probably saves power.
Cutting off the device also probably necessary. Also power sequencing.

Router is powered by USB-C. Probably 5V. 5.2V will probably be fine also.
Needs at least a transistor for power sequencing. 3A.

Switch is 5V. Still want a separate transistor for power sequencing. 0.6A.


Peripherals.
Software Radio. Switchable Power
USB Power
Thermistors
Multimeter
Osciloscope



router is gl.inet mt3000. Has 3.3v uart header. Unpopulated. Has 4pin unlabeled
header J2, with JST style shroud. 5 chips under cans. Mediatek near antennas.
Xilinx? near ethernet. Unknown running 4 pairs to 1G_LAN. 1 DRAM cell next to
PHY?
Details at https://openwrt.org/toh/gl.inet/gl-mt3000?s[]=gl&s[]=inet&s[]=mt3000
https://wikidevi.wi-cat.ru/GL.iNet_GL-MT3000_(Beryl_AX)


switch TL-SG105
https://archive.goughlui.com/wp-content/uploads/2022/02/2022022417550763.jpg
https://datasheet.lcsc.com/lcsc/2103121437_Realtek-Semicon-RTL8367S-CG_C2760849.pdf
