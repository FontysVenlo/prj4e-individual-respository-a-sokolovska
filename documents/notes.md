## Components
Table of content:

- [Motors](#motors)
- [Motor Drivers](#motor-drivers)
- [Microcontrollers](#microcontrollers)
- [Power Supply](#power-supply)
- [Sensors](#sensors)

<br>

---

<br>

### Motors:
As of now, main options for the motors are brushed DC motors with H-bridge or BLCD with gearboxes, as we need continious rotation at high torque, relative ease of control and relatively cheap price. <br>
As to more detailed specifications, I would consider options with voltage starting from **12V**, as 5V introduce quite significant power limitations (less voltage requires more current, hence specialized high-current motor drivers). <br> Considering targeted water enviroment, RPM range should start at slow speeds to push water efficiently, but at the same higher boundary should be quite big to ensure options of manouvering. This brings us to approximate of **50-150 RPM**. In case of high-speed motors we would also need to consider gear reduction ratios. <br>
To figure out torque requirements, we need to know wheels specifications (paddle bades, radius), but safe minimum point would be around **1 Nm**.

| Feature | Suggestion |
|------|------------|
| Voltage | 12V and higher |
| RPM | 50 - 150 rpm |
| Torque | 1Nm and higher |
| Power | 30W or 50W |
| Current Draw | 5A - 10A |


**Option**: [RS PRO Brushed Geared DC Geared Motor - €39.40 RS](https://nl.rs-online.com/web/p/dc-motors/2389670) <br>
19.8 W, 12 V dc, 59 Ncm, 84 rpm, 6mm Shaft Diameter <br> (a bit weaker, current draw)

<br>

---

<br>

### Motor Drivers:
Motor driver would need to handle 12V from motor, as well as estimate of 10A, have PWM speed control and dualdirectional control. (!! Possibly logic level shifter needed in case of 5V microcontroller !!)

| Feature | Suggestion |
|------|------------|
| Max voltage | 12V |
| Max current | 10A and higher |
| Control features | PWM, half or dual bridge |

**Option:** [VNH5019ATR-E - €8.79 DigiKey](https://www.digikey.nl/en/products/detail/stmicroelectronics/VNH5019ATR-E/3087980)
<br> 5.5V ~ 24V, 30A, Brushed DC, Parallel, PWM, Half Bridge

<br>

----

<br>

### Microcontrollers:
With microcontroller options, need for significat number of GPIOs must be considered, as well as PWM support with reliable frequency, relatively low power consumption and ease of expansion.
| Feature | Suggestion |
| ------- | ---------- |
| Voltage | 3.3V, 5V |
| PWM | 8+ channels, 10-20 kHz |
| Sensors support | I2C, SPI |

**Option:** ESP32-WROOM-32E - €13,95 <br>
https://www.reichelt.de/de/de/shop/produkt/entwicklungsboard_esp32-wroom-32e-341303


<br>

---

<br>

### Power Supply:





<br>

---

<br>
 
### Sensors:

Motion controller, distance, speaker, 

<br>

---

### Additionals:
Return bluetooth button