
# VLSI SoC Design & Chip Modeling

These are the **seven steps of chip modeling** we learnt in class. The goal is to move from **spec → silicon** while keeping verification checkpoints consistent (**O0 = O1 = O2 = O3**).

---

## 🔹 Step 1: Specification Modeling

* **Task:** Model the specifications using a **C-like testbench**.
* **Goal:** Make O0 → O1.
* **Deliverables:** `spec/testbench.c`, golden vectors.

---

## 🔹 Step 2: RTL Design (Verilog)

* **Task:** Convert specification into **RTL using Verilog**.
* **Goal:** Make O0 = O1 = O2 (soft copy of hardware).
* **Deliverables:** `rtl/*.v`, RTL testbench, simulation results.

---

## 🔹 Step 3: RTL Partitioning

* **Task:** Divide Verilog into **processor and peripherals**.

  * Processor → synthesizable gate-level netlist (soft logic).
  * Peripherals → macros (synth RTL).
  * Analog IPs → functional RTL.
* **Goal:** Maintain O1 = O2 consistency.
* **Deliverables:** `rtl/processor/`, `rtl/peripherals/`, analog IP functional models.

---

## 🔹 Step 4: SoC Integration

* **Task:** Integrate processor and peripherals using **GPIOs and buses**.
* **Deliverables:** Top-level RTL, integration scripts.
* **Goal:** Integrated behavior matches intended O2 behavior.

---

## 🔹 Step 5: Physical Design (PD)

* **Task:** Floorplanning → Placement → CTS → Routing.
* Hardened macros and analog IP libraries. Processor remains soft logic.
* **Deliverables:** Floorplan, placement reports, CTS, routed netlists.
* **Goal:** Preserve functional intent (O2).

---

## 🔹 Step 6: GDSII & Sign-off

* **Task:** Generate **GDSII file**.
* Run **DRC/LVS checks** (tapeout and tapein).
* **Deliverables:** Final GDS, DRC/LVS reports.
* **Goal:** Layout = schematic and rule-clean (O3).

---

## 🔹 Step 7: Final Verification & Handoff

* **Task:** Add peripherals to the chip and run **full-chip testbench**.
* **Goal:** Ensure **O0 = O1 = O2 = O3**.
* **Deliverables:** Full-chip test vectors and verification report.

---

