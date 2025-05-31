# Study of Class A Amplifier Operation

## Objective
To study the operation of Class A amplifier and determine voltage gain.

## Apparatus
| Sl. No. | Instruments/Apparatus      | Instrument Serial No. | Range | Quantity |
|---------|---------------------------|----------------------|-------|----------|
| 1       | Power Amplifier Trainer Kit| NV6522               | -     | 1        |
| 2       | 2 mm patch cords           | -                    | -     | 6        |
| 3       | Oscilloscope               | SM430                | -     | 1        |

## Setup Diagram
![Class A Amplifier Setup Diagram Placeholder](setup_class_a.png)

## Observations

| Sno. | Input Voltage | Output Voltage | Gain  |
|------|---------------|---------------|-------|
| 1    | 2V            | 1.4V          | 0.7   |
| 2    | 2.4V          | 1.8V          | 0.7   |
| 3    | 3.2V          | 2V            | 0.625 |
| 4    | 4V            | 2.2V          | 0.55  |
| 5    | 8V            | 6V            | 0.75  |

**Frequency:** 10 kHz

## Calculations
- \(V_0/V_{in} = 1.4/2 = 0.7\)
- \(V_0/V_{in} = 1.8/2.4 = 0.7\)
- \(V_0/V_{in} = 2/3.2 = 0.625\)
- \(V_0/V_{in} = 2.2/4 = 0.55\)
- \(V_0/V_{in} = 6/8 = 0.75\)

## Results and Comments
The voltage gain was found to be close to 0.6 or 60% for most input voltages. The output showed very little distortion compared to class B amplifiers, due to high linearity. The amplifier had a simple design with only one BJT transistor, making it excellent for applications where output signal quality is prioritized[2].

## LTspice Simulation

### Schematic
![LTspice Schematic Placeholder for Class A Amplifier](ltspice_schematic_class_a.png)

### Plot
![LTspice Simulation Plot Placeholder for Class A Amplifier](ltspice_plot_class_a.png)
