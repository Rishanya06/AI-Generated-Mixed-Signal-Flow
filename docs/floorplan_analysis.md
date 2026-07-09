# Floorplan Analysis

## Objective

The floorplanning stage defines the physical boundaries of the design and establishes the initial placement area for standard cells, routing resources, and power distribution networks.

## AI-Assisted Investigation

The reference repository was first analyzed using AI-generated prompts to understand how OpenLane performs floorplanning for mixed-signal designs. AI explanations were used to understand:

* Core utilization
* Die area allocation
* Placement boundaries
* Power grid preparation
* Macro placement requirements

The generated explanations were compared against OpenLane documentation before execution.

## Observations

The floorplan was generated successfully during the OpenLane flow without fatal errors.

The design area was automatically configured based on the selected SKY130 standard cell library and OpenLane floorplanning parameters.

The generated floorplan provided sufficient area for subsequent placement and routing stages.

## Result

The floorplanning stage completed successfully and enabled the design to proceed to placement and routing.
