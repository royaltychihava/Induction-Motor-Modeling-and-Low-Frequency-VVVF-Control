# Induction Motor Modeling and Low-Frequency VVVF Control Analysis

## Overview
This project focuses on deriving induction motor performance parameters from manufacturer datasheet values and validating them through simulation. It also investigates motor behavior at low frequencies using Variable Voltage Variable Frequency (VVVF) control.

---

## Objectives
- Derive key motor parameters from manufacturer datasheet  
- Validate parameters using simulation (no-load and locked rotor tests)  
- Analyze motor performance at low frequencies using VVVF control  

---

## Parameter Derivation

### Manufacturer Datasheet
![Motor Datasheet](INSERT_IMAGE_LINK_HERE)

Motor parameters were derived from the manufacturer’s datasheet and used to build the simulation model.

---

## Simulation Setup (PLECS)

The induction motor was simulated using the Direct-On-Line (DOL) method to perform:

- No-load test  
- Locked rotor test  

These tests were used to validate the derived parameters.

---

## Model Validation

### Dynamic Performance
![Motor Performance](INSERT_IMAGE_LINK_HERE)

This plot shows:
- Motor speed vs time  
- Electromagnetic torque vs time  
- Load torque vs time  

The simulation validates:
- Pull-out torque  
- Rated motor speed  
- Full-load torque  

---

## Low-Frequency Operation Analysis

### VVVF Control at 5 Hz
![Low Frequency Operation](INSERT_IMAGE_LINK_HERE)

Simulation of no-load and full-load operation at 5 Hz using VVVF control to maintain constant flux.

Key observations:
- No-load synchronous speed ≈ 10 rpm  
- Loaded speed ≈ 8 rpm  
- Speed drop ≈ 20% due to increased slip  

---

## Key Insights

- Derived parameters closely match simulation results, confirming model accuracy  
- Induction motor maintains operation under rated load at 5 Hz  
- Required slip frequency for rated load ≈ 1.15 Hz  
- Since 5 Hz > 1.15 Hz, the motor can sustain rotation under load at low frequency  
- At frequencies below 1.15 Hz (e.g., 1 Hz), the motor cannot produce sufficient torque to drive the load  

---

## Tools Used
- PLECS  

---

## Files
- Project report (PDF)

---

## Conclusion
This project demonstrates accurate parameter derivation and validation of an induction motor model. It also highlights that while VVVF control enables low-frequency operation, there exists a minimum frequency threshold required to sustain load torque, below which the motor cannot operate effectively.

---

## Author
Royalty Holyworth Chihava
