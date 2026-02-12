**5-Bit Flash ADC in 45nm Technology**

This repository contains the design and implementation of a high-speed 5-Bit Flash Analog-to-Digital Converter (ADC), fabricated in the GPDK 45nm technology node. The project includes schematics, layout, and simulation results for a converter designed to accurately sample and convert a 33.3 MHz analog input signal.

Repository Structure
The repository is organized as follows:

images/ - Screenshots of the complete design

schematic/ - Circuit schematics including Sample-and-Hold, R-2R ladder, comparator bank, and encoder

simulation/ - Simulation results and testbenches for performance verification


**Key Features & Architecture**
Resolution: 5-bit (32 quantization levels)

Input Frequency: Supports up to 33.3 MHz

Sample-and-Hold (S/H): Integrated to ensure input stability during conversion

Reference Generation: R-2R ladder network for improved linearity and matching

Core Conversion: 31-comparator bank for single-cycle conversion

Priority Encoder: Custom tree-based encoder using 16-input OR gates for low latency

**Implementation Details**
PDK: GPDK 45nm

Design Tools: Cadence Virtuoso (schematic & layout), Spectre (simulation)

Design Views: Schematic and simulation waveforms

**Design Screenshots**
The repository includes screenshots of:

Sample-and-Hold circuit schematic

R-2R ladder network implementation

Comparator bank design

Priority encoder architecture with 16-input OR gates

Complete ADC layout view

**Performance Goals**
High-speed conversion suitable for RF applications

Stable operation at 33.3 MHz input frequency

Low power consumption and compact layout in 45nm technology

**Simulation Results**
Simulation results confirming the ADC's performance it coverts the analog input to digital as expected, but there are still issue to work upon the conversion is not accurate. 

## 📄 Technical Report

[View the full PDF report](report/https://github.com/AryanSingh0813/5bit_ADC/blob/main/5bitADC.pdf)

