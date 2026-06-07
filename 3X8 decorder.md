# 3×8 DECODER USING IC 74138

## AIM

To construct and verify a 3×8 Decoder using IC 74138.

---

## APPARATUS REQUIRED

* IC 74138 (3×8 Decoder)
* Digital Trainer Kit / Breadboard
* Connecting Wires
* Power Supply (+5V)

---

## THEORY

Discrete quantities of information are represented in digital systems using binary codes.

A binary code of **n bits** can represent **2ⁿ** distinct information combinations. A **decoder** is a combinational circuit that converts binary information from **n input lines** to a maximum of **2ⁿ output lines**.

These circuits are known as **n-to-m line decoders**, where:

* `n` = Number of input lines
* `m` = Number of output lines
* `m ≤ 2ⁿ`

The primary purpose of a decoder is to generate the **minterms** of the input variables.

A **3×8 Decoder** has:

* 3 input lines
* 8 output lines

Each output corresponds to one minterm of the three input variables.

### Applications

* Binary-to-Octal Conversion
* Memory Address Decoding
* Data Routing
* Code Conversion
* Digital Control Systems

The IC 74138 is a high-speed 3-to-8 line decoder/demultiplexer with active LOW outputs.

---

## IC USED

### IC 74138

* Type: 3-to-8 Line Decoder
* Number of Inputs: 3
* Number of Outputs: 8
* Active LOW Outputs

---

## PIN DIAGRAM (IC 74138)

<img width="379" height="265" alt="image" src="https://github.com/user-attachments/assets/c22b9294-c445-4463-b144-0e82a938cabd" />

### Important Pins

| Pin   | Function                   |
| ----- | -------------------------- |
| A     | Input A (LSB)              |
| B     | Input B                    |
| C     | Input C (MSB)              |
| G1    | Enable Input (Active HIGH) |
| G2A   | Enable Input (Active LOW)  |
| G2B   | Enable Input (Active LOW)  |
| Y0–Y7 | Outputs                    |
| VCC   | +5V Supply                 |
| GND   | Ground                     |

---

## CIRCUIT DIAGRAM

<img width="679" height="815" alt="image" src="https://github.com/user-attachments/assets/5c85ac80-4aa9-4436-8cb4-22eb29c75012" />


### Connections

* Connect VCC to +5V.
* Connect GND to Ground.
* Enable the decoder using:

  * G1 = HIGH
  * G2A = LOW
  * G2B = LOW
* Apply inputs to pins A, B, and C.
* Observe outputs Y0 to Y7.

---

## FUNCTION TABLE

<img width="883" height="647" alt="image" src="https://github.com/user-attachments/assets/287237df-e6bb-48b9-9df1-701b9b941cb2" />


> Note: Outputs of IC 74138 are active LOW. The selected output becomes LOW while all other outputs remain HIGH.

---

## PROCEDURE

1. Place IC 74138 on the breadboard/trainer kit.
2. Connect the power supply:

   * VCC → +5V
   * GND → Ground
3. Enable the decoder:

   * G1 = HIGH
   * G2A = LOW
   * G2B = LOW
4. Apply input combinations to A, B, and C.
5. Observe the outputs Y0 to Y7.
6. Verify that only one output becomes LOW for each input combination.
7. Record the observations in the function table.

---

## OBSERVATION

For every binary input combination applied to A, B, and C, the corresponding output line becomes active (LOW), while all other outputs remain inactive (HIGH).

---

## RESULT

Thus, the **3×8 Decoder** was successfully constructed and verified using **IC 74138**.
