# Digital System Design Mini Project
## 4-Bit Decimal Counter with 7-Segment Display

This project implements a **4-bit decimal counter** that counts from 00 to 15 and displays the output on two **7-segment displays**. It was developed as part of the Digital System Design course to reinforce concepts such as synchronous counters, binary-to-BCD conversion, and display interfacing.

---

## 🧠 Objective

To design and build a hardware-based system that:
- Counts from 0 to 15 in decimal.
- Uses standard logic ICs to perform binary counting and conversion.
- Displays the real-time count on a pair of 7-segment displays.

---

## 🔧 Components Used

| Component         | Quantity | Description                          |
|------------------|----------|--------------------------------------|
| NE555 Timer IC   | 1        | Clock signal generator               |
| 74LS163          | 1        | 4-bit synchronous binary counter     |
| 74LS85           | 1        | Magnitude comparator (>9 detection)  |
| 74LS83           | 1        | 4-bit binary full adder              |
| 74LS47           | 2        | BCD to 7-segment decoder/driver      |
| 7-Segment Display| 2        | Common cathode displays              |
| Resistors & Wires| -        | For connections & LED protection     |
| Breadboard       | 1        | Prototyping platform                 |
| Power Supply     | 1        | 5V DC                                |

---

## ⚙️ Working Principle

1. **Clock Generation**: NE555 generates clock pulses at a regular interval.
2. **Counting Logic**: 74LS163 counts in binary from 0000 to 1111 (0–15).
3. **Magnitude Comparison**: 74LS85 checks if the count exceeds 9.
4. **BCD Correction**: If the count is >9, 74LS83 adds 6 to correct binary to BCD.
5. **Display Driver**: 74LS47 decodes BCD into 7-segment control signals.
6. **Output Display**: Two 7-segment displays show the final BCD count (00 to 15).

---

## 🎯 Output

<img src="https://github.com/RKS200/4-Bit-Counter/blob/main/vlcsnap-2025-05-06-17h04m33s710.png" width="480">

The system displays a continuous loop from 00 to 15 in decimal, accurately and clearly using 7-segment displays. The transition is smooth with clean display timing thanks to the stable clock input.

---

## 🧪 Learnings

- IC-level implementation of synchronous digital systems.
- Practical challenges in clock synchronization and signal propagation.
- Binary to BCD conversion using adders and comparators.
- Debugging and validating real-time hardware behavior.

---

