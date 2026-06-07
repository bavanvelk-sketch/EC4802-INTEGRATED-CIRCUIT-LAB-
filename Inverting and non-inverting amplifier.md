# INVERTING AND NON-INVERTING AMPLIFIER USING OP-AMP (IC 741)

---

# 1. INVERTING AMPLIFIER

## AIM

To design an **Inverting Amplifier** using IC 741 for a gain of **−2**.

---

## APPARATUS REQUIRED

| S.No | Components                     | Specification |
| ---- | ------------------------------ | ------------- |
| 1    | Operational Amplifier          | IC 741        |
| 2    | Resistors                      | 1 kΩ, 2 kΩ    |
| 3    | Breadboard / Trainer Kit       | 1             |
| 4    | CRO (Cathode Ray Oscilloscope) | 1             |
| 5    | Function Generator             | 1             |
| 6    | Connecting Wires               | As Required   |

<img width="423" height="425" alt="image" src="https://github.com/user-attachments/assets/3674eb7b-218f-40aa-b61c-15f822d0bb16" />



## CIRCUIT DIAGRAM

<img width="561" height="386" alt="image" src="https://github.com/user-attachments/assets/ff091bd3-1a72-45d6-b099-78dd79944ca9" />


---

## PROCEDURE

1. Connect IC 741 on the trainer kit.
2. Give dual power supply (+VCC and −VCC) to the IC.
3. Make the circuit connections as per the circuit diagram.
4. Apply a sinusoidal input signal from the function generator to the inverting terminal.
5. Ground the non-inverting terminal.
6. Connect feedback resistor (R_f) between output and inverting terminal.
7. Switch ON the power supply and CRO.
8. Observe the input and output waveforms on the CRO.
9. Verify that the output waveform is amplified and 180° out of phase with the input.
10. Tabulate the readings.

---

## OBSERVATION TABLE

| S.No | Vin (V) | Vout (V) | Practical Gain | Theoretical Gain |
| ---- | ------- | -------- | -------------- | ---------------- |
| 1    | 0.2v    |  -2v     |   1 ms         | -2               |
| 2    | 0.4v    |  -4v     |   1 ms         | -2               |
| 3    | 0.6v    |  -6v     |   1 ms         | -2               |

---

## WAVEFORM

### Input Waveform

* Sinusoidal Signal

### Output Waveform

* Amplified Sinusoidal Signal
* 180° Phase Shift with respect to input
* <img width="431" height="443" alt="image" src="https://github.com/user-attachments/assets/60ad165b-c5e9-44e0-806f-ca85ee173fea" />


---

## RESULT

The working of the **Inverting Amplifier** was studied and verified successfully.

---

# 2. NON-INVERTING AMPLIFIER

## AIM

To design a **Non-Inverting Amplifier** using IC 741 for a gain of **2**.

---

## APPARATUS REQUIRED

| S.No | Components            | Specification |
| ---- | --------------------- | ------------- |
| 1    | Operational Amplifier | IC 741        |
| 2    | Resistors             | 1 kΩ, 2 kΩ    |
| 3    | Function Generator    | 1             |
| 4    | CRO                   | 1             |
| 5    | Dual Power Supply     | ±12 V         |
| 6    | Trainer Kit           | 1             |
| 7    | Connecting Wires      | As Required   |

---

<img width="574" height="306" alt="image" src="https://github.com/user-attachments/assets/abe9a5c9-afc4-4a63-aeaa-f93568ecd7b5" />


## CIRCUIT DIAGRAM
<img width="566" height="331" alt="image" src="https://github.com/user-attachments/assets/a46109b6-b41f-4162-aaa5-d0a8e0cef8ae" />


---

## PROCEDURE

1. Place IC 741 on the trainer kit.
2. Connect dual power supply ±12 V to the IC.
3. Make connections as per the circuit diagram.
4. Apply a sinusoidal input signal from the function generator to the non-inverting terminal.
5. Connect feedback resistor (R_f) and resistor (R_1) properly.
6. Switch ON the power supply and CRO.
7. Observe input and output waveforms on the CRO.
8. Measure input voltage, output voltage, time period and frequency.
9. Verify that the output waveform is amplified and in phase with the input waveform.
10. Tabulate the readings.

---

## OBSERVATION TABLE

| S.No | Vin (V) | Vout (V) | Practical Gain | Theoretical Gain |
| ---- | ------- | -------- | -------------- | ---------------- |
| 1    |   0.2v  |  2v      |  1ms           | 2                |
| 2    |   0.4v  |  4v      |  1ms           | 2                |
| 3    |   0.6v  |  6v      |  1ms           | 2                |

---

## WAVEFORM

### Input Waveform

* Sinusoidal Signal

### Output Waveform

* Amplified Sinusoidal Signal
* In Phase with Input Signal
*  <img width="638" height="574" alt="image" src="https://github.com/user-attachments/assets/ca89755b-ccce-4771-b0e7-bf65b9bb53b1" />


---

## RESULT

The **Non-Inverting Amplifier** was designed and verified successfully.

---

## CONCLUSION

Thus, the **Inverting Amplifier** and **Non-Inverting Amplifier** using **IC 741** were designed, implemented, and verified successfully. The measured gains closely matched the theoretical values, and the phase relationships between input and output waveforms were observed as expected.
