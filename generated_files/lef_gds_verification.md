# LEF/GDS Verification

## Objective

Verify understanding of physical abstraction versus physical implementation.

## Verification

LEF was identified as the physical abstraction used by OpenLane.

GDS was identified as the final physical layout database used for manufacturing.

The AMUX2_3V macro follows this methodology:

* LEF → Placement and routing
* GDS → Final layout representation

## Observation

Successful mixed-signal integration requires both views of the macro.

## Status

Verified
