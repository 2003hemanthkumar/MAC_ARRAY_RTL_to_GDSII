# 🏗️ Floorplanning in Cadence Innovus

## 📖 What is Floorplanning?

Floorplanning is the first major stage of the **ASIC Physical Design Flow**, where the physical structure of the integrated circuit (IC) is established. It defines the **die area**, **core dimensions**, **placement region**, **power distribution network (PDN)**, and **routing resources**, creating the foundation for placement, clock tree synthesis, and routing.

A well-planned floorplan minimizes routing congestion, improves timing performance, optimizes power distribution, and enhances the overall quality of the final layout.

---

# 📋 Requirements Before Floorplanning

Before starting floorplanning in **Cadence Innovus**, the following design inputs are required.

## 1️⃣ Technology Files

- **Technology LEF (.lef)** – Defines routing layers, via rules, manufacturing grid, and technology information.
- **Macro LEF (.lef)** – Describes the physical dimensions and pin locations of standard cells and macros.
- **Liberty File (.lib)** – Contains timing, power, and functional characteristics of the standard cell library.

---

## 2️⃣ Logical Design Inputs

- **Synthesized Gate-Level Netlist (.v)** generated from **Cadence Genus**.
- **SDC Constraint File (.sdc)** containing:
  - Clock Definitions
  - Input Delays
  - Output Delays
  - Timing Constraints

---

## 3️⃣ Physical Design Parameters

- Core Utilization
- Aspect Ratio
- Core Margins
- Placement Site Information
- Routing Layer Preferences

---

## 4️⃣ Power Planning Requirements

- Power Net (**VDD**)
- Ground Net (**VSS**)
- Power Rings
- Power Stripes
- Follow Pins

---

# 🧩 Floorplanning Flow

## 1️⃣ Import Design

Load all required design files into **Cadence Innovus**.

### Input Files

- ✔️ Synthesized Netlist
- ✔️ Technology LEF
- ✔️ Macro LEF
- ✔️ Liberty Library
- ✔️ SDC Constraints

---

## 2️⃣ Initialize Floorplan

Define the physical dimensions of the design.

Typical parameters include:

- Core Utilization
- Aspect Ratio
- Core Offset
- Placement Site

The objective is to allocate sufficient routing space while maximizing silicon utilization.

---

## 3️⃣ Power Planning

Create the **Power Distribution Network (PDN)**.

This stage includes:

- Power Rings
- Horizontal Power Stripes
- Vertical Power Stripes

The PDN ensures reliable power delivery across the entire design while minimizing IR drop and voltage fluctuations.

---

## 4️⃣ Special Routing (SRoute)

Special Routing establishes dedicated power connectivity by connecting:

- Standard Cell Power Pins
- Power Rings
- Power Stripes
- Core Power Nets (VDD/VSS)

This step prepares the design for placement and signal routing.

---

## 5️⃣ Floorplan Verification

Verify the following before proceeding:

- ✔️ Core Boundary
- ✔️ Placement Rows
- ✔️ Power Ring Connectivity
- ✔️ Power Stripe Connectivity
- ✔️ Available Routing Resources

Any floorplanning issues should be resolved before the placement stage.

---

# 🎯 Objectives of Floorplanning

- Optimize chip area utilization
- Minimize routing congestion
- Improve timing performance
- Enable efficient power delivery
- Reduce overall wirelength
- Prepare the design for placement and clock tree synthesis

---

# 📦 Deliverables

The floorplanning stage generates:

- Initialized Core Layout
- Placement Rows
- Power Rings
- Power Stripes
- Floorplan Database

---


The quality of the floorplan significantly influences the final performance, power, area, and manufacturability of the ASIC design.
