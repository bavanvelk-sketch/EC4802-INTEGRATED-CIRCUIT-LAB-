# INTEGRATOR AND DIFFERENTIATOR USING OP-AMP

## AIM

To design and set up an integrator and differentiator circuit using an operational amplifier (Op-Amp).

---

## APPARATUS REQUIRED

- Power Supply
- CRO (Cathode Ray Oscilloscope)
- Function Generator
- Breadboard
- Op-Amp
- Capacitors
- Resistors
- Connecting Wires

---

## THEORY

### Integrator

The integrator circuit performs mathematical integration of the input signal.

The output voltage is given by:

\[
V_o = -\frac{1}{RC}\int V_i\,dt + k
\]

where:

- \(V_o\) = Output voltage
- \(V_i\) = Input voltage
- \(R\) = Resistance
- \(C\) = Capacitance
- \(k\) = Constant of integration

The peak output voltage is:

\[
V_T = \frac{V_iT}{4RC}
\]

where:

- \(T\) = Time period of the input square wave

#### Applications

- Analog computers
- Wave shaping circuits
- Signal processing systems

---

### Differentiator

A differentiator is obtained by replacing the input resistor of an inverting amplifier with a capacitor.

The output voltage is:

\[
V_o = -R_F C_i \frac{dV_i}{dt}
\]

where:

- \(R_F\) = Feedback resistance
- \(C_i\) = Input capacitance

#### Characteristics

- Acts as a High Pass Filter
- Gain increases with frequency
- Susceptible to high-frequency noise
- May become unstable at high frequencies

Additional circuit elements can be used to improve stability and reduce noise.

---

## DESIGN AND CIRCUIT DIAGRAMS

### Design of Integrator

Given:

- Input Frequency = 1 kHz
- Capacitance, \(C = 0.01 \mu F\)

The unity gain frequency is:

\[
f = \frac{1}{2\pi R_1 C}
\]

Calculating:

\[
R_1 = 15.9\,k\Omega
\]

Standard value used:

- \(R_1 = 15\,k\Omega\)

Feedback resistor:

- \(R_2 = 470\,k\Omega\)

#### Purpose of \(R_2\)

- Reduces low-frequency gain
- Minimizes effects of DC offset voltage
- Typically selected as 10 times or more than \(R_1\)

---

### Design of Differentiator

Given:

- Frequency = 1 kHz
- Capacitance \(C = 0.01 \mu F\)

Using:

\[
f = \frac{1}{2\pi RC}
\]

Calculating:

\[
R = 15.9\,k\Omega
\]

Standard value used:

- \(R = 15\,k\Omega\)

---

## CIRCUIT DIAGRAMS

### Figure 1: Integrator Circuit
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/d83a10ad-2401-470d-ab67-d2c06c5489c3" />

- Input resistor \(R_1 = 15\,k\Omega\)
- Feedback capacitor \(C = 0.01 \mu F\)
- Feedback resistor \(R_2 = 470\,k\Omega\)

### Figure 2: Differentiator Circuit
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/4232d4da-f57b-4fed-9037-9beaae96fbd9" />


- Input capacitor \(C = 0.01 \mu F\)
- Feedback resistor \(R = 15\,k\Omega\)

---

## PROCEDURE

### Integrator

1. Set up the integrator circuit as shown in the circuit diagram.
2. Apply a square wave input of:
   - Amplitude: ±5 V (10 Vpp)
   - Frequency: 1 kHz
3. Observe both input and output waveforms simultaneously on the CRO.
4. Vary the DC offset of the square wave input and observe the changes in the output waveform.
5. Apply a triangular wave input and observe the output waveform.
6. Apply a sine wave input and observe the output waveform.
7. Record all observations.

---

### Differentiator

1. Set up the differentiator circuit as shown in the circuit diagram.
2. Apply a square wave input of:
   - Amplitude: ±5 V (10 Vpp)
   - Frequency: 1 kHz
3. Observe both input and output waveforms simultaneously on the CRO.
4. Apply a triangular wave input and observe the output waveform.
5. Apply a sine wave input and observe the output waveform.
6. Record all observations.

---

## WAVEFORMS

### Integrator Output
<img width="572" height="286" alt="image" src="https://github.com/user-attachments/assets/945e6716-486c-42e3-9ae0-ef74cc65cee8" />




**Input:** Square Wave

**Output:** Triangular Wave

*(Refer Figure 3)*

---

### Differentiator Output
<img width="226" height="173" alt="image" src="https://github.com/user-attachments/assets/e22c9e29-181a-48db-a0ee-0da0e4aa072f" />



**Input:** Square Wave

**Output:** Positive and Negative Spikes

*(Refer Figure 4)*

---

## OBSERVATIONS

### Integrator

| Input Waveform | Output Waveform |
|---------------|----------------|
| Square Wave | Triangular Wave |
| Triangular Wave | Parabolic Wave |
| Sine Wave | Cosine Wave |

---

### Differentiator

| Input Waveform | Output Waveform |
|---------------|----------------|
| Square Wave | Positive and Negative Spikes |
| Triangular Wave | Square Wave |
| Sine Wave | Cosine Wave |

---

## RESULT

- The Op-Amp Integrator circuit was designed and tested successfully.
- The Op-Amp Differentiator circuit was designed and tested successfully.
- The expected output waveforms were observed for various input waveforms.

---
