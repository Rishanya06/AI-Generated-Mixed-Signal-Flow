# Repository Breakdown

## Reference Repository

https://github.com/praharshapm/vsdmixedsignalflow

## Objective

The repository demonstrates a mixed-signal RTL-to-GDSII flow using OpenLane and the SKY130 Process Design Kit.

The design integrates an analog 2:1 multiplexer macro (AMUX2_3V) into a digital implementation flow.

---

## High-Level Flow

RTL Verilog
↓
Synthesis (Yosys)
↓
Floorplanning
↓
Placement
↓
Clock Tree Synthesis
↓
Routing
↓
DRC/LVS Verification
↓
GDSII Generation

---

## Key Components

### RTL Design

Digital logic described using Verilog.

### Analog Macro

AMUX2_3V analog multiplexer integrated as a black-box macro.

### LEF

Provides physical dimensions and pin locations.

### LIB

Provides timing information.

### OpenLane

Performs physical implementation.

### Magic

Used for layout inspection and DRC verification.

### Netgen

Used for LVS verification.

---

## Expected Outputs

* GDSII
* DEF
* LEF
* Timing Reports
* DRC Reports
* LVS Reports
