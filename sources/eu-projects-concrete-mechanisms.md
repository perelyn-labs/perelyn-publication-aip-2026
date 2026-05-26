# EU Projects & German Initiatives: Concrete Mechanisms for Tacit Knowledge
**Research Date:** May 19, 2026

---

## Key Finding: Despite 10+ years of EU/German funding, tacit knowledge capture remains fundamentally unsolved.

The Horizon Europe 2027 call (HORIZON-CL4-2027-02-DIGITAL-EMERGING-52) is the first funding instrument that explicitly asks for "capturing and formalising the knowledge which is dispersed and not explicit."

---

## 1. COGNIMAN (Horizon Europe, Grant 101058477)

**Architecture:** Layered digital twin with sensors, robotics, simulation, ML. Three-layer cognitive digital twin model (IJPR, Dec 2024): Ontology layer → Knowledge layer → Cognitive layer.

**What it captures:** Process parameters, sensor observations, machine states. NOT heuristic judgment, NOT embodied skills.

**Limitation:** "Cognitive" refers to computational reasoning about machine states, not capturing human cognition. Worker knowledge enters only through structured Q&A interfaces.

## 2. SatisFactory (H2020, Grant 636302, 2015-2017)

**Built:** AR glasses + gamified training platform + collaboration tools. Deployed at COMAU (automotive, Turin) and SUNLIGHT (batteries, Greece). >80% user satisfaction.

**What it captures:** Explicit procedural knowledge, collaborative patterns, training content. Workers had to articulate knowledge into the platform.

**Limitation:** No mechanism to observe expert behavior and automatically extract techniques/heuristics. Predates LLM era.

## 3. TEAMING.AI (H2020, Grant 957402, 2021-2024)

**Built:** BPMN2KG tool (open-source) converting BPMN process models into RDF knowledge graphs. Modular KG framework for human-AI teaming.

**What it captures:** Explicit process knowledge (via BPMN transformation), sensor-derived situational data, expert-derived decision rules formalized in ontologies.

**Limitation:** Knowledge must be explicitly modeled as BPMN diagrams or ontological rules. No automated extraction from worker behavior.

## 4. Ageing@Work (H2020, Grant 826299)

**Built:** AR remote collaboration (retired experts guide on-site novices), empathic virtual coach, adaptive workstations.

**What it captures:** Expert guidance in real-time, but does NOT store or systematize for later reuse.

**Limitation:** Knowledge transfer, not preservation. When the expert is unavailable, the system has no stored knowledge.

## 5. Fraunhofer IESE (Kaiserslautern) — MOST RELEVANT

**Built and deployed:** Dialogue-based AI assistants using generative AI for knowledge elicitation during work. Digital twin integration. Anti-hallucination safeguards.

**Deployed in:** Pump manufacturing, crane systems, switch cabinet construction.

**What it captures:** Experiential knowledge (Erfahrungswissen), diagnostic heuristics, edge-case machine behavior.

**Limitation:** Workers must verbalize knowledge. Embodied knowledge (feel, sound) cannot be captured through dialogue.

## 6. Fraunhofer IPA (Stuttgart)

**Built:** MonSiKo (3D-sensor adaptive assembly assistance), motion analysis (ML classifies hand/arm movements), data fusion for worker activity recognition.

**What it captures:** Worker movements and task progress, NOT worker knowledge.

**Limitation:** Can detect that experts move differently from novices, but cannot tell you what the expert knows that causes them to move that way.

## 7. Fraunhofer IPK (Berlin)

**Built:** ErgoJack (wearable exosuit for ergonomics), KIRA Pro (personalized training plans), context-based assistance systems.

**What it captures:** Body movement data, worker profiles. Delivers pre-encoded specialist knowledge, does NOT extract new knowledge.

**Limitation:** Sophisticated sensing for worker state, but no sensing for worker knowledge.

## 8. CONVERGING (Horizon Europe, Grant 101058521)

**Built:** Platform for reconfigurable production with autonomous agents. Multi-level AI cognition: Perceive → Reason → Adapt.

**What it captures:** Production system state and process data, not worker knowledge.

**Limitation:** Production optimization project, not knowledge preservation.

## 9. XR5.0 (Horizon Europe, Grant 101135209, ongoing)

**Built:** Cloud-based XR training platform with Human Digital Twins, remote expert guidance, AI-adapted training.

**What it captures:** Worker biometrics, skill profiles, ergonomic preferences. Expert guidance delivered in real-time.

**Limitation:** Knowledge delivery and training platform, not knowledge extraction. Unclear if guidance sessions are stored as persistent artifacts.

## 10. Horizon Europe 2027 Call (HORIZON-CL4-2027-02-DIGITAL-EMERGING-52)

**Budget:** EUR 30M total, EUR 4-6M per project, up to 5 projects. Stage 1 deadline: March 17, 2026. Stage 2: October 13, 2026.

**Key language:** "AI can enhance the value of the companies by capturing and formalising the knowledge which is dispersed and not explicit."

**Significance:** First EU call that explicitly frames the problem as AI-assisted capture of tacit/implicit knowledge at the workstation level.

---

## German BMBF Projects

### KI_eeper ("Know how to keep") — MOST RELEVANT BMBF PROJECT

**What:** Multimodal AI that "learns with all senses" to automatically store expert knowledge. Assistance system builds itself automatically during work process.

**Tested in:** Two SMEs. Published as open-access Springer book (Dec 2025).

**Key finding:** 80% of business-relevant knowledge is NOT documented. Heavy emphasis on sociotechnical approach / change management.

**Limitation:** Book focuses on organizational acceptance, suggesting technical system alone was insufficient. Prototype demonstrated feasibility but not production-readiness.

### Service Secretary (BMBF)

AI-supported knowledge management for technical service. Captures knowledge during repair/diagnosis, generates repair guidelines.

### KiWi-Pro (BMBF, DFKI Saarland)

**Notable:** Combines desktop recording (digital activities) + camera-based CV (manual work steps) into unified process documentation. One of the few that attempts to capture what workers actually do via observation.

---

## Cross-Cutting Gaps (NONE of these projects address):

1. **Embodied/sensory knowledge** — no project captures what operators feel, hear, or smell
2. **Automatic extraction from expert behavior** — only KiWi-Pro and Fraunhofer IPA attempt to learn from watching experts, neither extracts reasoning
3. **Episodic memory** — no temporal record of what happened, when, under what circumstances
4. **Knowledge experts cannot articulate** — all dialogue-based approaches depend on verbalization
5. **Long-term knowledge evolution** — knowledge captured as snapshot, not living resource
6. **Integration of knowledge types** — no unified representation combining procedural + heuristic + causal + embodied knowledge
