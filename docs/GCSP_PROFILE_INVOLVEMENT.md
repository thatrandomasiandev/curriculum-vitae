# GCSP Profile — Involvement Descriptions

Paste-ready text for Grand Challenges Scholars Program profile fields.  
Profile links: LinkedIn `www.linkedin.com/in/jterranovacs` · Website `www.jcompsci.com` · Expected grad year 2028 · Theme Joy of Living

---

## Rocket Propulsion Laboratory

I work on software for RPL's liquid and hybrid propulsion tests. On hot-fire days that usually means pressure transducers, thermocouples, and load cells logging at the right rates, with alarms set so out-of-range readings are obvious. I wrote the pre-fire checklist, countdown, and abort tooling so the team is not depending on memory under pressure. After a run I help turn raw traces into chamber pressure, specific impulse, and thrust curves from the load cell. During design I've helped with mass-flow estimates, nozzle expansion trades, and rough thermal margins. None of it is flashy. Bad logging or a missed abort can waste a test, so I focus on the unglamorous parts.

---

## Field Robotics Lab

I lead software for our URC 2026 rover on ROS 2 (Humble). I also wrote the full computer vision stack myself: camera calibration, ArUco marker detection with IPPE pose estimation, multi-frame confirmation gating, YOLO-based object detection with class-wise acceptance rules, depth-assisted bearing and distance estimates, and the visual servo PID that closes the loop on docking. No one else on the team owns that perception path. Detections feed a seven-target mission orchestrator that steps the rover through GNSS waypoints, post search arcs, precision approach, and science-object stops under URC 2026 rules.

On the navigation side I built GNSS following with WGS-84 to local ENU transforms, EKF fusion across IMU, wheel odometry, and GPS via `robot_localization`, and Nav2 integration so perception outputs trigger behavior-tree transitions instead of one-off scripts. Competition safety work includes hardware and software e-stops, watchdogs, heartbeat checks, and a judge-facing WebSocket dashboard. I wrote a 1,000+ line architecture spec that maps GPS acceptance (haversine plus multi-frame confirmation), ArUco gating, servo gains, YOLO `ObjectGate` logic, twist_mux priorities, and the e-stop lattice back to the written rules, so parameters are traceable rather than tuned by guesswork. We test outdoors often. I track localization drift, false-positive rates on detections, and replan latency before competition week.

---

## SC Racing, Project Athena

On USC Racing I own the path from the car to data a driver or engineer can use. That is getting suspension, brake, and powertrain sensors on the bus, logging CAN traffic, and feeding displays plus post-run analysis. I've helped with suspension geometry and lap-time simulation so setup changes are not pure guesswork. Race weekends are messy. I want logs the team can trust in the few minutes between sessions.

---

## Research (non-program affiliated)

Active project (2026): I am building Module 11 of my research suite: From Pixels to Actions, a unified visual robot learning benchmark and paper on the Visual Compounding Problem. The claim is that perception and control modules can pass isolated benchmarks and still fail in deployment because errors multiply through the camera-to-action loop. I proved a lower bound on that compounding (Theorem 1) with per-module violation severities and cross-module coupling terms, then implemented thirteen benchmark sections (3D scene understanding through formal safety) plus a full-loop compound experiment. The repo (`11-cv-robotics-unified`) has synthetic data generators, YAML runners, 100+ pytest cases, and a script that fills the LaTeX paper from results JSON files so numbers are reproducible. Day to day I am fixing DGP and adapter bugs, re-running benchmarks 05–14 in full trial mode, finishing the compound experiment, and writing the JMLR-format manuscript. This is the research thread I am focused on right now.

Earlier work in the same program: Modules 01–10 of the ML Research Benchmark Suite (~33k lines of Python, 310 pytest cases) covering causal inference, Bayesian deep learning, offline/safe RL, generative modeling, graph ML, self-supervised learning, neurosymbolic reasoning, federated privacy, and scientific ML, each with oracle ground truth and violation knobs. Companion papers for modules 01–10 live in a shared `papers/` LaTeX workspace.

Other completed threads: EfficientNetV2B0 pneumonia classification on chest X-rays (~83% validation accuracy); URC-CV architecture report (sole author) for competition perception and control; SpaAIder (local multi-agent runtime with tiered memory); LLM-V1.0 (~30M-parameter GPT-style transformer trained from scratch). PhD interest: computer vision and robotics, especially closed-loop perception that stays reliable under outdoor shift. My URC rover stack is field testing in parallel and feeds examples for Module 11.

---

## Internship (combined — NASA)

I have completed five internships with the National Aeronautics and Space Administration (NASA), from 2024 through 2026: three consecutive mission-design placements; a Computer Engineer internship in 2025 (multiple terms); and a Lead Systems Engineer internship (2025–2026) spanning two engineering teams.

The three early placements were structured aerospace challenges with NASA-style concept development, requirements, and team deliverables on deadline. As Computer Engineer intern in 2025 I supported integration work, simulation, and milestone documentation on agency review schedules.

As Lead Systems Engineer at NASA I led engineering integration on two projects. In 2025 that was a lunar in-situ repair technology proposal: vacuum cold-welding parameters from ISS heritage and agency technical literature, quantitative performance requirements, the final proposal package, ROS 2/Gazebo simulation with structural checks, and service on a formal peer review panel scoring competing submissions. In 2026 it was a lunar permanently shadowed region volatile-prospecting rover, from mission concept review through preliminary design review: interface control architecture, subsystem requirements flow-down, command-and-data-handling ownership, thermal analysis across a 40 to 394 K envelope, and S-band downlink margin work. Much of the work was reconciling subsystem documentation before program manager review.

I co-authored or authored twelve NASA technical documents. In 2026, as Lead Systems Engineer on the lunar volatile-prospecting rover, those were the Mission Concept Review on autonomous volatile reconnaissance in permanently shadowed regions; the System Requirements Review on subsystem allocation and interface control architecture; the Mission Definition Review on mission architecture and operational paradigm for in-situ volatile characterization; the Preliminary Design Review on integrated vehicle baseline and verification matrix for a rover at Nobile Rim 2; the CDH Interface Document on command, telemetry, timing, and fault-response contracts; and the Thermal Subsystem Report on heat-flow analysis and MLI versus active-heating trades across the PSR thermal envelope.

In 2025, as Lead Systems Engineer on the lunar in-situ repair proposal, I co-authored the Final Proposal on solid-state cold-welding attachment for infrastructure salvage, the Quad Charts portfolio on three lunar ISRU and mobility concepts, and the Teaming and Workforce Development Section on competency matrices for technology infusion proposals. I was lead author on the L-MAP-FI Technical Presentation on multi-agent lunar pathfinding and environmental forecasting (ROS 2/Gazebo and structural validation). I was primary research author on the Technical Research Memorandum on vacuum cold-welding parameters for robotic lunar repair, drawing on ASTROBEAT ISS heritage and NTRS literature. I also wrote the sole-author Review Panel #6 evaluation, formally scoring technology proposals from three competing teams using NASA structured review criteria.

### Internship — split option A (Lead Systems Engineer, NASA)

Lead Systems Engineer intern at the National Aeronautics and Space Administration from 2025 through 2026. I delivered six milestone reports on a lunar volatile-prospecting rover in 2026 and six proposal and review documents on a lunar in-situ repair technology study in 2025, including lead authorship on L-MAP-FI, primary research authorship on the cold-welding memorandum, and sole authorship on a formal peer evaluation for Review Panel #6.

### Internship — split option B (Computer Engineer, NASA)

Computer Engineer intern at the National Aeronautics and Space Administration, 2025, multiple terms: integration support, milestone deliverables, simulation and documentation alongside subsystem leads.

### Internship — split option C (mission-design placements, NASA)

Three consecutive NASA mission-design internships (2024–2025): aerospace scholar-style mission challenges, concept development, and team deliverables under agency review structure.

---

## Optional — USC MESA (Other activity / Social Consciousness)

Since 2024 I have mentored MESA students trying to break into research: reading papers, writing proposals, presenting without freezing, and navigating graduate school applications. The work is mostly about making the research path legible. That path was not obvious to me early on either.

---

## Rewrite notes (avoid-ai-writing pass)

Issues fixed: em dashes removed; negative-parallel constructions trimmed; hollow intensifiers cut; varied openers; technical terms kept where load-bearing.

Latest edit: NASA section lists all 12 technical documents by title and year.
