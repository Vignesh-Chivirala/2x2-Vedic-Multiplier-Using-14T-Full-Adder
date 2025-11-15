# **2×2 Vedic Multiplier Using 14T Full Adder**

This repository contains the design, implementation, and analysis of a **low-power, high-speed 2×2 Vedic Multiplier** based on the **Urdhva Tiryagbhyam** sutra of Vedic Mathematics. The multiplier internally uses an optimized **14-Transistor (14T) Full Adder**, designed to reduce transistor count, power consumption, and propagation delay, making it suitable for modern VLSI applications.

---
### 📦 Block Diagram of 2×2 Vedic Multiplier

![2×2 Vedic Multiplier Block Diagram](./Circuit_design_images/2X2 Vedic Multiplier using 14T Full Adder.png)


## **📌 Project Overview**

This project focuses on building an efficient arithmetic circuit using CMOS design principles.
The **2×2 Vedic Multiplier** is implemented using:

* The **Urdhva Tiryagbhyam algorithm** for parallel multiplication
* Optimized **14T Full Adders** for addition of partial products
* Circuit design and simulation using **DSCH 3.9** and layout implementation in **Microwind**

The design demonstrates advantages in terms of **speed**, **area**, and **power efficiency**, making it suitable for power-constrained digital systems.

---

## **🎯 Objectives**

* Design a high-speed **2×2 Vedic Multiplier** using Vedic mathematics.
* Implement a **14T Full Adder** to minimize transistor usage and power.
* Simulate and verify functionality using **DSCH 3.9**.
* Analyze **power, delay, and efficiency** of the proposed design.
* Establish a foundation for scaling to **higher-order multipliers** (4×4, 8×8, etc.).

---

## **📐 Design Components**

### **🔹 14T Full Adder**

* Implemented using a combination of **pass-transistor logic** and **transmission gates**.
* Produces SUM and COUT outputs with reduced delay.
* Uses fewer transistors compared to 28T and traditional full adders.
* Verified through simulations and waveform analysis.

### **🔹 2×2 Vedic Multiplier Architecture**

Inputs:

* **A = A1 A0**
* **B = B1 B0**

Outputs:

* **4-bit product: S3 S2 S1 S0**

Working Principle (Urdhva Tiryagbhyam):

1. Vertical multiplication for **S0 = A0B0**
2. Crosswise multiplication + Full Adder for **S1**
3. Vertical + carry addition using Full Adder for **S2 and S3**

This enables **parallel processing**, reducing computation time significantly compared to conventional multipliers.

---

## **📊 Performance Comparison**

| Full Adder Type | Power (µW) | Delay (ns) |
| --------------- | ---------- | ---------- |
| **11T**         | 2.10       | 24.5       |
| **14T**         | 2.45       | **18.0**   |
| 28T             | 3.85       | 26.0       |
| General         | 4.10       | 28.5       |

🔸 **14T Full Adder provides the best balance of power, speed, and stability.**
🔸 The proposed multiplier outperforms other variants in efficiency.

---

## **🖥️ Tools & Technologies Used**

* **DSCH 3.9** – Schematic design & simulation
* **Microwind** – Layout design
* **CMOS Logic Design**
* **Vedic Mathematics (Urdhva Tiryagbhyam)**

---

## **📷 Included Work**

The project includes:

* 14T Full Adder schematic, layout, and waveforms
* 2×2 Vedic Multiplier schematic and simulation results
* 11T Full Adder comparison implementation
* 4-bit Ripple Carry Adder using 14T FA
* 4×4 Vedic Multiplier layout

---

## **📝 Conclusion**

The proposed **2×2 Vedic Multiplier using 14T Full Adder** shows significant improvements in:

* **Speed**
* **Power efficiency**
* **Circuit compactness**

The architecture demonstrates how optimized transistor-level designs can improve arithmetic circuit performance, making them ideal for **low-power VLSI systems**, DSP processors, and embedded applications.

---

## **🚀 Future Work**

* Extend the design to **4×4, 8×8, and 16×16 Vedic Multipliers**.
* Perform transistor-level optimization in:

  * Microwind
  * Tanner EDA
  * Synopsys/Cadence tools
* Implement advanced low-power techniques:

  * Supply voltage scaling
  * Transistor sizing
  * Hybrid logics (GDI, PTL)
* FPGA or ASIC implementation for real-time testing and timing analysis.

---

## **📚 References**

Included in the original project report.
