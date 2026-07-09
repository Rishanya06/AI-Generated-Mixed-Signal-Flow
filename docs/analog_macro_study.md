# Analog Macro Study

## What is an Analog Macro?

An analog macro is a pre-designed circuit block that is integrated into a larger digital system.

Unlike standard-cell digital logic, analog circuits are usually handcrafted and represented through physical layout abstractions.

---

## Macro Used

AMUX2_3V

Function:

2:1 Analog Multiplexer

The macro selects one of two analog input signals and routes it to the output based on a control signal.

---

## Files Associated with the Macro

### Verilog Wrapper

Provides logical connectivity for synthesis.

Example:

AMUX2_3V.v

---

### LEF File

Provides:

* Physical dimensions
* Pin locations
* Routing blockages

Used by floorplanning and placement tools.

---

### GDS File

Contains actual mask layout geometry.

Used for fabrication and layout verification.

---

### LIB File

Contains timing and power information.

Used during timing analysis.

---

## OpenLane Perspective

OpenLane treats the analog macro as a black box.

The internal transistor-level implementation is not synthesized.

Instead, OpenLane uses:

* LEF for physical placement
* LIB for timing
* Verilog wrapper for connectivity

This allows analog and digital blocks to coexist in the same design.
