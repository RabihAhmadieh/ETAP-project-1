# ETAP-project-1
This project presents the modeling and analysis of a simple industrial electrical distribution system using ETAP 19.0. The objective is to perform a complete load flow and short-circuit study following common engineering practices used in industrial power system design.

The project demonstrates how to evaluate equipment loading, bus voltages, power losses, and fault currents to ensure the electrical system operates safely and reliably.

## Objectives
Model an industrial electrical distribution system in ETAP.

Perform Load Flow Analysis.

Perform ANSI Short-Circuit Analysis. 

Evaluate transformer loading.

Verify voltage profile.

Calculate system losses.

Determine the required interrupting capacity of the LV circuit breaker.

## System Description

The system consists of:

Utility Source: 11 kV, 250 MVAsc

Transformer: 2 MVA, 11/0.4 kV, Dyn11, 6% impedance

LV Busduct: 3200 A

Motor 1: 500 kW

Motor 2: 300 kW

Static Load: 700 kVA

## Software
ETAP 19.0

ANSI Short-Circuit Method

Adaptive Newton-Raphson Load Flow Solver


## Studies Performed
### 1. Load Flow Analysis

The load flow study evaluates:

Bus voltages

Active and reactive power

Transformer loading

Branch loading

Voltage drop

System losses

Power factor

### 2. Short-Circuit Analysis

The short-circuit study evaluates:

Three-phase fault current

Line-to-ground fault current

Fault contribution from motors

Equipment interrupting duty

## Results Summary

| Parameter                     |          Result |
| ----------------------------- | --------------: |
| Utility Voltage               |           11 kV |
| Transformer Rating            |           2 MVA |
| Transformer Loading           |          81.2 % |
| Total Demand                  |       1.624 MVA |
| Power Factor                  | 90.36 % Lagging |
| Minimum Bus Voltage           |         97.37 % |
| Maximum 3-Phase Fault Current |        51.19 kA |
| Recommended LV Breaker Rating |           65 kA |


## Engineering Discussion
### Load Flow

The transformer operates within its rated capacity with approximately 81% loading, indicating adequate capacity for the connected loads.

Replacing the original LV cable with a 3200 A busduct eliminated the branch overload observed during the initial design.

The minimum operating voltage is approximately 97.4%, which is slightly below the nominal value but acceptable for this study.

### Short-Circuit

The maximum three-phase fault current occurs on the 400 V bus and is approximately 51.2 kA.

The two synchronous motors contribute additional fault current during the first few cycles of the fault.

Since the calculated fault current exceeds 50 kA, a 65 kA interrupting capacity circuit breaker is recommended for the LV main incomer.

## Conclusions

This study demonstrates the complete workflow of industrial power system analysis using ETAP.

The project includes:

Electrical system modeling

Load flow analysis

Short-circuit analysis

Equipment loading assessment

Voltage profile evaluation

Engineering recommendations

The analysis confirms that the transformer operates within its rating, the upgraded busduct eliminates the overload condition, and a 65 kA LV breaker is required to safely interrupt the calculated fault current.

## Author

## Rabih Kamal Al Ahmadieh

Electrical Engineer | Power Systems | ETAP | Machine Learning for Power Systems
