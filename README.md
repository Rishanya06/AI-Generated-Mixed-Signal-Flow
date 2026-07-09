# AI-Assisted Mixed-Signal Physical Design Flow

## Overview

This project documents an AI-assisted approach for understanding and reproducing a mixed-signal RTL-to-GDS flow using OpenLane and the SKY130 Process Design Kit (PDK).

The work is based on studying the reference repository:

https://github.com/praharshapm/vsdmixedsignalflow

Rather than directly copying the implementation, AI tools were used to analyze the repository, understand the physical design flow, generate supporting artifacts, assist debugging, and document the complete engineering process.

The objective was to demonstrate how AI can support mixed-signal physical design while maintaining manual verification and engineering judgement.

---

## Project Objectives

* Understand the reference mixed-signal repository
* Study analog macro integration using AMUX2_3V
* Explore LEF, GDS, and OpenLane configuration files
* Generate AI-assisted implementation artifacts
* Document debugging workflows
* Verify OpenLane execution results
* Compare AI-assisted methodology with the reference flow

---

## Tools Used

### Physical Design Tools

* OpenLane
* SKY130 PDK
* Magic
* Netgen
* OpenROAD

### AI Tools

* ChatGPT (GPT-5)

Used for:

* Repository analysis
* Prompt generation
* Macro study
* Configuration understanding
* Debugging assistance
* Documentation generation
* Report interpretation

---

## Repository Structure

```text id="3jnnm2"
docs/              → Technical documentation
prompts/           → AI prompts used throughout the project
generated_files/   → AI-generated artifacts and verification files
debugging/         → Error analysis and debugging records
screenshots/       → Flow outputs and verification evidence
```

---

## AI-Assisted Workflow

The project followed the workflow:

```text id="g5lq8d"
Repository Study
        ↓
Prompt Creation
        ↓
AI Analysis
        ↓
Manual Verification
        ↓
OpenLane Execution
        ↓
Debugging
        ↓
Report Analysis
        ↓
Final Documentation
```

---

## Key Topics Explored

### Repository Understanding

The reference repository was analyzed to understand:

* Mixed-signal design hierarchy
* Analog macro integration
* OpenLane implementation stages
* Required input files
* Expected outputs

### Analog Macro Study

The AMUX2_3V analog macro was studied to understand:

* Verilog wrappers
* LEF abstraction
* GDS representation
* Black-box integration methodology

### Physical Design Flow

The following stages were explored:

* Synthesis
* Floorplanning
* Placement
* Routing
* DRC verification
* LVS verification
* GDS generation

---

## Results

Final implementation results:

* OpenLane flow completed successfully
* Final GDS generated
* Layout verified in Magic
* DRC violations = 0
* LVS status = Clean
* Matched Nets = 359
* Fanout Violations = 3
* Antenna Violations = 1 pin, 1 net

---

## Screenshots

Available evidence includes:

* GDS generation
* Magic layout inspection
* Routed layout views
* Metrics reports
* STA reports
* Manufacturability analysis
* LVS verification

---

## Key Learning Outcomes

This project provided practical exposure to:

* Mixed-signal physical design
* Analog macro integration
* LEF and GDS usage
* OpenLane implementation flow
* DRC and LVS verification
* Engineering debugging workflows
* AI-assisted design exploration

The most valuable lesson was learning how to use AI as an engineering assistant while independently validating every result through actual tool execution and verification.

---

## Reference

Reference Repository:

https://github.com/praharshapm/vsdmixedsignalflow
