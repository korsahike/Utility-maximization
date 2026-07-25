# Geospatial Optimization & Fleet Telemetry

##Project Objective

This repository contains an end to end geospatial AI & Multi agents Telematics system to design,track,control and analyse an autonomous robotic fleet in real time. The system uses a feedback control loop with spatial econometric diagnostics and a spatial database layer to optimises multi agent systems operations and also detetcing spatial anomalies.

##System Architecture
```mermaid
graph TD
    A[Simulated fleet telemetry dataframe] --> |kinematics engine|,B(Proportional Controller,v& omega)
    A -->|Spatial Topology| C(Global Morans I Network Analysis)
    B -->|WKT Geometries & Metrics| D(SpatiaLite Relational Database Engine)

