# BPSK Modulation and Demodulation Project

## Table of Contents
- [Project Overview](#project-overview)  
- [Why BPSK?](#why-bpsk)  
- [Mathematical Background](#mathematical-background)  
- [Project Work Methodology](#project-work-methodology)  
  - [Part A – Generating a BPSK Signal](#part-a--generating-a-bpsk-signal)  
  - [Part B – Demodulating BPSK Signal Using Product Detector](#part-b--demodulating-bpsk-signal-using-product-detector)  
  - [Part C – Restoring Data Using Comparator](#part-c--restoring-data-using-comparator)  
  - [Part D – Adding Noise to Transmitted Signal](#part-d--adding-noise-to-transmitted-signal)  
- [Simulation Results](#simulation-results)  
- [Conclusion](#conclusion)  
- [Files Included](#files-included)  

---

## Project Overview

This project demonstrates the simulation and hardware implementation of **Binary Phase Shift Keying (BPSK)** modulation and demodulation. BPSK is a simple digital modulation technique where the phase of a carrier signal is shifted between two states (0° and 180°) to represent binary data (0s and 1s).

---

## Why BPSK?

- BPSK is the simplest digital modulation method.  
- It uses only two phase states, making it highly resistant to noise.  
- It requires less power compared to more complex modulation schemes.  
- Commonly used in wireless communication, satellite links, and other digital communication systems.
<p align="center">
<img src="https://github.com/user-attachments/assets/4c7f903a-e913-413c-9e32-61add458918b" width="400">
</p>
---

## Mathematical Background

- **BPSK Modulation:** The carrier phase changes according to the binary input data.  
- **BPSK Demodulation:** The received modulated signal is multiplied with a synchronized reference carrier, filtered to recover the baseband signal, and then decoded to retrieve original binary data.

---

## Project Work Methodology

### Part A – Generating a BPSK Signal

- Designed the circuit and block diagrams for BPSK modulation.  
- Implemented the system on Emona board.  
- Observed the modulated signal output on a Pico-scope.
<p align="center">
  <table align="center">
    <tr>
      <td><img src="https://github.com/user-attachments/assets/661033c8-8208-4e20-a40c-825a1abbeaff" width="300"></td>
      <td><img src="https://github.com/user-attachments/assets/78b51c74-67eb-46e7-8025-670b61cbd326" width="300"></td>
    </tr>
  </table>
</p>
<p align="center">
<img src="https://github.com/user-attachments/assets/6d27cbb0-bcb8-4e92-9f4d-8b27a91e068e" width="400">
</p>

### Part B – Demodulating BPSK Signal Using Product Detector

- Built the product detector circuit for demodulation.  
- Tested and captured the demodulated output on the Pico-scope.

### Part C – Restoring Data Using Comparator

- Added a comparator circuit to restore the recovered binary data.  
- Verified output using hardware and Pico-scope.

### Part D – Adding Noise to Transmitted Signal

- Added noise of different levels (-20 dB, -6 dB, 0 dB) to the transmitted BPSK signal.  
- Observed the effect of noise on demodulation performance using Pico-scope.

---

## Simulation Results

- Simulink schematics for modulation and demodulation were created.  
- Compared hardware results with Simulink outputs.  
- Observed low pass filter outputs at modulation and demodulation stages.  
- Verified signal behavior under noisy conditions.

---

## Conclusion

This project successfully demonstrated the entire process of BPSK modulation and demodulation using both hardware and simulation. The results show how noise affects signal quality and how the design mitigates noise effects, ensuring reliable data recovery.

---
