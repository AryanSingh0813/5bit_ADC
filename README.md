**5 Bit Flash ADC:**
This repository contains the design of a high-speed 5-Bit Flash Analog-to-Digital Converter (ADC), implemented in the GPDK 45nm technology node. The ADC is designed to accurately sample and convert a 33.3 MHz analog input signal into a 5-bit digital output at a high sampling rate.

**Key Features & Architecture**
Resolution & Speed: 5-bit resolution (32 levels) with conversion speeds suitable for high-frequency applications.

Input Frequency: Designed for stable operation with a 33.3 MHz analog input.

Sample-and-Hold (S/H): An integrated S/H circuit ensures the input voltage is stable during the conversion process, which is critical for achieving accuracy and preventing metastability at high speeds.

Reference Generation: Utilizes an R-2R Ladder network for generating precise and well-matched reference voltages for the comparator bank, offering advantages in layout and linearity over a standard resistor string.

Core Conversion: A parallel bank of 31 comparators performs the ultra-fast analog-to-digital conversion in a single clock cycle.

Priority Encoder: The thermometer-to-binary conversion is handled by a custom digital priority encoder. For optimal performance in the 45nm process, the encoder is designed using a tree structure with high-speed 16-input OR gates to minimize critical path delay.

**Technology**

PDK: GPDK 45nm
Tools: Cadence Virtuoso (for schematic and layout), Spectre (for simulation)

**Performance Goals**

The primary design goals are to maintain:
High-Speed operation enabled by the flash architecture and optimized encoder logic.
Stability for the target 33.3 MHz input, achieved by the front-end Sample-and-Hold circuit.
