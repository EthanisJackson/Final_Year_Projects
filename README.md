# Final_Year_Projects
Research and Design projects completed at the University of Pretoria in 2026
# Final Year Engineering Projects

**Ethan Jackson** | Mechanical Engineering, University of Pretoria (2026)

This repository contains my two final year projects: a research project on vibration-based fault detection and a design project on improving waste picker trolleys.

| Project | Type | Report |
|---|---|---|
| Multi-Channel Signal Processing for Impulsive Fault Detection in Rotating Machinery | Research (MRN 422) | [`MRN422_21481629_Final.pdf`](MRN422_21481629_Final.pdf) |
| Increasing the Productivity of Waste Reclamation Efforts | Design (MOX 410) | [`MOX410_Final_21481629_Final.pdf`](MOX410_Final_21481629_Final.pdf) |

---

## Research: Multi-Channel Signal Processing for Impulsive Fault Detection

**Focus:** Whether using several accelerometers instead of one makes rolling element bearing fault detection more reliable when random impulsive disturbances are present.

**What was done:**
- Built an 8-DOF lumped-parameter numerical bearing model to simulate healthy and faulty vibration signals with virtual accelerometers at different positions and orientations.
- Developed a full detection pipeline: automatic filtering (Power Envelope Spectrum and PESOgram), feature extraction, feature-level fusion with weighted PCA, and anomaly detection using a Gaussian Mixture Model trained on healthy data only.
- Validated the pipeline on both simulated data and measurements from a multi-sensor test bench.

**Key findings:**
- Multi-sensor combinations consistently matched or outperformed single sensors.
- Sensor orientation mattered more than proximity to the fault. Sensors aligned with the applied load gave the clearest fault signatures.
- Detection accuracy was high across speeds and fault severities, but depends heavily on the filtering stage. When impulses are not fully removed, healthy signals can be misclassified as faulty.

**Tools:** Python, signal processing, numerical modelling, statistical modelling.

---

## Design: Increasing the Productivity of Waste Reclamation Efforts

**Focus:** A low-cost add-on that reduces fatigue and improves control of the trolleys South African waste pickers use to move heavy loads.

**What was done:**
- Analysed user needs and set technical design specifications.
- Generated and ranked concepts using weighted decision matrices.
- Designed a rear bicycle wheel assembly with a lockable steering pin, a universal attachment bracket that fits many trolley types, and a pulling handle with a manual brake.
- Sized components using hand calculations (straight and curved beam theory, von Mises stress, bolt stress) with a global safety factor of 2. The wheel mounting arm is S355J2 steel with a final safety factor of 2.45.
- Produced 3D models, manufacturing and assembly drawings, a cost analysis and an environmental and safety review.

**Outcome:** The design meets the load, temperature and ingress protection specifications. It does not yet meet the mass or cost targets (the full package costs R2 587), though bulk manufacturing could reduce this. Physical testing and field trials are recommended next steps.

**Tools:** SolidWorks, Python, mechanical design and stress analysis.
