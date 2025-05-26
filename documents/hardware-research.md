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
*Primarly*: As to more detailed specifications, I would consider options with voltage starting from **12V**, as 5V introduce quite significant power limitations (less voltage requires more current, hence specialized high-current motor drivers). <br>
*Week 7 update:* After a lot of consideration and research, we have been advised to switch to 6V motors. This decision makes the possibility of combining different modules easier, but introduces the risk of motor being too weak to operate in the water enviroment. At the same time, 12V motors required rather complicated way of powering, so we decided to take on the risk of 5V mototrs. <br> 
<br> Considering targeted water enviroment, RPM range should start at slow speeds to push water efficiently, but at the same higher boundary should be quite big to ensure variety of manouvering. This brings us to approximate of **50-150 RPM**. In case of high-speed motors we would also need to consider gear reduction ratios. <br>
To figure out torque requirements, we need to know wheels specifications (paddle bades, radius), but safe minimum point would be around **1 Nm**.

| Feature | Suggestion |
|------|------------|
| Voltage | 5V - 9V |
| RPM | 50 - 150 rpm |
| Torque | 1Nm and higher |
| Power | 30W or 50W |


**Option 12V**: [RS PRO Brushed Geared DC Geared Motor - €39.40 RS](https://nl.rs-online.com/web/p/dc-motors/2389670) <br>
19.8 W, 12 V dc, 59 Ncm, 84 rpm, 6mm Shaft Diameter <br> (a bit weaker, current draw) <br>
**Option 6V**: [Parallax Feedback 360° High-Speed Servo - €25.82 DigiKey](https://www.digikey.nl/en/products/detail/parallax-inc/900-00360/7707660) <br>
Servomotor RC 120 RPM 6V
<br>

---

<br>

### Motor Drivers:
Motor driver would need to handle 12V (6V) from motor, as well as estimate of 1A, have PWM speed control and dualdirectional control. 
For case of 6V motor, the driver isn't neseccary, but would provide precise control over RPM and additional isolation from power spikes and other possible power problems. 

| Feature | Suggestion |
|------|------------|
| Max voltage | 12V |
| Max current | 1A and higher |
| Control features | PWM, half or dual bridge |

**Option 12V:** [VNH5019ATR-E - €8.79 DigiKey](https://www.digikey.nl/en/products/detail/stmicroelectronics/VNH5019ATR-E/3087980)
<br> 5.5V ~ 24V, 30A, Brushed DC, Parallel, PWM, Half Bridge <br>
**Option 6V:** [TB6612FNG DUAL MOTOR DRIVER - €4.57 DigiKey](https://www.digikey.nl/en/products/detail/pololu/713/10450399?s=N4IgTCBcDaICoCEBsSCMYBiA5A4iAugL5A) <br>
Brushed 4.5 ~ 13.5VDC Supply 1A 4.5 ~ 13.5V Load

<br>


----

<br>

### Microcontrollers:
With microcontroller options, need for significat number of GPIOs must be considered, as well as PWM support with reliable frequency, relatively low power consumption and ease of expansion. Considering experience with LilyGO TTGO v1.6.1 it would be a sufficient option as well,
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

### Power:

Minimum: 2500mAh Li-ion or LiPo with corresponding to the moters voltage.

<br>

---

<br>
 
### Sensors:

For sensors the intended functionality needs to be heavily considered. While the level of the project doesn't expect the highest precision or control, the sensor modulees still should be sufficient for the intended purposes. Besides that, power limitations must be taken into consideration, bringing the possible voltage options to **3.3 - 5V**. 

Separately for each sensor:  <br>
[Sen-15559 HC-SR04 Ultrasonic Distance Sensor](https://www.distrelec.nl/en/hc-sr04-ultrasonic-distance-sensor-sparkfun-electronics-sen-15569/p/30160395?trackQuery=Distance%20sensor&pos=5&origPos=3&origPageSize=50&track=true&sid=1bde0xNWYx&itemList=search) - 5v, analogue
<br>

[Open-Smart MP3 Module with Speaker](https://www.tinytronics.nl/en/audio/audio-sources/open-smart-mp3-module-with-speaker) - 3.3V ~ 5V, UART, USB

---

### Additionals:
Return bluetooth button