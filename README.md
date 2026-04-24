<img width="100" height="100" alt="repad_logo" src="https://github.com/user-attachments/assets/58f76651-cff3-4eea-8064-01fd6ef86486" />
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
<svg width="100%" height="100%" viewBox="0 0 1000 1000" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">
    <g transform="matrix(1.323706,0,0,1.323706,-186.401918,-115.643811)">
        <path d="M216.364,491.155L216.364,162.909L820.727,162.909L820.727,480.266C820.495,480.264 820.262,480.263 820.028,480.263C803.442,480.263 790.66,484.787 781.684,493.833C772.709,502.88 768.221,515.843 768.221,532.723C768.221,549.574 772.716,562.556 781.706,571.669C790.7,580.777 803.475,585.331 820.028,585.331C820.262,585.331 820.495,585.33 820.727,585.328L820.727,660.669C820.495,660.667 820.262,660.666 820.028,660.666C803.442,660.666 790.66,665.189 781.684,674.236C772.709,683.282 768.221,696.245 768.221,713.125C768.221,729.976 772.716,742.958 781.706,752.071C790.7,761.179 803.475,765.733 820.028,765.733C820.262,765.733 820.495,765.732 820.727,765.73L820.727,767.273L622.691,767.273C633.356,765.461 643.39,762.469 652.792,758.297C669.417,750.921 683.558,740.227 695.216,726.213C706.878,712.2 715.438,695.337 720.896,675.624L658.578,675.624C651.51,687.645 642.966,696.786 632.947,703.047C622.933,709.308 611.346,712.438 598.187,712.438C576.128,712.438 559.621,704.683 548.667,689.172C540.712,677.904 535.647,662.865 533.471,644.058L712.879,644.058C713.328,640.394 713.689,636.567 713.963,632.577C714.237,628.583 714.373,624.383 714.373,619.978C714.373,589.637 709.687,563.8 700.315,542.468C690.943,521.131 677.46,504.842 659.867,493.599C642.275,482.353 621.113,476.729 596.381,476.729C570.681,476.729 548.301,482.631 529.24,494.435C510.184,506.234 495.414,522.904 484.932,544.444C474.451,565.984 469.21,591.575 469.21,621.217C469.21,652.427 474.299,679.068 484.479,701.142C494.664,723.215 509.298,740.104 528.383,751.809C540.89,759.475 555.023,764.63 570.782,767.273L406.885,767.273L406.885,708.648L326.252,708.648L326.252,618.135C326.252,593.753 329.45,575.613 335.848,563.714C342.246,551.816 352.088,545.867 365.375,545.867C386.287,545.867 396.743,559.465 396.743,586.661L396.743,620.749L463.388,620.749L463.388,577.943C463.388,547.333 457.526,523.909 445.802,507.671C434.079,491.434 417.227,483.315 395.248,483.315C382.651,483.315 371.442,486.037 361.621,491.481C351.8,496.925 344.269,504.64 339.028,514.626L323.227,514.626L323.227,491.155L216.364,491.155ZM216.364,708.648L216.364,550.031L262.737,550.031L262.737,708.648L216.364,708.648ZM534.277,594.361C536.792,579.174 541.638,566.603 548.816,556.647C559.864,541.316 575.719,533.65 596.381,533.65C616.155,533.65 631.052,540.95 641.071,555.549C647.796,565.341 652.266,578.279 654.479,594.361L534.277,594.361Z" style="fill:rgb(255,255,255);"/>
    </g>
</svg>

# rePad Hardware Design
A 3-key Custom Hall Effect Keypad for osu! utilizing an RP2040-Zero base. Hardware Design Repo.
### _[Firmware Repo (pending)]() | [Configurator Repo (pending)]()_


<img width="400" height="300" alt="Image of the keypad" src="https://github.com/user-attachments/assets/d54a0e71-e90b-4e8e-addc-af48be1077a1" />

## Case Design
Designed to be as sleek as possible, as the previous version was found to be bulky both during gameplay and in general both by myself and others who've tested it. 
Since this version is a huge overhaul, I decided to go with a custom PCB reducing the Z-height by a lot, comparable to the [Wooting UwU](https://wooting.io/uwu) even, at just about 3cm keycap-to-base.

<img width="300" alt="Side Profile + Branding" src="https://github.com/user-attachments/assets/256d6f22-768b-4f60-9b53-66e5466f86b2" />

It's a two-part design (three if including the board itself), involving a base (top of which the PCB sits) and a top plate/case into which the switches click into.

<img width="200" src="https://github.com/user-attachments/assets/686c72b0-b414-47f0-9b19-045b31e83356" />
<img width="200" src="https://github.com/user-attachments/assets/f0e754a9-4082-4273-a06e-6fa7905a2057" />
<img width="200" src="https://github.com/user-attachments/assets/828da911-a484-4f1d-b521-cf16eb4a1a97" />


## PCB/Controller Design
Designed in KiCad. First time trying out PCB design.
The custom PCB is designed with an RP2040-Zero in mind, with a footprint (credit: [CountParadox's KiCad Footprint](https://github.com/CountParadox/RP2040-Zero-Kicad)) that allows for an RP2040-Zero board to cleanly slot into. 

This saves a lot of effort and time with raw MCU interfacing being handled already, leaving the only soldering required to be simple THT components. SMD hall sensors would of course be ideal for such an implementation but unfortunately none as available as the TO-92 THT variant, so the slot cutouts are for the sensor legs to bend backwards and be flush with the board surface.

Similarly, the WS2812 RGB LEDs (one included on the RP2040-Zero package itself) had to be the THT variants due to component availability constraints. (though in this case it's a good thing since SMD LEDs seem like a pain to solder)

<img width="200" alt="image" src="https://github.com/user-attachments/assets/90391b73-42da-422a-9343-b1e06d6cca19" />
