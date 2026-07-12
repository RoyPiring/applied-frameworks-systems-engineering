<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Map Your Jagged Frontier with AI

**Project Link:** [View Project](https://nextwork.ai/projects/6fd38dca-b902-44ed-bac6-b4733149fd44)

**Author:** Roy Piring Jr  
**Email:** rpiringhawaii@gmail.com

---

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_scx5lchx)

## Building a Personal AI Mastery Drill from Scratch

### Project vision and goals

This project builds a four-persona AI drill simulator based on the Co-Intelligence framework. The goal was to map my personal Jagged Frontier and identify where AI helped my work, where it needed supervision, and where it became unreliable.

The system turned AI use into a structured practice drill instead of a loose prompting exercise. Each phase required prediction, execution, verification, scoring, and reflection so the learning came from comparing what I expected against what the AI actually did.

This mattered because AI skill is not just knowing how to prompt. It is knowing when to trust, when to verify, and when the model has crossed from useful support into confident overreach.

### Setting up the delivery toolchain

I set up the delivery toolchain by creating the private GitHub repository, jagged-frontier-drill, and establishing the build folder structure. This gave the simulator a version-controlled base where each artifact could be tracked.

I configured the Linear workflow with the required tickets from JFD-1 through JFD-6 and connected Linear to GitHub for workflow tracking. That connected each build step to a ticket and kept the implementation trail visible.

I also verified the AI client had enough rate limits for a 60-minute multi-turn session. The persona prompt test worked because the client correctly defined the jagged frontier in one sentence. I installed Obsidian and confirmed Mermaid rendering so the framework, diagrams, and drill artifacts could be read and maintained in the same workspace.

## Configuring the Build Pipeline: Linear, GitHub, and Obsidian

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_a2klblgj)

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_v4g1sjeq)

## Designing the System Architecture and Methodology

### Design principles and decision records

In this step, I drafted the design-decision record for the drill. It defined the five foundational principles, three core patterns, and four corrected misreadings that governed how the simulator worked.

I also created a Mermaid topology diagram to show how the personas, exercise phases, scoring rubrics, and final outputs connected. That made the drill easier to reason about before running a full session.

I defined the four persona profiles with explicit refusal rules and re-anchor triggers. Those controls mattered because each persona had to stay inside its assigned role during longer interactions instead of drifting into helpful but incorrect behavior.

### Three methodological patterns explained

The first pattern was predict-then-reveal. The learner had to state where they expected AI to fail before prompting the model, because the gap between prediction and result was the real learning signal. The Coach would not let the Mirror answer until a prediction was on the table.

The second pattern was separating the judge from the runtime. The Frontier Guide diagnosed the learner’s position while the Mirror produced the output. Keeping those roles separate stopped the model from grading its own work and drifting into self-approval.

The third pattern required both Centaur and Cyborg modes. The learner had to run at least one task in each mode and judge the fit to the task. The capstone failed if either mode was missing, because the drill was built to compare modes rather than declare one superior.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_o3wprbym)

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_y0fm9i0o)

## Building the Four-Persona Drill Simulator

### Simulator core construction

In this step, I built the core simulator prompt for the four-persona drill. The boot prompt defined the turn protocol, re-anchor cadence, and five profile scenarios.

I also wrote the eight timed-phase prompts that structured the 60-minute drill. Those phases gave the session a clear path from prediction to execution, scoring, and final reflection.

I then defined the Centaur handoff and Cyborg interleave scripts. These scripts made the difference between handoff-based AI work and tightly interleaved AI work explicit, which was needed for fair scoring.

### Centaur vs. Cyborg verification protocols

Centaur mode verified a complete draft as a unit. The AI produced one full deliverable with clear ownership boundaries, so the learner could check and judge the output holistically.

Cyborg mode verified at the seams. Because the output was co-created and could feel like the learner’s own work, verification had to target the Mirror’s specific additions and changes.

The core difference was visibility. Centaur mode made boundaries clear, which made verification simpler but broader. Cyborg mode blurred ownership, so it required finer seam-level checks to avoid trusting model contributions just because they blended into the work.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_q9ow7i5x)

## Creating the Frontier Map, Rubrics, and Adoption Cadence

### Validation instruments and map templates

In this step, I created the core instruments for the Jagged Frontier drill. The system included the Frontier Map skeleton, hypothesis worksheet, lane diagram, and session transcript template.

I also created four validation rubrics with clear pass bars. These covered per-step scoring, capstone scoring, a 6-item diagnostic, and a 30-day re-score instrument.

The adoption tools gave the drill a path beyond one session. The daily check-in protocol and long-term adoption timeline made it possible to turn the frontier map into an ongoing practice habit.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_c15ot7if)

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_sctpe2og)

## Running the Full Validation Pass and Tagging the Release

### Plain-language guide and end-to-end validation

In this step, I drafted the plain-language guide for /guide/README.md. The guide explained setup, run procedure, persona definitions, rubrics, and the caveats needed to run the drill honestly.

I then performed a full end-to-end execution using a chosen work task. The run used the instruments from earlier steps to score the results and confirm whether the simulator worked as designed.

After validation, I finalized the release path by closing the associated Linear tickets and tagging v1.0.0 in GitHub. That gave the build a clean proof trail from planned work to finished release.

### Prediction vs. actual frontier findings

The biggest gap came from sub-task 6, the leadership briefing. I predicted it would land green because executive-summary generation felt like safe AI-native territory, but it actually landed yellow.

The surprise was that the Mirror inserted an unwarranted claim that the pilot demonstrated operational readiness before any pilot had run. The prose looked clean, but the claim overreached the evidence and had to be removed.

The lesson was that frontier position is not determined by task type alone. A generation task can move to the edge the moment AI starts asserting facts it does not have evidence for, which is where the learner can start falling asleep at the wheel.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_scx5lchx)

### Linear-to-GitHub proof-of-work trail

Every step tied a ticket to code. Each deliverable shipped on its own branch and through a pull request that used the real Linear close word, so the intent in the ticket and the implementation in the diff stayed linked.

The status transitions were machine-generated instead of manually set. Merging each pull request moved the ticket through the workflow with webhook timestamps, which created a clear event trail for when each step changed state.

The trail ended in a verifiable anchor. All five merges landed on main, and the v1.0.0 tag pinned the chain to commit da4c00a, so the path could be checked from ticket to pull request to merge to release.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_85nxe9nw)

## Secret Mission: Operational Extensions and Two-Audience Walkthrough

### What broke during validation and how it was fixed

Phase 3 scored 5 out of 6 because the step prompt did not ask for the mode pre-assignment required by the per-step rubric and hypothesis worksheet. That exposed a seam between the simulator and its validation instruments.

The fix was diagnosed and documented as a one-line Phase 3 prompt addition. It was offered but not yet applied, so this remained a fix-forward recommendation rather than a completed fix.

The second issue was the mismatch between the JFD-N labels and the real Linear IDs, which were PS-38 through PS-43. Bare branch pushes and Fixes JFD-N did not move tickets. I corrected this in-flight across all six pull requests by using Closes PS-N with the real IDs, which drove each ticket from Backlog to In Progress to Done.

![Image](https://nextwork.ai/refreshed_maroon_timid_jujube/uploads/6fd38dca-b902-44ed-bac6-b4733149fd44_wlxrqx8b)

## Reflections and Lessons Learned

### Key tools and concepts mastered

The key tools I used included Git and GitHub for version-controlled file management, Linear for ticket-driven tracking, and Obsidian for technical documentation and Mermaid diagrams.

The main concepts I learned included the Co-Intelligence framework for mapping AI capability, the design of a four-persona drill system, refusal rules, re-anchor logic, and the use of a Personal Frontier Map to separate Centaur work from Cyborg work.

The larger lesson was that AI mastery needs a validation loop. The drill forced prediction before prompting, separated execution from judgment, and used rubrics to show where the model helped and where it overreached.

### Time investment and challenges

This build took me approximately 70 minutes. That time covered repository setup, Linear and GitHub linkage, Obsidian validation, persona design, drill prompts, rubrics, end-to-end scoring, release tagging, and issue cleanup.

The hardest part was keeping the persona roles inside their constraints during longer interaction sequences. The main risk was the Executor self-correcting when errors were introduced, which would break the purpose of the drill.

I addressed that by tightening the re-anchor protocol and sharpening the Challenger instructions so role drift could be caught earlier.

### Personal takeaways

I completed this build to create a system for mapping my personal AI frontier. The drill helped me identify where AI strengthened my workflow and where it became prone to hallucination or unsupported claims.

The most useful takeaway was that confidence is not the same as reliability. The model can produce clean prose and still insert a false claim, so the learner has to verify the parts that carry meaning.

Next, I want to apply this persona-based framework to more complex technical workflows so I can strengthen my prompt engineering, validation habits, and AI-assisted delivery process.

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/6fd38dca-b902-44ed-bac6-b4733149fd44)*
