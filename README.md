![Board front render](https://github.com/anm/plant-led-driver/blob/main/led-driver.png?raw=true)

This was designed for grow light but obviously can be rather more general
purpose.

I have made one and it works.

Software incomplete, but may clean up / publish at some point, especially if
there is interest. I didn't do modbus yet but the 485 link works with custom
commands. It could also be persuaded to understand DMX, I believe.

Some idiosyncracities in design becasue of what parts I had. The 5V supply is
just for the MAX485. You could use a MAX3485 or other 3.3V part.

The electrolytic caps and inrush NTC are not needed.

I only tested it up to 700mA (nominal) per channel.