# 🏭 GDSII Stream-Out

## 📖 Overview

GDSII Stream-Out is the final stage of the ASIC Physical Design flow, where the completed physical layout is exported into the **GDSII (Graphic Data System II)** format. The generated GDSII file contains all geometric information required for semiconductor fabrication, including standard cells, routing, vias, metal layers, and physical design structures.

After successful timing closure and routing verification, the MAC Array design was streamed out as a GDSII file using **Cadence Innovus**.

---

# 🎯 Objectives

- Generate the final GDSII layout database
- Export the complete physical design
- Verify successful stream-out completion
- Prepare the design for fabrication

---

# 📋 Prerequisites

Before generating the GDSII file, the following implementation stages were successfully completed:

- ✅ Floorplanning
- ✅ Power Planning
- ✅ Standard Cell Placement
- ✅ Clock Tree Synthesis (CTS)
- ✅ Signal Routing
- ✅ Post-Route Timing Analysis
- ✅ Design Rule Verification (DRV)

---

# 🛠️ GDSII Stream-Out Flow

## 1️⃣ Design Verification

The routed design was verified for:

- Timing Closure
- Physical Connectivity
- Design Rule Compliance

---

## 2️⃣ Stream-Out Configuration

Cadence Innovus was configured with:

- Layer Mapping File
- Technology LEF
- Standard Cell LEF
- Routed Design Database

---

## 3️⃣ GDSII Generation

The complete physical layout was exported into a **GDSII (.gds)** file containing all fabrication-ready geometric information.

---

# 📊 Stream-Out Results

| Parameter | Status |
|-----------|--------|
| Stream-Out | ✅ Successful |
| GDSII File Generated | ✅ Yes |
| Physical Layout Exported | ✅ Complete |
| Design Ready for Fabrication | ✅ Yes |

---

# 📁 Generated Deliverables

The final implementation produced:

- ✅ GDSII Layout File (.gds)
- ✅ Routed Physical Database
- ✅ Timing Reports
- ✅ Design Rule Reports
- ✅ Final Physical Layout

---

# 🧰 Tool Used

| Tool | Purpose |
|------|----------|
| Cadence Innovus | GDSII Stream-Out |

---

# 📚 Learning Outcomes

Through this stage, the following concepts were implemented:

- GDSII Stream-Out
- Physical Layout Export
- Manufacturing Database Generation
- Final Design Verification
- ASIC Tape-Out Preparation

---

# 🎯 Final Design Status

| Check | Status |
|--------|--------|
| RTL Design | ✅ Completed |
| Logic Synthesis | ✅ Completed |
| Floorplanning | ✅ Completed |
| Placement | ✅ Completed |
| Clock Tree Synthesis | ✅ Completed |
| Signal Routing | ✅ Completed |
| Timing Closure | ✅ Achieved |
| GDSII Generation | ✅ Completed |

---

# 🏁 Conclusion

The **MAC_ARRAY** ASIC Physical Design flow was successfully completed from **RTL to GDSII** using **Cadence Genus** and **Cadence Innovus**. The design achieved successful timing closure, clean design rule verification, successful signal routing, and final GDSII stream-out, producing a fabrication-ready layout database.
