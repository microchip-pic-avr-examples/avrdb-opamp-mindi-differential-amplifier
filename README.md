![Microchip logo](images/microchip.png)
# Getting started with Mindi™ simulation and AVR®DB microcontrollers
This guide will get you up and running with simulating the analog OPAMP module in AVR DB family devices using the Mindi simulation tool.
## Configuration: Differential Amplifier
The differential amplifier op amp configuration outputs the amplified difference between two signals. The amplification can be configured by setting the feedback divider.

![Differential Amplifier](images/configuration.png)

### Mindi Simulation
![Mindi](images/mplab-mindi-analog-simulator.png)

Download and open the **Mindi schematic [here](https://github.com/microchip-pic-avr-examples/avrdb-opamp-mindi-differential-amplifier/releases/latest)**

Press the _play_ button to simulate with an example stimulus source.

### Tweaking
The amplification of the differential amplifier can be adjusted to any of 8 levels from 0.06 to 15 by changing the MUXWIP value in the control register. The Mindi schematic contains a table detailing the levels of gain and their associated register and resistor values.

### Updating composer fields
Once the desired result has been verified with Mindi simulation, the corrected values should be moved back into MCC/Start by copying resistor configurations across to the composer of your preference.

### Don't have Mindi?
Download and install [Mindi simulation tool](https://www.microchip.com/mplab/mplab-mindi)
