# Paper List (ISCA2025)

## 1. Hardware-aware Calibration Protocol for Quantum Computers

### Blueprint for the paper

- Calibration in quantum computers: Quantum computer is error-prone (0.1% and 1% error for single qubit gate and two qubit gate, respectively). To maintain the high fidelity, good calibration protocol is important. Also, calibration is crucial for quantum error correction (QEC), because the calibration can make physical error rate below the threshold.
- Problem of Calibration: Calibration requires hours/days for its completion. This can introduce the system drift that affects the system performance.

  - Q) What is the system drift?
  - Q) What is the system performance?
- How to improve the fidelity by calibration?

  - Major factor-1 (Getting a better control of microwaves): generating accurate microwave pulses (i.e., pulse amplitudes, frequenciees, durations).
  - Major factor-2 (Refresh): performing regular calibrations to compensate for system drift and external perturbations (hourly/daily intervals).
- Limitations of Prior Works:

  - (1) Existing calibration protocol does not consider the awareness of differences between physical qubits, even if it consider the trade-off between the calibration time and fidelity. This problem becomes severe when it comes to two-qubit gate operations (e.g., cross-resonance gates).

    - (a) What happens in CR gate? An unwanted excitation in control qubit occurs due to off-resonant drives.
    - Q) What is off-resonant drives?
  - (2) The calibration protocol is serialized.
- Insights to overcome the limitation:

  - (1) Profiling qubit pairs and evaluate their responses. The standard derivative removal by adiabatic gate (DRAG) technique addresses this issue.

    - Q) Why two pairs?, What is adiabatic gate?
  - (2) Especially, multi-derivative DRQG offers a  solution by applying recursive corrections to suppress multiple transitions simulataneously. Graph traverse to calibrate quantum computer in parallel.
- Design: Three calibration policies
- (1) Brute-force clustering
- (2) Topology-oriented representative
- (3) Hardware-oriented policy

###

## 2. ARTERY Fast Quantum Feedback using Branch Prediction

## 3. Constant-Rate Entanglement Distillation for Fast Quantum Interconnects

## 4. S-SYNC Shuttle and Swap Co-Optimization in Quantum Charge-Coupled Devices

## 5. Qtenon Towards Low-Latency Architecture Integration for Accelerating Hybrid Quantum-Classical Computing

## 6. Synchronization for Fault-Tolerant Quantum Computers

## 7. Variational Quantum Algorithms in the era of Early Fault

## 8. swiper_Minimizing Fault-Tolerant Quantum Program Latency via Speculative Window Decoding
