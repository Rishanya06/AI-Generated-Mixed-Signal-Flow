# Required Inputs

## Mandatory Files

### RTL Verilog

Describes the digital logic of the design.

Example:

* design_mux.v
* spi_slave.v
* raven_spi.v

---

### Analog Macro Wrapper

Provides logical representation of the analog block.

Example:

* AMUX2_3V.v

---

### LEF File

Provides:

* Macro dimensions
* Pin locations
* Routing blockages

Example:

* AMUX2_3V.lef

---

### OpenLane Configuration

Controls implementation settings.

Examples:

* config.json
* config.tcl

---

### SKY130 PDK

Provides:

* Standard cells
* Technology rules
* Timing libraries

---

## Generated Outputs

### DEF

Placement and routing information.

### GDS

Final layout database.

### Timing Reports

Generated after implementation.

### DRC Reports

Physical rule verification.

### LVS Reports

Logical-versus-physical verification.

---

## Optional Files

### Documentation

Project reports and observations.

### Screenshots

Flow execution and layout verification images.
