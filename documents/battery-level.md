## LiPo battery SOC tracking

SOC (State of Charge) represents the remaining charge in a battery and tracking it in standard "dumb" LiPo batteries is usually done by approximating capacity based on the battery's voltage level. For example, in a standard 1S LiPo battery, the voltage is 4.2 V when fully charged. As the battery discharges, the voltage decreases — reaching approximately 3.73 V when the charge drops to around 20%.

By tracking this voltage drop curve, it's possible to estimate the current SOC. 

![LiPo SOCs](/images/lipo-voltage.png)

The tracking of the voltage level can be done through A/D conversion.

### Our case

Initially, we planned to monitor the battery level using A/D conversion directly from one of the LiPo batteries. This  would have allowed us to read the voltage curve and detect decrease in voltage.
However, reviewing the microcontroller's specifications, we found the following note: "The pins on the board are directly connected to the ESP32 chip and are therefore only suitable for **3.3V** signals." Using one of the 2 LiPo batteries would result in 3.7V and around 4.2V in charged state, which exceeds the 3.3V limit. 

Knowing that, we are left with little to no options: route the A/D conversion through resistors (voltage divider) to decrease the voltage.

A voltage divider circuit is a circuit that takes a higher voltage and converts it to a lower one by using a pair of resistors. 

Votage Divider Formula: Vout = Vs*R2/(R1+R2)

To decrease coltage by half with voltage divider - use two same resistors.

After researching online, we started considering using both batteries, so entire 7.4, for the conversion due to difficulties in connection in the case of only one. But after multiple discussions with coaches, we did stick with the original plan of using only one battery with 3.7V.

The final resistors values are: 47K and 12K, leaving us with the formula being 3.018V = 4.2V * 47k Ohm / (47k Ohm + 12k Ohm) where

| Variable | Meaning | Value |
|----------|---------|-------|
| Vout | Output voltage after the divider | 3.018V |
| Vs | Source voltage | 4.2V |
| R2 | Resistor connected to ground | 47K Ohm |
| R1 | Resistor connected to power | 12K Ohm | 

<br>

### Used sources
| Source | Description |
|---|---|
| [Ufine Article](https://www.ufinebattery.com/blog/useful-overview-of-lipo-battery-voltage/) | General Introduction into LiPo SOC |
| [RCdronegood Article](https://www.rcdronegood.com/looking-after-quadcoper-lipo-battery-tips/) | Charging tips, but quadrocoper batteries |
| [LilyGo TTGO Specifications](https://www.tinytronics.nl/en/development-boards/microcontroller-boards/with-lora/lilygo-ttgo-t3-lora32-868mhz-v1.6.1-esp32) | 
| [Arduino Forum](https://forum.arduino.cc/t/reading-a-lipo-voltage-with-a-3-3v-arduino/1084802/9) | Discussion about reading a lipo voltage with 3.3V |
| [Voltage Divider Calculator](https://ohmslawcalculator.com/voltage-divider-calculator) | Calculator for resistors |
| [Jeelabs Article](https://jeelabs.org/2013/05/16/measuring-the-battery-without-draining-it/) | On how to measure battery witout draining it |
| [Engineers Garage Article](https://www.engineersgarage.com/string-array-of-batteries-monitoring-with-arduino/) | On how to monitor individual battery in a series |
| [Youtube Video](https://www.youtube.com/watch?v=JGXdi7XcQi8&t) | Explanation of Voltage Divider |