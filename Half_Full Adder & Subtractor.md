# HALF/FULL ADDER & HALF/FULL SUBTRACTOR

## AIM

To realize:

### Using X-OR and Basic Gates

* Half Adder
* Full Adder
* Half Subtractor
* Full Subtractor

### Using NAND Gates Only

* Half Adder
* Full Adder
* Half Subtractor
* Full Subtractor

---

## APPARATUS REQUIRED

* Digital Trainer Kit
* IC 7486 (X-OR Gate)
* IC 7432 (OR Gate)
* IC 7408 (AND Gate)
* IC 7400 (NAND Gate)
* Connecting Wires

---

## THEORY

### Half Adder

A Half Adder is a combinational circuit that performs the addition of two binary digits.

#### Outputs

* Sum (S)
* Carry (C)

#### Boolean Expressions

[
S = A \oplus B
]

[
C = A \cdot B
]

---

### Full Adder

A Full Adder adds three binary inputs:

* A
* B
* Carry Input ((C_{n-1}))

#### Outputs

* Sum (S)
* Carry (C)

#### Boolean Expressions

[
S = A \oplus B \oplus C_{n-1}
]

[
C = AB + BC_{n-1} + AC_{n-1}
]

---

### Half Subtractor

A Half Subtractor performs subtraction of two binary digits.

#### Outputs

* Difference (D)
* Borrow (B)

#### Boolean Expressions

[
D = A \oplus B
]

[
Borrow = \overline{A}B
]

---

### Full Subtractor

A Full Subtractor subtracts:

* B
* Borrow Input ((C_{n-1}))

from A.

#### Outputs

* Difference (D)
* Borrow (B)

#### Boolean Expressions

[
D = A \oplus B \oplus C_{n-1}
]

[
Borrow = \overline{A}B + \overline{A}C_{n-1} + BC_{n-1}
]

---

## CIRCUIT DIAGRAMS

### Using Basic Gates

#### Half Adder

<img width="438" height="204" alt="image" src="https://github.com/user-attachments/assets/107eca6f-aa44-42aa-ac5b-154f75ce3919" />
#### Full Adder
<img width="780" height="267" alt="image" src="https://github.com/user-attachments/assets/e4e4a060-9914-4654-9659-1ace9219c79a" />

---

### Using NAND Gates Only

#### Half Adder

<img width="780" height="250" alt="image" src="https://github.com/user-attachments/assets/d74c3eaf-f6e8-48bf-acb9-11144338f644" />


#### Full Adder
<img width="780" height="215" alt="image" src="https://github.com/user-attachments/assets/55266553-a19f-4343-a4ff-2762664f03ec" />



#### Half Subtractor

<img width="780" height="259" alt="image" src="https://github.com/user-attachments/assets/435cceb8-b68a-4cd3-a0ef-b5078f3c9b24" />


#### Full Subtractor

<img width="780" height="217" alt="image" src="https://github.com/user-attachments/assets/38e8a098-3bea-457e-a91d-4c3737eb0596" />


---

## PROCEDURE

1. Verify the working of all required logic gates.
2. Make the connections according to the circuit diagram.
3. Switch ON the power supply (VCC).
4. Apply various combinations of inputs according to the truth table.
5. Observe and record the outputs.
6. Verify the Sum/Difference and Carry/Borrow outputs.
7. Compare the observed outputs with the theoretical truth table.

---

# TRUTH TABLES

## Half Adder

| A | B | S | C | S(V) | C(V) |
| - | - | - | - | ---- | ---- |
| 0 | 0 | 0 | 0 |  0   |  0   |
| 0 | 1 | 1 | 0 |  1   |  0   |
| 1 | 0 | 1 | 0 |  1   |   0  |
| 1 | 1 | 0 | 1 |  0   |   0  |

---

## Full Adder

| A | B | Cn-1 | S | C | S(V) | C(V) |
| - | - | ---- | - | - | ---- | ---- |
| 0 | 0 | 0    | 0 | 0 |  0   |  0   |
| 0 | 0 | 1    | 1 | 0 |  1   |  0   |
| 0 | 1 | 0    | 1 | 0 |  1   |  0   |
| 0 | 1 | 1    | 0 | 1 |  0   |  1   |
| 1 | 0 | 0    | 1 | 0 |  1   |  0   |
| 1 | 0 | 1    | 0 | 1 |  0   |  1   |
| 1 | 1 | 0    | 0 | 1 |  0   |  1   |
| 1 | 1 | 1    | 1 | 1 |  1   |  1   |

---

## Half Subtractor

| A | B | D | Borrow | D(V) | B(V) |
| - | - | - | ------ | ---- | ---- |
| 0 | 0 | 0 | 0      | 0    |  0   |
| 0 | 1 | 1 | 1      | 1    |  1   |
| 1 | 0 | 1 | 0      | 1    |  0   |
| 1 | 1 | 0 | 0      | 0    |  0   |

---

## Full Subtractor

| A | B | Cn-1 | D | Borrow | D(V)  | B(V) |
| - | - | ---- | - | ------ | ----  | ---- |
| 0 | 0 | 0    | 0 | 0      |  0    |  0   |
| 0 | 0 | 1    | 1 | 1      |  1    |  1   |
| 0 | 1 | 0    | 1 | 1      |  1    |  1   |
| 0 | 1 | 1    | 0 | 1      |  0    |  1   |
| 1 | 0 | 0    | 1 | 0      |  1    |  0   |
| 1 | 0 | 1    | 0 | 0      |  0    |  0   |
| 1 | 1 | 0    | 0 | 0      |  0    |  0   |
| 1 | 1 | 1    | 1 | 1      |  0    |  1   |

---

## OBSERVATION

* The output Sum and Carry for Half Adder and Full Adder were observed and verified.
* The output Difference and Borrow for Half Subtractor and Full Subtractor were observed and verified.
* The outputs obtained matched the corresponding truth tables.

---

## CONCLUSION

Thus, the **Half Adder, Full Adder, Half Subtractor, and Full Subtractor** were successfully realized using:

* XOR and Basic Gates
* NAND Gates Only

and their truth tables were verified successfully.
