# FBI Negotiation Tactics with AI Roleplay

> Inside the [Applied Frameworks Systems Engineering](../../README.md) portfolio · *Frameworks from books and methodologies, engineered into working systems.*

## Overview

This project turns the FBI hostage-negotiation tactics from Chris Voss's Never Split the Difference into a repeatable, AI-coached rehearsal system for a real salary renegotiation. Across structured roleplay rounds it drills all nine tactics, scores each one before and after, and captures reusable script cards so the techniques hold under live pressure.

In this project, I prepared for an upcoming salary renegotiation by practicing FBI negotiation techniques through AI-powered roleplay. My objective was to build a structured approach that would help me communicate confidently while keeping the conversation collaborative instead of confrontational. Rather than relying on instinct during a high-pressure discussion, I wanted a repeatable framework that would allow me to stay composed regardless of how the conversation evolved.

Throughout the training, I focused on developing a calm delivery using the "late-night FM DJ" voice, sharpening my use of Mirroring and Labeling techniques, and learning how to respond to difficult situations with Calibrated Questions instead of immediate counter-offers. By repeatedly practicing realistic scenarios, I became more comfortable managing tension and maintaining control of the conversation while encouraging the other person to work toward a solution with me.

The architecture is built across **6 phases**, anchored by **Setting Up the Negotiation Coach** on the input side and **Going Further: Adaptation and Teaching** at the end. Each phase is listed in the Implementation section below.

## Architecture

```mermaid
---
title: FBI Negotiation Tactics with AI Roleplay
---
%%{init: {"theme":"base","themeVariables": {"primaryColor":"#1B4332","primaryTextColor":"#F4D03F","primaryBorderColor":"#F4D03F","secondaryColor":"#264653","tertiaryColor":"#2F5233","lineColor":"#F4D03F","fontFamily":"ui-monospace, SFMono-Regular, Menlo, Consolas, monospace","fontSize":"13px"}}}%%
flowchart TD
    classDef datastore fill:#264653,stroke:#F4D03F,stroke-width:2px,color:#FFFFFF
    classDef service fill:#1B4332,stroke:#F4D03F,stroke-width:2px,color:#F4D03F
    classDef event fill:#7B42BC,stroke:#F4D03F,stroke-width:2px,color:#FFFFFF
    classDef io fill:#0d1117,stroke:#F4D03F,stroke-width:1.5px,color:#F4D03F,font-style:italic

    Scenario[/Real Negotiation Scenario/] --> Coach
    BeforeScore[/Baseline Self-Assessment 12 of 27/] --> Coach

    subgraph Setup[Environment Setup]
        PSScript(PowerShell Setup Script)
        ProjectFiles[(Generated Project Files)]
        EdgeTTS(edge-tts Voice Engine)
        Playbook[(Pocket Playbook)]
    end

    Setup --> Coach

    subgraph Coach[AI Negotiation Coach]
        ClaudeDesktop(Claude Desktop)
        Cowork(Cowork Project)
        SystemPrompt[(AI Coach System Prompt)]
    end

    ClaudeDesktop -->|teaches| Tactics
    ClaudeDesktop -->|runs| Rounds

    subgraph Tactics[Nine FBI Tactics - Voss Method]
        Mirror([Mirroring])
        Label([Labeling])
        Empathy([Tactical Empathy])
        Audit([Accusation Audit])
        ThatsRight([That's Right])
        Calibrated([Calibrated Questions])
        NoGambit([The No Gambit])
        Ackerman([Ackerman Bargaining])
        BlackSwan([Black Swans])
    end

    subgraph Rounds[Progressive Practice Rounds]
        direction TB
        MirrorDrill{{Mirror Drills x3}}
        LabelDrill{{Labeling Drills x3}}
        QuestionDrill{{Calibrated Question Drills}}
        Capstone{{Capstone - 4 Scenarios}}
        MirrorDrill --> LabelDrill --> QuestionDrill --> Capstone
    end

    Mirror -. drilled in .-> MirrorDrill
    Label -. drilled in .-> LabelDrill
    Empathy -. drilled in .-> LabelDrill
    Calibrated -. drilled in .-> QuestionDrill
    Audit -. combined in .-> Capstone
    NoGambit -. combined in .-> Capstone
    Ackerman -. combined in .-> Capstone
    BlackSwan -. combined in .-> Capstone

    Capstone -->|best line feeds| Voice

    subgraph Voice[Voice Playback Pipeline]
        BestScript[(best-script.txt)]
        GenPlayback(generate-playback Script)
        AudioFiles[(Audio Playback Files)]
        BestScript --> GenPlayback --> AudioFiles
    end

    MirrorDrill -->|saves| MirrorCard[(Mirror Script Card)]
    LabelDrill -->|saves| LabelCard[(Label Script Card)]
    Audit -->|produces| AuditCard[(Accusation Audit Card)]

    Rounds -->|telemetry| AfterScore[/Final Assessment 27 of 27/]
    AfterScore -->|plus 15 point gain| Review{{Pre vs Post Review}}

    Review --> Further

    subgraph Further[Going Further]
        Adapt(Archetype Adaptation)
        Teach(Teach the Mirror Technique)
    end

    class ProjectFiles,Playbook,SystemPrompt,BestScript,AudioFiles,MirrorCard,LabelCard,AuditCard datastore
    class PSScript,EdgeTTS,ClaudeDesktop,Cowork,GenPlayback,Mirror,Label,Empathy,Audit,ThatsRight,Calibrated,NoGambit,Ackerman,BlackSwan,Adapt,Teach service
    class MirrorDrill,LabelDrill,QuestionDrill,Capstone,Review event
    class Scenario,BeforeScore,AfterScore io
```

The diagram shows the topology and data flow of the system as built. The full architectural narrative, with screenshots and prose, lives in [`documents/fbi-negotiation-ai-roleplay.md`](./documents/fbi-negotiation-ai-roleplay.md).

## Implementation

This system is built across **6 phases**:

1. **Setting Up the Negotiation Coach**
2. **Mastering the Mirror Technique Under Pressure**
3. **Labeling Emotions to Earn 'That's Right'**
4. **Using Calibrated Questions to Drive the Negotiation**
5. **Closing with No, Ackerman, and Black Swan Tactics**
6. **Going Further: Adaptation and Teaching**

For the full walkthrough with screenshots and step-by-step content, see [`documents/fbi-negotiation-ai-roleplay.md`](./documents/fbi-negotiation-ai-roleplay.md).

## Validation

Build outcomes verified end-to-end. Each phase below is captured with screenshots, configuration, and observable behavior in [`documents/fbi-negotiation-ai-roleplay.md`](./documents/fbi-negotiation-ai-roleplay.md):

- ✅ Setting Up the Negotiation Coach
- ✅ Mastering the Mirror Technique Under Pressure
- ✅ Labeling Emotions to Earn 'That's Right'
- ✅ Using Calibrated Questions to Drive the Negotiation
- ✅ Closing with No, Ackerman, and Black Swan Tactics
- ✅ Going Further: Adaptation and Teaching
