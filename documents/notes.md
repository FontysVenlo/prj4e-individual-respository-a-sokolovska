### Components
#### Motors:
As of now, main options for the motors are brushed DC motors with H-bridge or BLCD with gearboxes, as we need continious rotation at high torque, relative ease of control and relatively cheap price. <br>
As to more detailed specifications, I would consider options with voltage starting from **12V**, as 5V introduce quite significant power limitations (less voltage requires more current, hence specialized high-current motor drivers). <br> Considering targeted water enviroment, RPM range should start at slow speeds to push water efficiently, but at the same higher boundary should be quite big to ensure options of manouvering. This brings us to approximate of **50-150 RPM**. In case of high-speed motors we would also need to consider gear reduction ratios. <br>
To figure out torque requirements, we need to know wheels specifications (paddle bades, radius), but safe minimum point would be around **1 Nm**.

| Spec | Suggestion |
|------|------------|
| Voltage | 12V and higher |
| RPM | 50 - 150 rpm |
| Torque | 1Nm and higher |
| Power | 30W or 50W |
| Current Draw | 5A - 10A |


**Option**: 37GB555 DC Geared Motor - €16.69 Aliexpress <br>
24V at 100rpm (75 rpm load, torque 1.18 Nm, current 7.5A)  https://nl.aliexpress.com/item/32849218686.html?gatewayAdapt=glo2nld#nav-specification