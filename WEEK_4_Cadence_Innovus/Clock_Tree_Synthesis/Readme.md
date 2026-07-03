# 🌳 Clock Tree Synthesis (CTS) in Cadence Innovus

## 📖 What is Clock Tree Synthesis?

Clock Tree Synthesis (CTS) is a critical stage in the **ASIC Physical Design Flow** that constructs a balanced clock distribution network from the clock source to all sequential elements such as flip-flops and latches.

The primary objective of CTS is to minimize **clock skew**, **clock latency**, and **clock uncertainty** while maintaining signal integrity and meeting timing requirements.

A well-designed clock tree improves setup and hold timing, reduces clock-related violations, and ensures reliable chip operation.

---

# 📋 Requirements Before CTS

Before performing Clock Tree Synthesis, the following stages must be completed successfully.

## 1️⃣ Placement

- Standard cell placement completed
- Placement optimization performed
- No major placement congestion

---

## 2️⃣ Timing Constraints

The design should contain a valid **SDC** file including:

- Clock Definitions
- Clock Period
- Generated Clocks (if any)
- Input Delays
- Output Delays
- Timing Exceptions

---

## 3️⃣ Clock Network Information

The CTS engine requires:

- Clock Source
- Clock Ports
- Clock Buffers
- Clock Inverters
- Clock Routing Rules

---

## 4️⃣ Power Distribution Network

Before CTS, the following should already exist:

- Power Rings
- Power Stripes
- Special Routing (SRoute)

A proper PDN ensures that inserted clock buffers receive stable power.

---

# 🧩 Clock Tree Synthesis Flow

## 1️⃣ Create Clock Tree Specification

Generate the clock tree specification describing:

- Clock Buffer Cells
- Clock Inverter Cells
- Clock Routing Rules
- Buffer Insertion Strategy

This specification guides the CTS engine during clock optimization.

---

## 2️⃣ Clock Tree Construction

Cadence Innovus inserts clock buffers and inverters to distribute the clock signal evenly throughout the design.

Objectives include:

- Balanced Clock Paths
- Reduced Clock Skew
- Controlled Clock Latency
- Improved Timing

---

## 3️⃣ Clock Optimization

The CTS engine optimizes the clock network by:

- Buffer Insertion
- Buffer Sizing
- Clock Path Balancing
- Delay Adjustment

The goal is to improve setup and hold timing while minimizing clock uncertainty.

---

## 4️⃣ Clock Routing

Dedicated routing resources are used to connect:

- Clock Source
- Clock Buffers
- Clock Inverters
- Sequential Elements

Clock routing follows technology-specific routing rules to reduce delay and signal degradation.

---

## 5️⃣ Post-CTS Timing Analysis

After clock tree construction, timing analysis is performed to verify:

- Setup Timing
- Hold Timing
- Clock Skew
- Clock Latency
- Timing Violations

Any violations are corrected before proceeding to signal routing.

---

# 🎯 Objectives of Clock Tree Synthesis

- Minimize Clock Skew
- Reduce Clock Latency
- Improve Setup Timing
- Improve Hold Timing
- Balance Clock Distribution
- Reduce Clock Uncertainty
- Achieve Timing Closure

---

# 📦 Deliverables

The CTS stage produces:

- Optimized Clock Tree
- Inserted Clock Buffers
- Clock Routing
- Post-CTS Timing Reports
- Updated Physical Database

---

# 📊 Key Metrics

The quality of Clock Tree Synthesis is evaluated using:

- Clock Skew
- Clock Latency
- Setup Slack
- Hold Slack
- Clock Buffer Count
- Clock Tree Depth

---

# ✅ Outcome

A successful Clock Tree Synthesis stage provides a balanced and optimized clock distribution network with minimal skew and positive timing margins.

The design is then ready for the **Signal Routing** stage, where all remaining signal connections are completed before final timing verification and GDSII generation.
