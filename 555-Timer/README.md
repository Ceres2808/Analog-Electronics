# Astable Multivibrator using 555 Timer

## Objective
To design and study Astable Multivibrator using 555 timer.

## Theory
When IC555 is configured as an astable multivibrator, both the trigger and threshold inputs (pins 2, 6) are connected together and to a capacitor. The capacitor charges towards the supply voltage through resistors \(R_1\) and \(R_2\). The discharge pin (7) is connected to the junction of those resistors. When power is applied, the capacitor starts charging through \(R_1\) and \(R_2\). When the capacitor voltage reaches \(2/3\) of the supply, the upper comparator triggers, resetting the flip-flop and switching the output low. The internal transistor \(T_1\) conducts, effectively connecting \(R_2\) to ground, allowing the capacitor to discharge through \(R_2\). The result is a continuous stream of rectangular pulses[1].

## Circuit Diagram
![Circuit Diagram Placeholder for Astable Multivibrator](circuit_astable_555.png)

## Apparatus
| Sl. No. | Instruments/Apparatus | Maker's Name | Specification | Quantity |
|---------|----------------------|--------------|---------------|----------|
| 1       | IC 555               | -            | -             | 1        |
| 2       | Resistors            | -            | 494kΩ, 496kΩ, 1kΩ | 3    |
| 3       | Capacitors           | -            | 12.9nF, 2.29µF | 2     |
| 4       | Bread Board          | -            | -             | 1        |
| 5       | DC Power Supply      | Hi-Watt      | 9V            | 2        |
| 6       | LED                  | -            | -             | 1        |
| 7       | Oscilloscope         | Rigol        | -             | 1        |
| 8       | Connecting wires     | -            | -             | 7        |

## Observations
- **Calculations:**
  - \(T_{ON} = 0.693 \times (R_1 + R_2) \times C_1 = 1.57\,s\)
  - \(T_{OFF} = 0.693 \times R_2 \times C_1 = 0.785\,s\)
  - \(T_{ON}\) % error \(= \frac{|1.58-1.57|}{1.57} \times 100 = 0.64\%\)
  - \(T_{OFF}\) % error \(= \left|\frac{0.78-0.79}{0.78}\right| \times 100 = 1.28\%\)

## Results and Conclusions
The error for \(T_{ON}\) is 0.64%, and for \(T_{OFF}\) is 1.24%. This shows that the formula used for theoretical calculations works satisfactorily. The frequency and duty cycle can be adjusted by varying \(R_1\), \(R_2\), and \(C_1\), making the circuit versatile for clock pulses, light flashing, and tone generation[1].

## LTspice Simulation

### Schematic
![LTspice Schematic Placeholder for Astable Multivibrator](ltspice_schematic_astable.png)

### Plot
![LTspice Simulation Plot Placeholder for Astable Multivibrator](ltspice_plot_astable.png)
