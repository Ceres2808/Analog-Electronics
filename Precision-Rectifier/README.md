# Precision Half and Full Wave Rectifier using Op-Amp

## Objective
To verify the output voltage of precision half wave rectifier and full wave rectifier using OP-AMP.

## Theory
Ordinary diodes cannot rectify voltages below 0.6V (the cut-in voltage). The precision rectifier (super diode) uses an op-amp to behave like an ideal diode and rectifier, making it useful for high-precision signal processing[6].

- **Half Wave Rectifier:** Converts AC to positive DC using one diode.
- **Full Wave Rectifier:** Converts AC to pulsating DC using both half cycles of the input, employing two diodes.

## Circuit Diagram
![Circuit Diagram Placeholder for Precision Rectifier]([Half_Wave\Half_Wave.jpg](Half_Wave\Half_Wave.jpg))
![Circuit Diagram Placeholder for Precision Rectifier](Full_Wave\Full_Wave.jpg)

## Apparatus
| Sl. No. | Apparatus                | Range        | Quantity |
|---------|-------------------------|--------------|----------|
| 1       | Op-Amp                  | -            | 3        |
| 2       | Resistors               | -            | 7        |
| 3       | Diodes                  | -            | 4        |
| 4       | Bread Board             | -            | 1        |
| 5       | Variable DC Power Supply| 10mV–30V     | 1        |
| 6       | Function Generator      | -            | 1        |
| 7       | Oscilloscope            | -            | 1        |
| 8       | Connecting wires        | -            | 14       |

## Observations

| Vin    | Vout (Half) | % Error (Half) | Vout (Full) | % Error (Full) |
|--------|-------------|----------------|-------------|----------------|
| 0.695  | 0.720       | 3.6            | 0.76        | 9.3            |
| 0.615  | 0.640       | 4.16           | 0.680       | 15.2           |
| 0.55   | 0.520       | 5.45           | 0.520       | 0              |
| 0.388  | 0.400       | 3.04           | 0.480       | 15.1           |
| 0.278  | 0.320       | 15.1           | 0.360       | 15.01          |

## Results and Conclusions
The experiments confirm the effectiveness of both half and full wave rectifiers in converting AC signals to DC. Both designs outperform traditional diode rectifiers, validating their use in low-voltage applications and various electronic circuits.

## LTspice Simulation

### Schematic
![LTspice Schematic Placeholder for Precision Rectifier](Half_Wave\schematic.png)
![LTspice Schematic Placeholder for Precision Rectifier](Full_Wave\schematic.png)

### Plot
![LTspice Simulation Plot Placeholder for Precision Rectifier](Half_Wave\plot.png)
![LTspice Simulation Plot Placeholder for Precision Rectifier](Full_Wave\plot.png)

### Osciloscope Plot
![DSO](Half_Wave\DSO.jpg)
![DSO](Full_Wave\DSO.jpg)
