# Paper List (ISCA2025)

## 1. Hardware-aware Calibration Protocol for Quantum Computers

- *Problem of Calibration Calibration* requires hours/days for its completion. This can introduce the system drift that affects the system performance.

- *Why does calibration important?* Quantum computer is error-prone (0.1% and 1% error for single qubit gate and two qubit gate, respectively).
<!-- //  To maintain the high fidelity, good calibration protocol is important. Also, calibration is crucial for quantum error correction (QEC), because the calibration can make physical error rate below the threshold. -->

  <!-- - Q) What is the system drift?
  - Q) What is the system performance?
- How to improve the fidelity by calibration? -->

  <!-- - Major factor-1 (Getting a better control of microwaves): generating accurate microwave pulses (i.e., pulse amplitudes, frequenciees, durations).
  - Major factor-2 (Refresh): performing regular calibrations to compensate for system drift and external perturbations (hourly/daily intervals).
- Limitations of Prior Works: -->

  - *Limitations of Prior Works*: Existing calibration protocol does not consider the awareness of differences between physical qubits, even if it consider the trade-off between the calibration time and fidelity. This problem becomes severe when it comes to two-qubit gate operations (e.g., cross-resonance gates). Also, the calibration protocol is serialized.

    <!-- - (a) What happens in CR gate? An unwanted excitation in control qubit occurs due to off-resonant drives.
    - Q) What is off-resonant drives?
  - (2) The calibration protocol is serialized. -->
- *Insights to overcome the limitation*:

  - (1) Profiling qubit pairs and evaluate their responses. The standard derivative removal by adiabatic gate (DRAG) technique addresses this issue.

  - (2) Especially, multi-derivative DRQG offers a  solution by applying recursive corrections to suppress multiple transitions simulataneously. Graph traverse to calibrate quantum computer in parallel.

- *Limitation of this work*: 
<!-- Design: Three calibration policies
- (1) Brute-force clustering
- (2) Topology-oriented representative
- (3) Hardware-oriented policy -->
<!-- 
### Background - Calibration and Characterization in Quantum Gates

Operating CNOT is enabled by sophisticated control of pulses, which depends a tuning of "drive frequency", "amplitude", "phase", and "duration".

If they are not calibriated well, the error will be *accumulated*. Thus, the program fidelity will be degraded.

To optimize the calibration, *characterization* of quantum gates in physical device is crucial.

Method-1: Quantum Process Tomography (QPT) is an approach that constructs the entire quantum process matrix for a certain gate. This requires (1) quibt preparation in various input states, gate application, and measurement of output states to characterize the gate's behavior fully.

Method-2: Randomized Benchmarking (RB) is more efficient alternative for characterization. It determines the average gate error rates through random gate sequences applied to qubit.

Modern Methods: Leverage both QPT and RB.


### Echoed CR

Echoed Cross Resonance (Echoed CR) pulse is  one of the implementation method for CNOT. It is implemented with multiple Hamiltonian interactions: `ZX, ZZ, IZ, IX, IY` and `ZY`. The goal is to tune `ZX` well to rotate 90' precisely.

* [ ] Q) Why does ZX matter?

$$
\hat{H}(\Omega_{CR}, \Omega_T) = v_{ZX}\hat{Z}\hat{X} +...

$$ -->
<!-- 
- ZZ interaction requires IY DRAG calibration Why? -->

## 2. Correlated Decoding of Logical Algorithms with Transversal Gates (PRL 2024)
- *What is Problem?* MWPM decoder fails to decode when the measurement error occurs before performing transversal CNOT.
- *Why is it important?* MWPM decoder takes more rounds and this leads to lower threshold.
- *Limitation of Prior Work*: MWPM decoder assumes that single physical fault flips upto 2 checks, but transversal CNOT 
- *Insight* Correlated decoding can decode 3 flips with one syndrome extraction round. 
<!-- because correlated decoder can explain it with one fault. No extra syndrome rounds are required because the model already contains the correct single-fault explanation. -->
- *Limitation of This Work*: TBD.


 - Hyperedge: 

The logical cycle is typically defined as d syndrome rounds where the zero or two error events occur.
However, 

- Consider the transversal CNOT between two logical qubit.
## 2. ARTERY Fast Quantum Feedback using Branch Prediction

## 3. Constant-Rate Entanglement Distillation for Fast Quantum Interconnects

## 4. S-SYNC Shuttle and Swap Co-Optimization in Quantum Charge-Coupled Devices

## 5. Qtenon Towards Low-Latency Architecture Integration for Accelerating Hybrid Quantum-Classical Computing

## 6. Synchronization for Fault-Tolerant Quantum Computers

## 7. Variational Quantum Algorithms in the era of Early Fault

## 8. swiper_Minimizing Fault-Tolerant Quantum Program Latency via Speculative Window Decoding
