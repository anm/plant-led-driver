![Board front render](https://github.com/anm/plant-led-driver/blob/main/led-driver.png?raw=true)

This was designed for grow light but obviously can be rather more general
purpose. I have made one and it works.

Drivers are PAM2863, controller STM32G030F6P6.

Software incomplete, but may clean up / publish at some point, especially if
there is interest. I didn't do modbus yet but the 485 link works with custom
commands. It could also be persuaded to understand DMX, I believe.

Some idiosyncracities in design becasue of what parts I had. The 5V supply is
just for the MAX485. You could use a MAX3485 or other 3.3V part. The board is
<100x100mm for cheap manufacture, and the components are cheap from LCSC. The
throughhole stuff could be made SMD for cheap manufacture, but I made this for
assembling myself with parts I had.

The electrolytic caps and inrush NTC are not needed.

I designed it for, and tested it up to, 700mA (nominal) per channel. The
drivers can do 2A, and the specified components should also work at 2A, except
that you need to change the current sense resistor to change the maximum
current. Choose resistance according to the table in the datasheet or on the
back of the board, with sufficient power dissapation.
