## Context
This file contains documentation on a system similar to our project — a remotely controlled car, which I reviewed to gain a better understanding of a real-world example.

The review process included the following steps:
- [Selecting a suitable product](#selecting-product)
- [Testing its basic functionality](#testing)
- [Disassembling it for autopsy](#autopsy)

### Selecting product
In selecting the product, my main criterion was that it had to be waterproof and capable of operating in a water environment. I considered several categories of RC-controlled toys, but most had limitations in relation to our project goals:

| Category | Why not | Example product |
|----------|---------|-----------------|
| RC boat | Uses a completely different propulsion system and mostly focuses on speed factor | [Link](https://www.amazon.com/Akargol-Boat-Light-Kids-Adults/dp/B0BPJ8D3H4/ref=sr_1_10?crid=3V81XOYBBVH0R&dib=eyJ2IjoiMSJ9.TATsdttgLigbiVFzcrZKPICuUk13ACbIU39_1EJibQl1omAv2AbiOgc0lwS-2-PzlbpqCvHGOMwj9Z-z01zqhCBetY4u0O2hxiMsbz8f-I1lFlyMLUZpeVowoaLNDq-DXbMJCAZrXd7OLLlKT0AnzY93vCXywt4X6iEGOuQhZoAqS28BAhAp1zCO98MP6OfxpZKaw98z-3kzz4CdZVIjYkLG8bENc6oArjYd5pUbn0JM5L4nqa2xpj6BMLXhxVfmx_RjBSwIl-AmzgYau5DueIzBfpk6n9-UwmY_jVNGK6c.R_1hW9y_EwBbTnYrDg2hQTOhCt6267SL5Xy3Oot-lXw&dib_tag=se&keywords=rc+boat&qid=1750319224&sprefix=rc+boat%2Caps%2C187&sr=8-10) |
| RC "head" water toy | Closer to our idea, but still uses a different type of movement mechanism | [Link](https://www.amazon.com/Doohickey-Control-Alligator-Simulates-Movement/dp/B0BYFSVNX1/ref=sr_1_5?crid=1CFYRUKP3XXJA&dib=eyJ2IjoiMSJ9.s0NlawsAlehwGz157YvDU8-UmwrgkPd0T8wDEquNtWfocq1Xxe4K3VQwzJ6EjvtYzlDWDqs31hvogedEZF-thlNFMRqxkcPEQhtAkPRApHK5lREbpijzGnsfdiCWJS9hDhgRBuGTqUcgiCQsORuUSB-ZhyKLU87f63tNHmhH5T-Rqb8YCQ-CF8H7qLRt-nNSQMGJ2oOUZ0wdj6HHdIcjh57T1PVtLvaw5ZjunO5_7-RbyX6Ta-ZFRuoY7A4cLVZbspXWeLdTVDRNRbtkWpWWOhN-Zh3z3SVPOye_s6kDKnbkBS00n_3uP2r1i4T8J92n_78n6WlnaxvTFdnfN2fPUJlhxD9IuuC8zPbJDJAVMBW0KlvTYrdYYUftrxhXYboPNKwFQyLDffikDWG6EyvkqK_oJBREzMpKaVgxxSznG70WTm9UUi9jcTp8CC13KNFK.mg6KVy7Xf4gFS8Cvj30YzgLAWCKHIePcNB_ZEe6nyJY&dib_tag=se&keywords=rc+duck&qid=1742322664&sprefix=rc+duck%2Caps%2C184&sr=8-5) |
| RC land car | Has similar wheel-based propulsion, but lacks waterproofing as a main focus | [Link](https://www.amazon.com/Kidcia-Remote-Control-Car-Christmas/dp/B0C9LXYX61/ref=sr_1_27?crid=2524AY861GMQO&dib=eyJ2IjoiMSJ9.VJOXEyPkSH29p3y9Z3Qf5LLGQUpvI0CAjMpXiY-7LyJY6kyLcWN5hU0mHISOQQSdIdFxtybrP1M7s-AwqH0-1ijkYdxsAendWuIC2pZPhIWA-CWqPMZ5YG9Jb4irBZrCzY8oVaZAyPU1nPenSR4IMmCLjGqWp1IAppCUmMhdESaw0S2mD5rVnmyCbsEhK3QJ6w7FAuVQBDPJgSXQfbIPVdVcyCOvL1E1jbASaNjW1Mf9VN41IWDWKidTCVNQT71J05aXT5fCgWI3qI1X2I3r2e26hiyQH8L3iUZGQq64hL4.mL5XUj75xecDMVORFJjROfLauKBT4Zh4StdSaeh4LtY&dib_tag=se&keywords=rc%2Bcar&qid=1750319264&sprefix=rc%2Bcar%2Caps%2C238&sr=8-27&th=1) |
| Underwater RC robots | Is way out of scope for our project | [Link](https://www.amazon.com/2-4G-Remote-Control-Shark-Toy/dp/B08CH6ZVL6/ref=sr_1_43?dib=eyJ2IjoiMSJ9.MAgTsf14ll_tA1A5hry340WsgquwEHUTNTmwz4apGefH68ZFJ2V7eSBQy-7Jgv9RuyHOAG0-CRjSI8Xb-utv9MGQGdy_6mYr_03GhIJxXDKSypBxSuwoDwZolTrldV_ItxYvdyHRhpKwUWtnwYc4DyCJr9fwOw6FgfFvGYKSOQ-TOMLQ4RsfgBH-1FKxvt3wmVzwVmIEnmMmbnY8bsqe22a6ynn8WC-bVkvNXLGtqqQuiLVVV3KhUzE_Yk70HwukIffZE2aTo9UuvnMbOLxp1Fx8WlchUdTh4Ae-W--82lWXp5fUBwsvFl0HqWgBBeuIeJElHi1yfLz8xvc-e0sTd6lLViSJYT7q7hyL0UGtgtM4Yktfif1WhKL0j6V8Wrk3NYi_d3XaDismONlZG-1c47-FroA8VbZHCbuxyeL14ud6PCPo0u-uqP66NpYyLvZN.IBOMYJzf4mxSv3Jvmlg2izl-XE5gcos3o6cKBt5TN84&dib_tag=se&keywords=rc+boat&qid=1742322570&sr=8-43)|

Eventually, I came across a [dual-environment RC car](https://www.amazon.nl/-/en/Amphibious-Controlled-Rotatable-Off-Road-Waterproof/dp/B0CYYYK7TG/ref=sr_1_7?crid=1S6HPJBUEGWW6&dib=eyJ2IjoiMSJ9.Vrycm-D9TMM76HAMZ8sNbtsD58ft4Jz37E7ZXsw7j-wB5VK2ZG1qOjC_agoPP-6mCa7MI4bGATSYuRP8Mi01T9pc6rR0Ng7xBifmykDuQqfpxclgSRy9GXMeDWzUjAo9-ObgObZHLz3o0sqTmlslqyujc7shoRsfmyn6XXXi04HmcZ066DKEbgSa67pOV7KK426gVjYc54lnpMmP2D7ltRpH2fG5qC9aVuAxMskuf9-58Tq2J84Pzd8pwmI2vfgLyp_gN47urlNZm-pSAlWP8uyIYvOFdDba4aWcvwvinDM.PakmM1Mh1BiprXVOJwy0POOIIJpdFEBs4fs26xyKGwA&dib_tag=se&keywords=rc%2Bwater%2Bcar&qid=1750322177&sprefix=rc%2Bwater%2Bcar%2Caps%2C76&sr=8-7&th=1), which turned out to be the most suitable choice. It operates with wheel-based propulsion and is specifically designed to function in both land and water environments. This made it an ideal reference for our duck project.

### Testing
To verify that the product is truly waterproof and meets the stated requirements, I tested it in both land and water environments. While this phase didn’t require any type of complexity, it was an important step before using the product as a reference for our own system.

[Land test - Video](/video/rc-car-test.mp4)


### Autopsy
The main goal of examining a product similar to our concept was to disassemble it and study real-world solutions to comparable design challenges.

![Dissasembly](/images/photos/rc_car_autopsy.jpeg)
![Insides](/images/photos/rc_car_insides.jpeg)

The internal layout turned out to be as simplified as possible, which is expected for a mass-produced toy. My primary interest was in the motor integration and the power supply circuit.

The car is powered by a 3.7V 1200mAh Li-Ion 18650 battery, placed in a separate compartment for easy user replacement and wrapped in heat-shrink film for insulation. 

![Battery](/images/photos/rc_car_battery.jpg)

This option is sufficient to power the system for approximately 2 hours using two [F130S-2365-36](https://www.robotshop.com/products/f130-15-3v-12000-rpm-brushed-dc-motor) DC motors. These are high-RPM (13,800 RPM at 3V) brushed motors with a basic two-wire interface for directional control. A small gear is directly mounted on the motor shaft.
![Motor](/images/photos/rc_car_motor.jpg)


What was of particular intrest to me was the way power was transferred to the wheels. Each motor is connected to a compact gearbox containing multiple plastic gears, which distribute power to both wheels on one side at the same time. This is a logical solution, considering the wheels on the same side are not needed to steer independently. The gearbox design also provides practical advantages, such as torque control, speed reduction, and an additional layer of isolation between internal components and the outer frame ensuring the overall water resistance.
![Gearbox](/images/photos/rc_car_gears.jpg)

### Summary
Overall, this review helped me to get a much better insight of what's to come in our project and what the futture challenges may be. Even though the case doesn't completely allign with our idea, it did provide possible solutions and features to think of while developing our version. 