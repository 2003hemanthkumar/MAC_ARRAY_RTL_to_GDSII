# 🛣️ Signal Routing

## 📖 Overview

Signal Routing is the stage in the ASIC Physical Design flow where all logical net connections are converted into physical metal interconnects. After Clock Tree Synthesis (CTS), Cadence Innovus performs global and detailed routing to establish complete connectivity while satisfying technology design rules and timing constraints.

Routing is a critical step that directly impacts signal integrity, timing closure, manufacturability, and overall design quality.

---

# 🎯 Objectives

- Complete physical connectivity for all signal nets
- Minimize routing congestion
- Eliminate routing overflow
- Meet timing constraints
- Ensure Design Rule Check (DRC) compliance
- Prepare the design for GDSII generation

---

# 📋 Prerequisites

The following stages were completed before routing:

- ✅ Floorplanning
- ✅ Power Planning
- ✅ Standard Cell Placement
- ✅ Clock Tree Synthesis (CTS)
- ✅ Special Routing (SRoute)

---

# 🛠️ Routing Flow

## 1️⃣ Global Routing

Global routing determines the optimal routing paths for signal nets across the chip while minimizing congestion and estimating routing resources.

---

## 2️⃣ Detailed Routing

Detailed routing assigns exact metal layers and routing tracks to every signal net while ensuring compliance with foundry design rules.

---

## 3️⃣ Routing Optimization

After routing, the design is optimized to:

- Reduce congestion
- Improve timing
- Resolve Design Rule Violations (DRVs)
- Optimize wirelength
- Improve signal integrity

---

# ⚙️ Routing Features

| Feature | Description |
|----------|-------------|
| Global Routing | Estimates routing paths and congestion |
| Detailed Routing | Creates physical metal interconnects |
| Timing Optimization | Improves setup and hold timing |
| DRC Fixing | Resolves routing rule violations |
| Wirelength Optimization | Reduces overall interconnect length |

---

# 📊 Routing Results

| Parameter | Result |
|-----------|--------|
| Routing Status | ✅ Completed |
| Routing Overflow | **0.00% Horizontal** |
| Routing Overflow | **0.00% Vertical** |
| Design Connectivity | ✅ Complete |
| Signal Routing | ✅ Successful |

---

# 🧰 Tool Used

| Tool | Purpose |
|------|----------|
| Cadence Innovus | Global Routing, Detailed Routing & Routing Optimization |

---

# 📂 Generated Outputs

The routing stage generated:

- Routed Physical Database
- Routed Signal Nets
- Updated Timing Database
- Routing Reports
- Design Ready for Post-Route Timing Analysis

---

# 📚 Learning Outcomes

Through this stage, the following concepts were implemented:

- Global Routing
- Detailed Routing
- Routing Congestion Analysis
- Routing Overflow Analysis
- Routing Optimization
- Physical Connectivity Verification

---

# ✅ Conclusion

Signal Routing was successfully completed using **Cadence Innovus**. All signal nets were routed with **zero routing overflow**, maintaining complete connectivity and satisfying physical design requirements. The routed design is now ready for **Post-Route Static Timing Analysis (STA)** and **GDSII Stream-Out**.
