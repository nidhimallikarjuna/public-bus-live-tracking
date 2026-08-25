# Public Bus Live Tracking & Crowding Estimator

## Project Overview

A municipal transit intelligence system that uses bus GPS feeds to track vehicles, estimate arrival times (ETA) at downstream stops, and estimate passenger crowding from ticketing/sensor data.

### Target Stakeholders / Actors

- **Commuter**
- **Fleet Controller**

## Deliverables

### 1. Requirements Table
Contains exactly:
- 5 Functional Requirements (FR-001 to FR-005)
- 2 Non-Functional Requirements (NFR-001 to NFR-002)

See [`Requirements/requirements.pdf`](Requirements/requirements.pdf).

### 2. UML Use-Case Diagram
Models the Commuter and Fleet Controller actors, primary use cases, and the required `<<include>>` and `<<extend>>` relationships.

See [`UML/use-case-diagram.png`](UML/use-case-diagram.png).

### 3. Use-Case Flow Specification
Documents the core **Check Bus ETA** use case with preconditions, postconditions, main success scenario, and an alternate flow for unavailable GPS data.

See [`Use-Case-Flow/check-bus-eta.pdf`](Use-Case-Flow/check-bus-eta.pdf).

## Core System Idea

The system continuously receives bus telemetry, uses the latest valid location data to calculate ETAs, and combines passenger/ticketing information to estimate crowding. This information is presented to commuters and fleet controllers so they can make better travel and operational decisions.
