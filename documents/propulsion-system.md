# Notes on Propulsion System and Motor Connection

## Context

The propulsion system of the amphibious robotic duck is based on two paddle wheels "Mississippi" style, which must be  connected to motors with the following specification:

- Spline: 25-tooth, 5.96 mm outer diameter
- The motor comes with a servo horn, but it is not suitable for directly mounting the wheel.

The primary goal of this research was to identify onnection mechanisms between the motor spline and a custom 3D-printed paddle wheel.

---

## Key Considerations

- The spline connection must transfer torque properly without slipping.
- The connection must have slight room for misplacement due to water movement.
- It should be detachable for maintenance, but also secure during operation.

---

## Explored Solutions

| Example Solution | Why It Doesn’t Work |
|------------------|---------------------|
| [3D model on Thingiverse](https://www.thingiverse.com/thing:2358211) | Spline pattern does not match, and the adapter is too large to be mounted securely on a 5.96 mm OD shaft. |
| [Forum post on motor-to-wheel connection](https://www.electro-tech-online.com/threads/connecting-motor-to-wheel.153148/) | Suggests using set screws and couplers, but does not consider specific spline geometry. Also risk of slipping under wet conditions. |

---

## Types of Motor-to-Wheel Connectors Researched

### 1. **Servo Horn Adapter with Custom Plate**
- Uses the included servo horn as a mounting base.
- Custom 3D-printed plate is attached to the horn using small bolts.
- Pros: Cheap, makes use of existing hardware.
- Cons: Low torque transfer, horn might flex or loosen.

### 2. **Set Screw Couple**
- A plastic coupler with set screws and a 3D-printed sleeve to adapt from spline to smooth shaft.
- Pros: High torque transfer, easily replaceable.
- Cons: It would be hard to model one that perfectly matches the lenght of our spline and doesn't get in the way of overall structure.

### 3. **Spline-Matched 3D-Printed Insert (Press-Fit)**
- The paddle wheel is printed with an internal spline connector matching the servo horn.
- Pros: Clean, integrated design.
- Cons: Requires vey detailed printing and modeling; brittle also big chance of fast wearing out.

### 4. **Cross-Drilled Pin Lock + Friction Fit**
- A tight-fitting shaft mount with a drilled hole for a small metal bolt.
- Pros: Mechanically strong, tolerates wear.
- Cons: Requires precision drilling, may loosen with vibration.

---