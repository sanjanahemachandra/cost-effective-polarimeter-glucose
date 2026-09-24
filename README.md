# Construction & Calibration of a Cost-Effective Polarimeter
## For Determining the Concentration and Chirality of Glucose

## Overview
A 5-week open-ended group project carried out as part of
**PH1023 - General Physics Laboratory II** at the
**Department of Physics, University of Colombo**.
A fully functional, low-cost polarimeter was designed,
constructed, and calibrated from scratch to determine the
optical rotation, concentration, and chirality of glucose
solutions. The device was built using 3D-printed components,
off-the-shelf electronics, and LCD-extracted polarizing
filters; achieving results within 0.76% of the theoretical
specific rotation of glucose.

## My Role
- **Group Leader** - coordinated tasks, timeline, and 
  report preparation
- Led glucose solution preparation across six concentrations
  (1.25M to 3.5M)
- Conducted polarimeter measurements and data collection
- Wrote the project proposal and individual final report
- Analyzed results and verified against Biot's Law and 
  Malus' Law

## Physics Behind the Project

### Biot's Law of Optical Rotation
Optically active substances like glucose rotate the plane
of polarized light. The rotation angle θ is given by:

θ = [α] · c · l

Where:
- [α] = specific rotation of the substance
- c = concentration of the solution
- l = path length of light through the sample

### Malus' Law
When polarized light passes through a second polarizer,
transmitted intensity follows:

I = I₀ cos²(θ)

This principle was used to detect the angle of minimum
intensity, corresponding to the optical rotation angle.

## Device Components
| Component | Details |
|---|---|
| Light Source | SMD RGB LED (1W) in parabolic reflector |
| Polarizing Filters | Extracted from LCD screen |
| Analyzer Rotation | Stepper motor (28BJ-48) + ULN2003 driver |
| Microcontroller | ESP32 Dev Module |
| Light Sensor | TCS3472 RGB sensor + photodiode |
| Sample Holder | Glass cuvette (16×4×3 cm) |
| Gears | 3D-printed spur gears (25-tooth & 100-tooth) |
| Assembly | Breadboard, jumper cables, connecting wires |

## Methodology

### Solution Preparation
- Prepared a 3.5M glucose stock solution
- Performed systematic dilution in 0.50M increments
- Resulted in 6 glucose solutions: 1.25M to 3.5M
- Used blank solution (distilled water) as zero reference

### Measurement Process
- Aligned polarimeter for proper light transmission
- Stepper motor rotated analyzer to find minimum intensity
  (dark point) - corresponding to optical rotation angle
- RGB sensor and photodiode detected intensity variations
- Repeated for all six glucose concentrations

## Results

| Concentration (mol dm⁻³) | Concentration (g/cm³) | Optical Rotation (°) |
|---|---|---|
| 3.50 | 0.630 | 45.4 ± 0.5 |
| 3.25 | 0.585 | 45.7 ± 0.5 |
| 2.75 | 0.495 | 34.3 ± 0.5 |
| 2.25 | 0.405 | 32.4 ± 0.5 |
| 1.75 | 0.315 | 22.0 ± 0.5 |
| 1.25 | 0.225 | 18.4 ± 0.5 |

### Key Findings
- Strong linear correlation between concentration and 
  optical rotation: R² = 0.9651
- Experimental specific rotation of glucose:
  **53.1 ± 4.8 °·ml·g⁻¹·dm⁻¹** (at 27°C, 620nm)
- Theoretical value: 52.7 °·ml·g⁻¹·dm⁻¹ (at 25°C)
- **Percentage deviation: only 0.76%**
- Clockwise rotation confirmed sample as **D-glucose**
  (dextrorotatory)
- Malus' Law verified through cos²θ intensity dependence

## Tools & Technologies
- **ESP32 + Arduino IDE** - stepper motor control and
  data acquisition (implemented by team member)
- **3D printing** - custom gear and sample holder fabrication
- **Python (Matplotlib)** - data analysis and graph plotting
- **Microsoft Excel** - data recording and processing

## Files in This Repository
- `Cost-effective_Polarimeter.pdf`: individual final report
- `Group_6_-_Project_Proposal.pdf`: project proposal

## Notes
The stepper motor and ESP32 control system was implemented
using Arduino IDE by a team member specializing in embedded
systems. The Arduino code is not included here as it was
not my contribution to the project.

## Applications of This Work
Polarimetry has real-world relevance in:
- **Sugar industry** - quality control of sugar concentration
- **Pharmaceuticals** - identifying chiral molecules to
  prevent adverse drug effects from wrong enantiomers
- **Clinical diagnostics** - measuring glucose in biological
  samples for diabetes management
- **Education** - demonstrating optical principles at low cost

## Team
Group 6 - General Physics Laboratory II

1st Year, 2nd Semester (February 2025)

## Course
PH1023 - General Physics Laboratory II, 
Department of Physics, Faculty of Science, University of Colombo
