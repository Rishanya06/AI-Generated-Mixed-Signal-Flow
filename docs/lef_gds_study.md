# LEF and GDS Study

## LEF (Library Exchange Format)

LEF provides a physical abstraction of a macro.

It contains:

* Cell dimensions
* Pin locations
* Routing blockages
* Placement information

OpenLane uses LEF during:

* Floorplanning
* Placement
* Routing

The internal transistor geometry is not included.

---

## GDS (Graphic Data System)

GDS contains the complete physical layout of the circuit.

It includes:

* Transistor geometries
* Metal layers
* Vias
* Contacts
* Complete fabrication information

The GDS file is the final layout delivered for manufacturing.

---

## Why Both Are Required

LEF allows physical-design tools to place and route around the macro.

GDS provides the actual physical implementation.

Together they enable mixed-signal integration without exposing the internal analog design during implementation.
