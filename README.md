# 2-bit Flash ADC using Comparators

## Overview
This project implements a 2-bit flash ADC using ideal comparators and a resistor ladder network.

## Working Principle
- A resistor ladder generates reference voltages: 1.25V, 2.5V, 3.75V
- Input voltage is compared against these thresholds
- Outputs form a thermometer code
- Logic gates convert thermometer code to 2-bit binary output

## Resolution
Resolution = 5V / 4 = 1.25V per step

## Truth Table

| Vin Range | Output |
|----------|--------|
| 0–1.25V  | 00     |
| 1.25–2.5V| 01     |
| 2.5–3.75V| 10     |
| 3.75–5V  | 11     |

## Files
- adc.asc (LTspice circuit)
