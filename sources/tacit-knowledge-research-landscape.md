# Tacit Knowledge Capture in Manufacturing — Research Landscape
## Deep Dive for AI in Production Workshop (May 2026)

---

# 1. THE CRISIS: BY THE NUMBERS

The "Silver Tsunami" in manufacturing is not hypothetical — it's happening now:

- **70% of critical manufacturing knowledge is undocumented** — lives in workers' heads
- **52.4%** of industrial products workforce expected to retire or leave within 5 years (APQC)
- **3.8M manufacturing jobs** need filling by 2033; **2.8M** are direct retirement replacements
- **44% of machinists** are 56+; average age in small shops ~55
- Each retiring technician with 20+ years takes **~$800K-$1.2M in undocumented troubleshooting knowledge**
- Knowledge transfer failures cost large businesses **$47M/year** (Panopto)
- **$92B/year** lost in manufacturing to human-error-caused downtime (23% of all machine downtime)
- **3-4x longer repair times** when tribal knowledge is lost; **40% more repeat failures**
- New hire ramp: 3-4 months → **8-12 months** without knowledge transfer
- Fortune (Jan 2026): **"1-2 years left to capture decades of industrial knowledge"**
- California Management Review (Mar 2026): Tacit knowledge is **"your next competitive moat"**
- Only **9%** of companies leverage AI to capture expert knowledge; **92%** do not capture know-how at all

---

# 2. THEORETICAL FOUNDATIONS

## 2.1 The SECI Model Gets an AI Update (4 Competing Frameworks)

Nonaka's classic SECI model (Socialization → Externalization → Combination → Internalization) is being revised for the AI era:

| Framework | Authors/Year | Key Innovation |
|-----------|-------------|----------------|
| **GRAI** | Bohm & Durst, VINE 2025 | Extends SECI to 8 interaction fields (human×machine × 4 phases) |
| **GenAI SECI** | Uchihira, arXiv 2026 | "Digital Fragmented Knowledge" — AI synthesizes informal traces (photos, chat, sensor logs) into coherent knowledge |
| **HAC-SECI** | Matsumoto et al., Springer 2025 | Dual-loop: Inner (agent growth) + Outer (human development) — knowledge co-evolution |
| **AI-Augmented SECI** | ResearchGate 2025 | Maps AI technologies to each phase: empathetic AI → socialization, generative AI → externalization, cognitive graphs → combination, simulation AI → internalization |

## 2.2 Polanyi's Paradox Persists
"We can know more than we can tell" — and this remains the fundamental constraint. AI can capture **expressible tacit knowledge** (heuristics, rules of thumb) but struggles with **deeply embodied, context-dependent skill** (the "feel" of a machine vibration, the "sound" of a properly running system).

Key 2026 position paper: Liu et al. — "Reliable AI Needs to Externalize Implicit Knowledge" (arXiv:2605.02010) — proposes **Knowledge Objects (KOs)** as structured artifacts that externalize implicit knowledge into inspectable, verifiable, endorsable forms.

## 2.3 The Apprenticeship Paradox
Ide (arXiv, 2026): In a formal economic model, **entry-level automation can increase output on impact but reduce long-term growth** by disrupting the apprenticeship pipeline through which tacit knowledge is transmitted. AI co-pilots may weaken novices' incentives for hands-on learning.

---

# 3. WHAT ACTUALLY WORKS: EMPIRICALLY VALIDATED SYSTEMS

## 3.1 Academic Research (Strongest Evidence)

| Paper | Approach | Key Result | Maturity |
|-------|----------|------------|----------|
| **Kernan Freire et al. (TU Delft, 2024)** | LLM Q&A from factory docs + expert knowledge | Works, but **workers still prefer human experts** | Factory-evaluated |
| **Kernan Freire & Wang (CHI 2023)** | Voice/text assistant with data visualization for reflective prompting | Elicits expressible tacit heuristics from shop-floor workers | Factory prototype |
| **Zuin et al. (IJCNN 2025)** | LLM agent iteratively interviews employees; SI diffusion model | **94.9% full-knowledge recall** in simulation | Research prototype |
| **Radhakrishnan (Aarhus, 2025)** | Conversational AI (Gemini 2.5 Pro) → BPMN diagrams | Accurate process model in **12-minute session**, SME-friendly costs | Proof-of-concept |
| **Horner et al. (FAU Erlangen, CSCW 2022)** | Design Science Research: tacit knowledge → digital assistance system | Standardized capture method; worker co-design critical for acceptance | Factory-evaluated |
| **Guo & Hu (2026)** | GenAI-augmented apprenticeship (50-person experiment) | **15-22% performance improvements** (expressiveness, verbal, learning) | Controlled experiment |
| **LLM-ACTR (AAAI 2025)** | Cognitive architecture (ACT-R) → latent representations → LLM adapters | Better decision-making representations than LLM-only on Design for Manufacturing | Research |
| **GOFAI meets GenAI (2025)** | LLM → Prolog expert systems; Claude Sonnet + GPT-4.1 | Fully interpretable, auditable, correctable symbolic output | Research |
| **PKAI (Springer BISE, 2025)** | Multi-agent system for process knowledge acquisition; 19 design requirements | Operationalizes SECI phases through specialized LLM agents | Theoretically grounded |

**Recurring finding:** Workers prefer humans when available. AI works as **supplement**, not replacement.

## 3.2 Key German Research (Directly Relevant to Workshop)

| Group | Focus | Status |
|-------|-------|--------|
| **Fraunhofer IESE** (your workshop co-organizers) | Deployed AI assistants for knowledge capture in pumps, crane systems, switch cabinet construction | **Deployed** |
| **FAU Erlangen** (Horner et al.) | Knowledge-based assistance from tacit expertise | Published (CSCW 2022) |
| **German manufacturing survey** (Computers, MDPI, May 2026) | Two-round survey of German manufacturers: KM perceived as highly relevant but incompletely implemented; 24 requirements derived | Empirical field study |

---

# 4. COMMERCIAL LANDSCAPE (17+ Products/Startups)

## 4.1 Dedicated Tacit Knowledge Startups (2024-2026 Wave)

| Company | Location | Raised | Approach | Key Customers | Results |
|---------|----------|--------|----------|---------------|---------|
| **Interloom** | Munich | $16.5M | "Context graphs" of operational decision patterns | VW, Commerzbank, Zurich Insurance | Live deployments |
| **Blockbrain** | Stuttgart | €17.5M Series A | Industrial "Knowledge Bots" | Bosch, Kärcher | Won Siemens Industrial AI Award |
| **Murray Mentor** | Indiana | Seed | Voice-first "digital apprenticeship", real-time in-ear guidance | F&B, automotive, chemicals | Reduced training cycles |
| **Datch** | — | $15M | Voice-visual AI for industrial environments | ConEd, ABB Robotics, Singapore Airlines | — |
| **Tribalize AI** | — | — | Structured assessment → extraction → custom tool generation | — | V2.0 |
| **Dovient** | — | — | Multi-modal (video, photos, voice) → structured SOPs | — | Diagnosis: **25 min → 90 sec** |
| **IntuigenceAI** | Berkeley | $10M seed | CV + LLM; P&IDs → knowledge graphs | — | **81% pass rate** on PE exams (vs. ChatGPT ~10%) |
| **WorkCell AI** | — | — | AI accumulates knowledge from operator interactions | — | Designed for 10-200 person shops |

## 4.2 Connected Worker Platforms (Mature, At Scale)

| Platform | Scale | Approach |
|----------|-------|----------|
| **MaintainX** | $254M raised, $2.5B valuation, 11K+ customers | CMMS + knowledge capture |
| **Poka** | 2,300+ customers (Nestlé, Mars, Bosch, L'Oréal, Tetra Pak) | Connected worker + video SOPs |
| **Augmentir** | Frost & Sullivan 2023 Company of Year | Only "AI-native" platform; GenAI + agentic AI |
| **Tulip** | — | No-code manufacturing apps |
| **Tractian** | — | AI CMMS; tribal knowledge → standardized workflows |
| **OxMaint** | — | Voice-to-work-order + LLM knowledge capture |

**OxMaint results:** 80-95% field expertise preserved, 60-75% faster problem resolution, 40-55% reduction in training time.

## 4.3 Enterprise/Big Tech

| Company | System | Approach |
|---------|--------|----------|
| **Siemens** | Industrial Foundation Model | Trained on 150PB of engineering data; partnerships with Blockbrain/Dirac |
| **SAP** | "Company Memory" context graph | Agentic AI for manufacturing (Hannover Messe 2026) |
| **Microsoft** | Copilot for Manufacturing | Shift handoff structuring, knowledge retention |
| **IBM** | Maximo 9.1 + watsonx.ai | Generative assistant that learns from technician interactions |
| **Honeywell** | Forge | KG capturing "intuition of seasoned maintenance technicians" |
| **Toyota** | "Battery Brain" / "Gear Pal" / "Project Cura" | LangChain + LlamaIndex, custom ingestion, "Prompt Guardian" |

## 4.4 Knowledge Management Platforms

| Platform | Key Result |
|----------|------------|
| **Squirro** (acquired Synaptica) | Speech-to-graph pipeline for exit interviews → KG; explicitly designed as agent memory |
| **eGain** | Mid-size utility: **$4.2M annual productivity improvement**, **35% error reduction** |
| **Sugarwork** (acquired by Decidr, Nov 2025) | Expert-learner video conversations; **70% onboarding reduction** at Appen |
| **Starmind** | Real-time expertise maps from corporate data; customer: Mondelēz |
| **Glean** | Saves **36 hours/employee** during onboarding |

---

# 5. TAXONOMY OF APPROACHES

| Approach | Method | What It Captures | What It Misses | Maturity |
|----------|--------|-----------------|----------------|----------|
| **Interview-to-KG** | Exit interviews → NLP → knowledge graph | Decision reasoning, context | Embodied skill, timing | Deployed (Squirro, Sugarwork) |
| **Dialogue-to-Process** | Conversational AI → BPMN/SOP | Procedures, decision points | Physical intuition | Prototype → Early commercial |
| **Voice/Video-to-SOP** | Multi-modal capture → structured instructions | Step sequences, tool use | The *why* behind decisions | Deployed (Dovient, Augmentir, OxMaint) |
| **Observation-to-Procedural** | AI watches production data, learns patterns | Process variations, anomalies | Expert reasoning | Deployed (WorkCell, UptimeAI) |
| **Document-to-Semantic** | LLM ingests docs/manuals/tickets | Explicit documented knowledge | Undocumented heuristics | Deployed (Glean, Korra) |
| **Expert-Learner Pairing** | AI mediates veteran-junior conversations | Contextual transfer, mentoring | Scale limitations | Deployed (Sugarwork) |
| **Passive Monitoring** | AI monitors interactions/chats/tickets | Knowledge exchanges, expertise maps | Deep procedural knowledge | Deployed (eGain, Starmind) |
| **Agent-Based Discovery** | LLM agents iteratively interview employees | Organizational knowledge topology | Embodied/contextual skill | Research (Zuin et al.) |
| **Cognitive Architecture** | ACT-R/Soar + LLM for decision modeling | Cognitive decision processes | Physical skill | Research (LLM-ACTR) |
| **Wearable Sensors + ML** | IMUs + deep learning → motion patterns | Expert movement patterns, ergonomics | Cognitive reasoning | Technically mature |

---

# 6. THE CRITICAL GAP: NO EPISODIC-TEMPORAL MEMORY

This is where your agentic memory research connects powerfully:

**Every commercial system captures knowledge as static artifacts** (documents, SOPs, KG triples, video clips). None implement:

1. **Episodic memory** — "That one time the bearing failed because of the humidity after the weekend shutdown in July 2023" — specific events with full context
2. **Temporal versioning** — "We used to set the pressure at 4.2 bar, then changed to 3.8 in March 2024 when we switched to the new polymer, but went back to 4.0 in September because..."
3. **Knowledge decay modeling** — tracking when captured knowledge becomes outdated
4. **Experiential learning** — an agent that actually improves its manufacturing knowledge through accumulated episodes

**The parallel to your SE findings is striking:**
- SE production harnesses: ALL lack episodic memory and temporal versioning
- Manufacturing knowledge systems: ALL lack episodic memory and temporal versioning
- The episodic-temporal paradox is domain-independent

**Squirro comes closest** — their speech-to-graph pipeline for exit interviews is explicitly designed as "foundational memory for AI agents." But it's still a static capture → graph pipeline, not a living episodic memory system.

---

# 7. THE PAPER ANGLE: MEMORY-ENABLED KNOWLEDGE VESSELS

## The Core Argument

Current approaches to tacit knowledge capture in manufacturing treat it as a **documentation problem** — extract knowledge from experts, store it as static artifacts (SOPs, KGs, videos), retrieve when needed.

We argue it should be treated as an **agent memory problem** — create agents with episodic, semantic, procedural, and temporal memory that:

1. **Absorb** tacit knowledge incrementally through ongoing interaction with experts (not one-shot exit interviews)
2. **Contextualize** knowledge episodically (when, where, why, under what conditions)
3. **Version** knowledge temporally (how practices evolved, what invalidated old approaches)
4. **Transfer** knowledge to new workers through contextualized retrieval (not just "here's the SOP" but "here's what happened last time someone tried this under similar conditions")
5. **Evolve** their knowledge through continued production experience after the expert retires

This reframes the agent from a **knowledge retrieval system** to a **knowledge vessel** — a persistent entity that carries and grows manufacturing expertise over time.

## Evidence Base
- **The crisis is real:** $92B/year, 70% undocumented, 1-2 years to act (Fortune)
- **Current solutions capture procedures, miss experience:** Video-to-SOP works for steps, but misses the *why* and *when*
- **Workers prefer humans:** (TU Delft finding) — because humans provide *contextual, episodic* knowledge, not just procedures
- **The memory gap exists in all agent systems:** Your 10-harness survey + 70-paper survey demonstrates this
- **Manufacturing has unique memory requirements:** Safety-critical, real-time, multi-modal, regulatory
- **No manufacturing memory benchmark exists:** Research opportunity

## Why This Is Novel
1. No paper connects the agent memory literature (CoALA framework, Mem0, Zep, etc.) to the manufacturing tacit knowledge problem
2. No paper identifies the episodic-temporal gap as the reason current knowledge capture systems fall short
3. The "knowledge vessel" framing (agent as persistent carrier of expertise) is new
4. The cross-domain analysis (SE gaps = manufacturing gaps) is new

---

# 8. FRAUNHOFER IESE CONNECTION

**Your workshop co-organizers (Siebert, Trendowicz) are at Fraunhofer IESE**, which has:
- Already deployed AI assistants for knowledge capture in pumps, crane systems, switch cabinet construction
- Direct experience with the tacit knowledge problem in German manufacturing SMEs
- This makes the topic directly relevant to the organizers' own research

For the **AI in Production** workshop (Uni Bamberg), the connection is through:
- **Ute Schmid** (organizer) works on explainable/interactive AI — relevant to knowledge elicitation
- **Jakob Wagner (BMW)** — BMW faces exactly this knowledge retention challenge at scale
- The workshop's focus on "Agentic Systems in Manufacturing" directly encompasses memory-enabled knowledge agents

---

# 9. KEY REFERENCES

## The Crisis
- Edwards et al. (MIT, 2026). "Agentic AI in Engineering and Manufacturing." arXiv:2604.09633
- California Management Review (Mar 2026). "Tacit Knowledge Is Your Next Competitive Moat"
- Fortune (Jan 2026). "1-2 years left to capture decades of industrial knowledge"
- Ide (2026). "Automation, AI, and Intergenerational Transmission of Knowledge." arXiv:2507.16078

## Theoretical Foundations
- Bohm & Durst (2025). GRAI Framework (SECI → AI). VINE Journal
- Uchihira (2026). GenAI SECI Model. arXiv:2603.21866
- MDPI (2025). "Unveiling the Unspoken: AI-Enabled Tacit Knowledge Co-Evolution"
- Liu et al. (2026). "Reliable AI Needs to Externalize Implicit Knowledge." arXiv:2605.02010

## Empirically Validated Systems
- Kernan Freire et al. (TU Delft, 2024). "Knowledge sharing in manufacturing using LLMs." Frontiers in AI
- Kernan Freire & Wang (CHI 2023). "Tacit Knowledge Elicitation for Shop-floor Workers"
- Zuin et al. (IJCNN 2025). "LLMs for Tacit Knowledge Discovery." arXiv:2507.03811
- Radhakrishnan (2025). "Conversational AI: From Tacit Knowledge to BPMN." arXiv:2512.05122
- Horner et al. (CSCW 2022). "Tacit Expert Knowledge for Shop-floor Operators"

## Cognitive Architectures
- LLM-ACTR (AAAI 2025). "From Cognitive Models to LLMs in Manufacturing"
- Wu et al. (SAGE, 2025). "Cognitive LLMs for Manufacturing Decision-Making"
- PKAI (Springer BISE, 2025). "LLMs for Process Knowledge Acquisition"

## German Manufacturing Context
- MDPI Computers (May 2026). "KM in Manufacturing: Current Practices, Barriers, and Automation Potential"
- Fraunhofer IESE — deployed AI assistants for industrial knowledge capture
- Blockbrain (Stuttgart, €17.5M) — Bosch, Kärcher
- Interloom (Munich, $16.5M) — VW

## Agent Memory (Your Existing Work)
- MemAgents workshop papers (70 papers analyzed)
- LoCoMo-Plus benchmark (35-45pp factual-to-cognitive gap)
- 10 production harness survey (all lack episodic memory)
