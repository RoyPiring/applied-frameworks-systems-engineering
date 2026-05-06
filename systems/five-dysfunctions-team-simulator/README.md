# Five Dysfunctions Team Simulator

> Inside the [Applied Frameworks Systems Engineering](../../README.md) portfolio · *Frameworks from books and methodologies, engineered into working systems.*

## Overview

This project builds an AI-driven simulator to operationalize Lencioni's Five Dysfunctions model through controlled interaction with resistant personas.

Instead of passively reading theory, the system forces real-time diagnosis and intervention across all five layers of the dysfunction pyramid. Each interaction is mapped to observable behavior and then tied to measurable business outcomes. The simulator creates a closed loop where leadership actions can be tested, evaluated, and refined under pressure conditions that resemble real team dynamics.

The architecture is built across **10 phases**, anchored by **Building an AI Team Effectiveness Simulator** on the input side and **Upward Accountability in a High Power-Distance Variant** at the end. Each phase is listed in the Implementation section below.

## Architecture

```mermaid
---
title: Five Dysfunctions Team Simulator
---
%%{init: {"theme":"base","themeVariables": {"primaryColor":"#1B4332","primaryTextColor":"#F4D03F","primaryBorderColor":"#F4D03F","secondaryColor":"#264653","tertiaryColor":"#2F5233","lineColor":"#F4D03F","fontFamily":"ui-monospace, SFMono-Regular, Menlo, Consolas, monospace","fontSize":"13px"}}}%%
flowchart TD
    classDef datastore fill:#264653,stroke:#F4D03F,stroke-width:2px,color:#FFFFFF
    classDef service fill:#1B4332,stroke:#F4D03F,stroke-width:2px,color:#F4D03F
    classDef event fill:#7B42BC,stroke:#F4D03F,stroke-width:2px,color:#FFFFFF
    classDef io fill:#0d1117,stroke:#F4D03F,stroke-width:1.5px,color:#F4D03F,font-style:italic







    Facilitator[/Leader Interventions/] --> Harness
    BeforeKPI[/Before KPI Scorecard/] --> Harness

    subgraph Harness[Simulation Harness]
        ClaudeDesktop(Claude Desktop Executor)
        MermaidViz(Mermaid Live Editor)
        SimFile[(Persona and Prompt Spec)]
    end

    ClaudeDesktop -->|loads personas| ForgeTeam
    ClaudeDesktop -->|injects| Trigger{{Pressure Event}}

    subgraph ForgeTeam[Forge Robotics Personas]
        Maya(Maya - Silent Skeptic)
        Sam(Sam - Harmony Keeper)
        Dev(Dev - Deflector)
        Jordan(Jordan - Status Seeker)
    end

    Trigger -->|triggers dysfunction| Stack

    subgraph Stack[Lencioni Dysfunction Pyramid]
        direction TB
        Trust([1 - Absence of Trust])
        Conflict([2 - Fear of Conflict])
        Commitment([3 - Lack of Commitment])
        Accountability([4 - Avoidance of Accountability])
        Results([5 - Inattention to Results])
        Trust -->|blocks| Conflict
        Conflict -->|weakens| Commitment
        Commitment -->|undermines| Accountability
        Accountability -->|erodes| Results
    end

    Maya -. surfaces .-> Trust
    Sam -. surfaces .-> Conflict
    Dev -. surfaces .-> Accountability
    Jordan -. surfaces .-> Results

    Stack -->|emits behavior signals| State[(Team State Telemetry)]
    State -->|scores| AfterKPI[/After KPI Scorecard/]
    AfterKPI -->|reports back| Facilitator
    AfterKPI -->|feeds AAR| Capstone{{Capstone Integrated Challenge}}
    Capstone -->|re-triggers| Trigger
class SimFile datastore
class Facilitator,BeforeKPI io

    class SimFile datastore
    class ClaudeDesktop,MermaidViz,Maya,Sam,Dev,Jordan,Trust,Conflict,Commitment,Accountability,Results service
    class Facilitator,BeforeKPI io
```

The diagram shows the topology and data flow of the system as built. The full architectural narrative, with screenshots and prose, lives in [`documents/five-dysfunctions-team-simulator.md`](./documents/five-dysfunctions-team-simulator.md).

## Implementation

This system is built across **10 phases**:

1. **Building an AI Team Effectiveness Simulator**
2. **Diagnosing Team Dysfunction: The Before KPI Scorecard**
3. **Building Vulnerability-Based Trust with Maya**
4. **Mining Productive Conflict with Sam**
5. **Driving Commitment Through Clarity and Buy-In**
6. **Delivering Peer Accountability Without Escalation**
7. **Focusing the Team on Collective Results**
8. **Capstone Meeting: All Five Layers Simultaneously**
9. **Before vs. After: Proving the KPI Movement**
10. **Upward Accountability in a High Power-Distance Variant**

For the full walkthrough with screenshots and step-by-step content, see [`documents/five-dysfunctions-team-simulator.md`](./documents/five-dysfunctions-team-simulator.md).

## Validation

Build outcomes verified end-to-end. Each phase below is captured with screenshots, configuration, and observable behavior in [`documents/five-dysfunctions-team-simulator.md`](./documents/five-dysfunctions-team-simulator.md):

- ✅ Building an AI Team Effectiveness Simulator
- ✅ Diagnosing Team Dysfunction: The Before KPI Scorecard
- ✅ Building Vulnerability-Based Trust with Maya
- ✅ Mining Productive Conflict with Sam
- ✅ Driving Commitment Through Clarity and Buy-In
- ✅ Delivering Peer Accountability Without Escalation
- ✅ Focusing the Team on Collective Results
- ✅ Capstone Meeting: All Five Layers Simultaneously
- ✅ Before vs. After: Proving the KPI Movement
- ✅ Upward Accountability in a High Power-Distance Variant
