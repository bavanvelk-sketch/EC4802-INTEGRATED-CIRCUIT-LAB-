# MONOSTABLE AND ASTABLE MULTIVIBRATOR USING 555 TIMER

## AIM

To design and verify **Monostable** and **Astable Multivibrators** using the **NE555 Timer IC**.

---

## APPARATUS REQUIRED

| S.No | Equipment                | Specification   | Quantity |
| ---- | ------------------------ | --------------- | -------- |
| 1    | NE555 Timer IC           | NE555           | 1        |
| 2    | Resistors                | 10 kΩ           | 1        |
| 3    | Resistors                | 3.5 kΩ, 6.8 kΩ  | 1 each   |
| 4    | Capacitors               | 0.1 µF, 0.01 µF | 1 each   |
| 5    | CRO                      | 20 MHz          | 1        |
| 6    | AFO (Function Generator) | 2 MHz           | 1        |
| 7    | Regulated Power Supply   | 0–30 V, 0–2 A   | 1        |
| 8    | Trainer Kit              | Digital Trainer | 1        |
| 9    | Connecting Wires         | As Required     | -        |

---

## SPECIFICATIONS OF NE555 TIMER

* Maximum Supply Voltage = **18 V**
* Maximum Power Dissipation = **600 mW**

---

# DESIGN

## ASTABLE MULTIVIBRATOR
Vc = Vcc (1-e –t/RC)
The time taken by the circuit to change from 0 to 2/3 Vcc  is

              2/3 Vcc =Vcc(1-e–t/RC)
                     t1= 1.09 C;
 The time taken circuit to charge from 0 to 1/3 Vcc 
                1/3 Vcc= Vcc(1-e–t2/RC)
The time taken to charge from 1/3 Vcc to 2/3 Vcc is
                  ton = t1-t2
                  ton =0.69 RC;
                   R = RA+RB
                  ton =0.69(RA+RB)
 The time taken by the capacitor to discharge from 2/3 Vcc to 1/3 Vcc is         
                 toff=0.69RBC
Duty cycle, D= ton/(ton+toff)
Frequency  f = 1/т = 1/(ton+ toff)
Let              f =1 kHz; T = 1 ms;
For 75% duty cycle , 
               ton = 0.75ms;
               toff = 0.25ms;
               toff = 0.69 RBC;
let C = 0.1 µf;
               RB= 3.623*103 Ω
RB is selected as 3.5kΩ
             ton = 0.69(Ra+Rb)C
             RA = 7.246kΩ
RA is selected as 6.8kΩ     
       R is approximately taken as 10kΩ

MONOSTABLE MULTIVIBRATOR:
         
 The voltage across the capacitor is given by,
                                       Vc = Vcc  [1- e-t/RC]
Let t = T,  Vc =2/3 Vcc
       Tc =Rc ln
       T  =1.1Rc ms
       f   = 500 Hz ; T=1/f = 2 ms
       C = 0.1µf≤ duty cycle = 50%
       Ton =Toff =1 ms
       R=T/1.1 C = 10-3/1.1*10-6*0.1
       R= 9.09 kΩ
       R is approximately taken as 10kΩ

## 555 TIMER PIN DIAGRAM

<img width="413" height="238" alt="image" src="https://github.com/user-attachments/assets/84714c55-77ea-42b9-9e65-ab0b28fe11c4" />


### Pin Description

| Pin No | Name            | Function             |
| ------ | --------------- | -------------------- |
| 1      | Ground          | Ground Reference     |
| 2      | Trigger         | Starts Timing Cycle  |
| 3      | Output          | Output Signal        |
| 4      | Reset           | Resets Timer         |
| 5      | Control Voltage | Threshold Control    |
| 6      | Threshold       | Ends Timing Cycle    |
| 7      | Discharge       | Discharges Capacitor |
| 8      | VCC             | Positive Supply      |

---

## FUNCTIONAL DIAGRAM

<img width="390" height="382" alt="image" src="https://github.com/user-attachments/assets/3553a208-0d29-4467-9ca4-c2ab7e308f4c" />


---

# CIRCUIT DIAGRAMS

## Astable Multivibrator

<img width="452" height="356" alt="image" src="https://github.com/user-attachments/assets/b3a66944-9d48-48cf-8824-91faa80501da" />

---

## Monostable Multivibrator

<img width="474" height="352" alt="image" src="https://github.com/user-attachments/assets/82e04805-2898-4737-a444-60df7007d2ab" />

---
# Procedure:
MONOSTABLE MULTIVIBRATOR:
          
                The circuit connections are made as shown in the circuit diagram. AFO input of desired frequency is given to input pin of 555 timer. The Multivibrator output of the required period is seen in CRO connected to output pin of 555 timer.
        The capacitor voltage waveform is also seen in CRO by connecting to pin 6. The magnitude of the waveform and time period of the wave form are noted 

ASTABLE MULTIVIBRATOR:

The circuit connections are made as shown in the figure. The case of astable multivibrator there is no need for triggering input; hence pins 2 and 6 are shorted. Based on he required duty cycle values resistance and capacitor are designed. The output of the astable multivibrator is seen in CRO. The magnitude and the time period of the waveforms are also noted.
 


# THEORY

## 555 AS MONOSTABLE MULTIVIBRATOR:

This circuit diagram shows how a 555 timer IC is configured to function as a basic monostable multivibrator.  A monostable multivibrator is a timing circuit that changes state once triggered, but returns to its original state after a certain time delay.  It got its name from the fact that only one of its output states is stable.  It is also known as a 'one-shot'. 
    
In this circuit, a negative pulse applied at pin 2 triggers an internal flip-flop that turns off pin 7's discharge transistor, allowing C1 to charge up through R1. At the same time, the flip-flop brings the output (pin 3) level to 'high'.  When capacitor C1 as charged up to about 2/3 Vcc, the flip-flop is triggered once again, this time making the pin 3 output 'low' and turning on pin 7's discharge transistor, which discharges C1 to ground. This circuit, in effect, produces a pulse at pin 3 whose width t is just the product of R1 and C1, i.e., t=R1C1.
    
The reset pin, which may be used to reset the timing cycle by pulling it momentarily low, should be tied to the Vcc if it will not be used.   

## Working:

1. A negative trigger pulse is applied to Pin 2.
2. The internal flip-flop is set.
3. Output at Pin 3 goes HIGH.
4. Capacitor begins charging through resistor R.
5. When capacitor voltage reaches 2/3 VCC, the threshold comparator resets the flip-flop.
6. Output returns LOW.
7. Capacitor discharges through Pin 7.


## 555 AS ASTABLE MULTIVIBRATOR
This circuit diagram shows how a 555 timer IC is configured to function as an astable multivibrator.  An astable multivibrator is a timing circuit whose 'low' and 'high' states are both unstable.  As such, the output of an astable multivibrator toggles between 'low' and 'high' continuously, in effect generating a train of pulses. This circuit is therefore also known as a 'pulse generator' circuit.
    
In this circuit, capacitor C1 charges through R1 and R2, eventually building up enough voltage to trigger an internal comparator to toggle the output flip-flop.  Once toggled, the flip-flop discharges C1 through R2 into pin 7, which is the discharge pin.  When C1's voltage becomes low enough, another internal comparator is triggered to toggle the output flip-flop. This once again allows C1 to charge up through R1 and R2 and the cycle starts all over again.
      
C1's charge-up time t1 is given by: t1 = 0.693(R1+R2)C1. C1's discharge time t2 is given by: t2 = 0.693(R2)C1.  Thus, the total period of one cycle is t1+t2 = 0.693 C1(R1+2R2).  The frequency f of the output wave is the reciprocal of this period, and is therefore given by: f = 1.44/(C1(R1+2R2)), wherein f is in Hz if R1 and R2 are in megaohms and C1 is in microfarads.   

### Working

1. Capacitor charges through RA and RB.
2. When capacitor voltage reaches 2/3 VCC, output changes state.
3. Capacitor discharges through RB and Pin 7.
4. When voltage drops to 1/3 VCC, output changes state again.
5. The cycle repeats continuously.

## MONOSTABLE MULTIVIBRATOR

1. Make the circuit connections as per the circuit diagram.
2. Apply trigger pulse from AFO to Pin 2.
3. Connect CRO to output Pin 3.
4. Observe the output pulse waveform.
5. Observe capacitor voltage waveform at Pin 6.
6. Measure pulse width and amplitude.
7. Compare measured value with theoretical value.

---

## ASTABLE MULTIVIBRATOR

1. Make circuit connections as shown in the circuit diagram.
2. Short Pins 2 and 6.
3. Connect timing components RA, RB and C.
4. Switch ON the power supply.
5. Observe the output waveform on CRO.
6. Measure frequency and time period.
7. Verify duty cycle and frequency using calculated values.

---

# WAVEFORMS

## Monostable Multivibrator

<img width="551" height="160" alt="image" src="https://github.com/user-attachments/assets/40c157bf-6975-4140-9994-2b361ec50410" />

---

## Astable Multivibrator
<img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/528351e0-9583-43ec-b236-9cfc5a5ca4c1" />


---

# RESULT

Thus, the **Monostable Multivibrator** and **Astable Multivibrator** were designed and verified successfully using the **NE555 Timer IC**. The practical frequency and pulse width closely matched the theoretical values, and the corresponding waveforms were observed on the CRO.
