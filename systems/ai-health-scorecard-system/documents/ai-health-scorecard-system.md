<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build an AI Health Scorecard System

**Project Link:** [View Project](https://learn.nextwork.org/projects/b1c2d865-f776-4554-812e-67190ff30935)

**Author:** Roy Piring Jr  
**Email:** rpiringhawaii@gmail.com

---

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_ecp9gq9f)

## Building a Personal AI Health Assessment System

### Project overview

In this project, I built an AI-powered personal health assessment system modeled after the longevity framework discussed in Outlive. The goal was to create a proactive system for understanding long-term health trajectory instead of reacting only after visible health decline appears.

The platform combined Claude Code, Obsidian, Mermaid diagrams, Fitbit telemetry, and multi-agent scoring workflows into a unified assessment pipeline. The system focused on prevention, longitudinal tracking, behavioral calibration, and actionable health optimization instead of generic wellness tracking.

### Environment setup goals

I verified Claude Code installation and authentication, created an Obsidian vault with the required folder structure and configuration files, and validated Mermaid Live Editor rendering for architecture visualization.

The environment was designed around persistent storage for prompts, scores, exports, dashboard code, and recurring assessments. This ensured the project remained reproducible, organized, and easy to iterate over time without losing operational consistency.

## Setting Up the Project Environment

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_qk8acnia)

### Tools and their roles

The tooling stack intentionally prioritized local-first workflows over cloud-hosted health platforms. This strengthened privacy, reduced vendor dependency, and preserved full control over prompts, dashboards, and personal health data.

The modular structure also simplified experimentation because scoring logic, orchestration behavior, and dashboard layouts could be modified directly without platform restrictions.

## Defining the Vision Anchor and Pipeline Architecture

### Step goals

I created a Personal Vision Anchor document defining five specific capabilities desired at age 90, then designed the six-agent assessment pipeline using Mermaid diagrams and structured input/output contracts.

Agent prompts, cross-validation rules, and score templates were then created to standardize orchestration behavior across the full pipeline.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_l79mb01q)

### Vision Anchor purpose and cross-validation logic

The Vision Anchor connected abstract health scores to meaningful future-life outcomes. A low metabolic score no longer represented only weak performance; it represented a direct threat to future independence, mobility, and quality of life.

Cross-validation logic forced wearable telemetry to act as a tiebreaker against self-reporting. This exposed gaps between perceived behavior and measured reality while reducing two major failure modes simultaneously: optimizing for the wrong goals and inaccurately reporting the right behaviors.

## Building the Conversational Assessment Engine

### Assessment engine goals

I developed the Intake Interviewer prompt containing five assessment modules, predict-then-reveal engagement logic, and emergency escalation handling.

The Data Integrator agent was then designed to process Fitbit telemetry, reconcile self-reported behaviors, and apply cross-validation logic before scoring workflows began.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_wh9h1q87)

### Predict-then-reveal engagement design

The predict-then-reveal workflow converted passive health metrics into active behavioral feedback. Users estimated metrics such as sleep quality, daily steps, or exercise intensity before viewing wearable telemetry.

This exposed overconfidence patterns while deepening long-term self-calibration. Repeated prediction cycles trained users to recognize where their intuition aligned with reality and where it consistently drifted.

Why behavioral calibration mattered

Most people significantly overestimate exercise consistency, sleep quality, and recovery performance. Seeing “predicted 8,000 steps / actual 3,200” creates stronger behavioral awareness than simply viewing a low metric in isolation.

The system treated the prediction gap itself as meaningful data instead of just user error.

## Building the Scoring Engine and Protocol Generator

### Scoring engine goals

I developed the Scoring Engine agent to generate domain scores with confidence indicators and Vision Anchor alignment.

The Protocol Architect identified the highest-leverage intervention across all domains, while the Pressure Tester introduced adversarial personas designed to challenge weak assumptions, unreliable data, and insufficient intervention plans.

### Priority Stack decision logic

The Priority Stack prioritized interventions capable of lifting multiple health domains simultaneously. Actions such as Zone 2 cardio strengthened metabolic health, cardiorespiratory performance, and sleep quality together, giving them significantly higher operational leverage.

When multiple interventions showed similar leverage, the Vision Anchor acted as the tie-breaker by prioritizing actions most connected to long-term capabilities and future-life goals.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_rcgz1dfs)

### Pressure Tester antagonist personas

The Skeptic persona challenged underreported calorie intake, exaggerated exercise intensity, and unreliable self-assessment patterns. Future Self at 75 challenged whether interventions were aggressive enough to realistically support the desired quality of life decades later.

One persona audited data reliability while the other audited long-term adequacy. Together they pressured the system toward more honest and actionable outputs.

## Running the First Full Assessment

### Assessment run goals

I reviewed a worked example, exported Fitbit telemetry, gathered physical measurements, and executed all assessment agents sequentially inside Claude Desktop before saving the final scored outputs.

This validated the full orchestration workflow across intake, integration, scoring, protocol generation, and adversarial review stages.

### Physical measurements and self-test results

The assessment incorporated balance testing, grip strength, mobility scoring, dead-hang endurance, body measurements, and wearable telemetry into a unified health profile.

Strength metrics reinforced evidence of a strength-trained profile, while metabolic indicators and recovery data surfaced weaker domains requiring deeper investigation.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_nudamjfy)

### Priority Stack action and Vision Anchor connection

The system identified fasting insulin and HbA1c testing as the highest-leverage next step because metabolic health represented the weakest-confidence domain with the highest long-term risk exposure.

The recommendation connected directly to the Vision Anchor capability focused on maintaining independence and dietary flexibility later in life.

## Building the Interactive Dashboard

### Dashboard build goals

I used Claude Code to generate an interactive dashboard featuring radar charts, source-quality indicators, trajectory projections, quarterly comparison views, and a collapsible Data Upgrade Path section.

The dashboard consolidated assessment outputs into a visual decision-support system tuned for recurring reviews and long-term trend tracking.

### Source quality indicator system

The dashboard categorized confidence into green, amber, and gray evidence states. Green represented directly measured telemetry such as HRV and VO2 max, while amber represented validated estimates derived from self-reporting.

Gray indicated missing or contradictory inputs so uncertainty remained visible instead of presenting all metrics with equal reliability.

The dashboard was intentionally designed to remain operational rather than motivational. Instead of focusing on gamification, the interface emphasized leverage, trend visibility, confidence weighting, and decision clarity.

This transformed the system into a structured analytical workflow instead of a generic wellness application.

## Establishing Reviews, Check-ins, and Quarterly Re-runs

### Review system goals

I created an After Action Review workflow to translate assessment outputs into operational next steps, then designed lightweight weekly check-ins to maintain continuity between quarterly reassessment cycles.

Quarterly re-run protocols and anti-drift re-anchoring workflows were also implemented to ensure scoring logic and long-term priorities remained aligned over time.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_60gcsl6i)

### Committed Priority Stack action

The system committed to scheduling fasting insulin and HbA1c testing as the highest-leverage next action across the scorecard.

The recommendation was prioritized because of family history, BMI indicators, waist measurements, and uncertainty surrounding long-term metabolic health.

The project treated health optimization as a continuous feedback system rather than a one-time evaluation. Repeated assessments sharpen calibration, expose trajectory shifts, and reduce the likelihood of unnoticed long-term decline.

This transformed the platform into a longitudinal decision-support system instead of a static health report.

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_r5z1x5od)

## Secret Mission: Building the Biological Age Clock

![Image](https://learn.nextwork.org/refreshed_maroon_timid_jujube/uploads/b1c2d865-f776-4554-812e-67190ff30935_ogdhzujl)

### Connecting biological age to Vision Anchor capabilities

The biological age clock weighted cardiorespiratory health, metabolism, sleep, strength, and nutrition into a composite delta against chronological age.

Instead of presenting only a number, the system mapped each Vision Anchor capability to the domains most responsible for preserving it long term.

## Reflections and Key Takeaways

### Tools and concepts learned

This project combined Claude Code, Obsidian, Mermaid diagrams, Fitbit telemetry, local HTML dashboards, and multi-agent orchestration into a structured AI-assisted health assessment platform.

The concepts reinforced included behavioral calibration, longitudinal tracking, data visualization, protocol generation, confidence scoring, and connecting measurable health metrics directly to long-term life outcomes.

### Time and challenges

This project required approximately 70 minutes to complete. The most difficult part was refining the dashboard structure to balance clarity, usability, and meaningful data density without overwhelming the user.

Multiple iterations were required across scoring presentation, projection logic, and dashboard layout before the system felt operationally coherent.

### Personal learning reflection

I completed this project to deepen my understanding of AI-assisted health assessment systems and learn how wearable telemetry, self-assessment, and long-term planning can operate together inside a structured scoring framework.

The next area I want to deepen is advanced health-data visualization using more dynamic dashboards and longitudinal trend analysis models.

---

*Built with [NextWork](https://learn.nextwork.org) - [View this project](https://learn.nextwork.org/projects/b1c2d865-f776-4554-812e-67190ff30935)*
