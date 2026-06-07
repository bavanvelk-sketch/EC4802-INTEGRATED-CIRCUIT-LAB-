# OCTAL TO BINARY ENCODER

## AIM

To realise and verify the truth table of octal to binary encoder using IC 74148 digital IC.

---

## APPARATUS REQUIRED

| S.No | Name of the Equipment | Specification | No. of Quantity |
|-------|----------------------|--------------|-----------------|
| 1 | 8×3 Encoder | IC 74148 | 1 |
| 2 | Trainer Kit | - | 1 |
| 3 | Connecting Wires | - | As Required |


---

## PIN CONFIGURATION

**Fig. 1**

<img width="495" height="433" alt="image" src="https://github.com/user-attachments/assets/ca3c5bd1-a695-4b66-abc8-70a3c2a8389f" />

## Function Table
<img width="631" height="341" alt="image" src="https://github.com/user-attachments/assets/44c80cbb-f13a-41ee-afbb-47da8ef1716a" />

## Logic Diagram
<img width="524" height="530" alt="image" src="https://github.com/user-attachments/assets/bd271c53-bfa5-4a17-b606-72d1a844791f" />


---

## THEORY

An encoder is a digital circuit that performs the reverse operation of a decoder. An encoder has \(2^n\) input lines and **n** output lines that generate the corresponding binary code.

The encoder is generally constructed using OR gates.

The encoder assumes that only one input line can be equal to 1 at any given time; otherwise, the output becomes ambiguous. The circuit has 8 inputs and can have \(2^8 = 256\) possible input combinations. Only 8 of these combinations are valid, while the remaining combinations are considered "don't care" conditions.

The encoder available in IC form is called a **Priority Encoder**. The IC 74148 is an **8-to-3 priority encoder** with:

- Active LOW inputs
- Active LOW outputs
- Enable input
- Carry output

These features allow cascading of multiple encoder circuits to handle a larger number of inputs.

---

## PROCEDURE

1. Make the connections as shown in the pin configuration diagram.
2. Apply inputs according to the truth table.
3. Observe the corresponding outputs.
4. Verify the output binary code for each input condition.
5. Record the observations.

---

## RESULT

Thus, the truth table of the octal-to-binary encoder was realised and verified using IC 74148.
