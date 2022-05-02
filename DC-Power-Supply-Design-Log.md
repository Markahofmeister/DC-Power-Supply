# Parts ordering

- Voltage regulator is NOT LM317 which I expected to be using. be on the lookout for strange behaviors.
- I decided on a 10k potentiometer for the adjustable voltage divider even though other schematics had 5k. I 
don't know how much a current decrease will affect the regulator - if it even is current driven. In my view, 
higher resistance is safer when I'm not familar with the regulator
- I made great effor to get a TO-220 (Transistor Outline) packaged regulator so I could bolt it to a heatsink. Also,
it made heatsink selection far easier due to standardized packaging. I'm slightly concerned about heat dissipation if
I'm outputting 1.5A at 30V, as I only have a 5V fan and a relatively small heatsink. This is something to watch closely.
- I'll have to check the true Buck converter output, especially if there is some ripple in the input voltage (there will be,
it's only after the big smoothing capacitor, not the small one.) 
- I selected a 230VAC/5A fuse. I'm not quite sure what's ideal. The circuit won't experience voltages nearly that high,
and I assume the same for the current since the regulator is capped at 1.5A and the Buck converter will likely pull little.
My concern is this: is the current rating too high? I can't find a max. current on the regulator's datasheet. 
I don't want to be pulling 4A (somehow) and demolish the regulator, so I may switch to 3A based on testing. 