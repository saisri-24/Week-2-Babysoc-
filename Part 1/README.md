# BabySoC: A Compact Open-Source SoC with DAC and PLL  

## Introduction  
A **System-on-Chip (SoC)** is a complete computing system built on a single chip. Instead of having separate processors, memory, and peripherals, an SoC integrates all these elements into one compact package. This makes devices like smartphones, smartwatches, and IoT gadgets both **powerful and energy-efficient**.  

This project explores **BabySoC**, a simplified, open-source SoC based on the **RVMYTH RISC-V processor core**. BabySoC integrates:  
- A **Phase-Locked Loop (PLL)** for stable clock generation.  
- A **10-bit Digital-to-Analog Converter (DAC)** for interfacing with analog devices.  

By combining these features, BabySoC can process digital data and generate **real-world analog outputs** such as audio and video, making it a perfect educational platform for students and researchers.  

---

## What is a System-on-Chip (SoC)?  
A **System-on-Chip** is like a full computer inside a single chip. It brings together processing, memory, input/output, and communication into one small unit.  

### Benefits of SoCs  
- **Space Saving:** Smaller devices like smartphones and wearables.  
- **Power Efficient:** Longer battery life.  
- **High Performance:** Faster processing due to tight integration.  
- **Cost-Effective:** Fewer components reduce overall cost.  
- **Reliable:** Fewer interconnections mean fewer points of failure.  

---

## Components of a Typical SoC  
1. **CPU (Central Processing Unit):** Executes instructions and runs programs.  
2. **Memory:**  
   - **RAM** for temporary storage.  
   - **ROM/Flash** for permanent storage.  
3. **Peripherals:** Interfaces like USB, HDMI, audio, Wi-Fi, and Bluetooth.  
4. **Interconnect (Bus System):** Connects CPU, memory, and peripherals for smooth data transfer.  

Examples: Apple A-series (iPhones), Qualcomm Snapdragon (Android), and NVIDIA Tegra (Nintendo Switch).  

---

## Why BabySoC is a Simplified Model  
Unlike complex commercial SoCs, BabySoC is intentionally **minimal** and **educational**:  
- Uses **RVMYTH** (a simple RISC-V CPU) for processing.  
- Includes a **PLL** for generating stable clock signals.  
- Features a **10-bit DAC** to demonstrate digital-to-analog conversion.  
- Designed as **open-source**, allowing students to learn SoC design hands-on.  

This simplification makes it easier to understand SoC fundamentals while still showing how digital systems interact with the analog world.  

---

## BabySoC Architecture and Workflow  
1. **Initialization & Clocking:** The PLL generates a stable and synchronized clock signal.  
2. **Processing (RVMYTH):** The CPU cycles through registers, preparing values for output.  
3. **Analog Output (DAC):** The DAC converts binary data into analog signals that can drive external devices like speakers or displays.  

This workflow highlights the **bridge between digital data and real-world signals**, a key concept in SoC learning.  

---

## Phase-Locked Loop (PLL)  
- A **PLL** locks the output frequency to match an input reference.  
- **Main Components:**  
  - Phase Detector  
  - Loop Filter  
  - Voltage-Controlled Oscillator (VCO)  
- **Why needed:** Off-chip clocks suffer from jitter, delay, and frequency drift. On-chip PLLs provide **stable, precise, and tunable clock signals**.  

---

## Digital-to-Analog Converter (DAC)  
- A **DAC** converts binary numbers into continuous analog signals.  
- **Types:**  
  - Weighted Resistor DAC  
  - R-2R Ladder DAC  
- **BabySoC’s 10-bit DAC:** Can represent 1024 levels, making it useful for audio/video signal generation.  

---

## Role of Functional Modelling in SoC Design  
Before RTL and physical design stages, SoC projects use **functional models** to validate design intent.  

- **What it does:** Describes system behavior without worrying about hardware implementation.  
- **Benefits:**  
  - Ensures correct functionality early.  
  - Provides a **golden reference** for RTL verification.  
  - Saves **time and cost** by catching errors before physical design.  
  - Helps explore **design trade-offs** like clock speed, memory size, and interconnects.  

Functional modelling is like the **blueprint stage** of SoC design—it confirms correctness before moving to expensive implementation stages.  

---

## Conclusion  
The **BabySoC project** shows how open-source hardware can be both **educational and practical**. With a lightweight RISC-V CPU, a PLL for precise clocking, and a 10-bit DAC for analog interfacing, BabySoC is an excellent platform for learning the fundamentals of SoC design.  

By simplifying the complexity of commercial SoCs, BabySoC makes it easier for students and researchers to:  
- Understand the **core components of an SoC**.  
- Explore the **digital-to-analog interface**.  
- Gain hands-on experience in SoC design flows.  

Built on **Sky130 technology**, BabySoC represents a bridge between **academic learning** and **real-world applications**, making it a valuable tool for the next generation of chip designers.  

---

