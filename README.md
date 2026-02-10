# DEXSPINE from Dex RoboKnix

### Cognitive Infrastructure for the Post-Training Era

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](https://github.com/DexRoboKnix/Dex_RoboKnix/releases)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

---

## Introduction

**DEXSPINE** is a rigid cognitive extraction protocol that forces Large Language Models to produce complete, structured analyses across 114 nodes and 6 architectural layers. Driven by the **DEX838 framework**, it eliminates hallucination in structural audits through mathematical constraints: **8 Plan + 3 MVE + 8 Execute = 19 nodes per layer × 6 layers = 114 total nodes**.

This is not a prompt. This is a protocol.

Created by **Dex RoboKnix** (typically known as Dan Cheeseman), DEXSPINE emerged from eight years of debugging complex enterprise systems in FinTech and Higher Education. When traditional prompting failed to deliver consistent, complete architectural documentation, the answer wasn't better prompts—it was enforcing structure before content. DEXSPINE transforms LLMs from conversational tools into deterministic extraction engines.

---

## What is DEX?

**DEX** (Data EXtraction) is the foundational framework and query language that powers DEXSPINE. Think of it as the syntax of structured thought—a bidirectional ladder that connects abstract values to concrete patterns.

### The 8:3:8 Law

The universal constant preventing cognitive drift. Every unit of analysis breaks down into exactly **19 nodes**:

**8 PLAN Nodes** — The Logic

- Definition, Purpose, Scope, Stakeholders, Success, Dependencies, Constraints, Metrics

**3 MVE Nodes** — The Essence

- **VA** (Value Essence): Keywords and driving forces
- **HU** (Human Insight): Lived experience and wisdom
- **LLM** (Pattern): Machine-recognizable structure

**8 EXECUTE Nodes** — The Action

- Approach, Tools, Workflow, Artifacts, Quality, Monitoring, Rollback, Improvement

This mathematical constraint is enforced structurally, not conversationally. The LLM cannot hallucinate layer 7. It cannot skip nodes. The structure is deterministic.

### The Six Layers

DEXSPINE forces every subject through 6 mandatory architectural layers:

1. **VALUES** — WHY it matters (fundamental essence)
2. **PRINCIPLES** — RULES to follow (governing laws)
3. **POLICY** — DECISIONS made (enabling constraints)
4. **PROCESS** — HOW it flows (end-to-end workflow)
5. **PROCEDURE** — STEPS to take (ordered actions)
6. **PATTERN** — REUSABLE templates (abstracted structures)

**Total: 6 layers × 19 nodes = 114 data points**

### The DEX Query Syntax

```javascript
// Full extraction (The Spine)
dex(full)["Subject"]

// Partial extraction (The Scan)
dex(values, plan)["Subject"]

// Context-aware extraction
dex(full, @context.md)["Subject"]
```

DEX is **markdown native**—written in markdown, generates markdown, validated by markdown. Zero install. Zero dependencies. Completely portable.

---

## Who is Dex RoboKnix?

**Dex RoboKnix** _(The K is silent — pronounced "Dex Row-bonix")_ is both a person and a philosophy.

**The Person:** Dan Cheeseman, AI Operations Engineer with 8 years engineering reliability across FinTech and Higher Education. Creator of DEXSPINE, DEX838, and the DEX framework. Specializes in root cause analysis, system architecture, and LLM-augmented operations.

**The Philosophy:** All data is valid. Transformation creates value. We build rigid tools to exploit fluid intelligence. We don't write prompts; we architect cognitive schemas that force probabilistic models to behave deterministically. In the post-training era, value emerges not from raw model output but from the transformation process itself—every layer (Values → Pattern) produces a capturable, version-controlled asset.

**The Mission:** Democratize cognitive architecture. Give everyone—researchers, engineers, analysts, students—the tools to extract deterministic structure from stochastic systems. Make the implicit explicit. Turn conversations into architecture.

---

## The Problem DEXSPINE Solves

LLMs excel at fluency but fail at rigor. Ask them to "analyze a system" and you get:

- **Inconsistent structure** — Different outputs every time
- **Arbitrary depth** — No way to know if analysis is complete
- **Missing connections** — Values disconnected from execution
- **Ghost nodes** — Things that exist in practice but lack stated purpose

Standard prompting produces _conversation_. DEXSPINE produces _architecture_.

---

## Empirical Validation

DEXSPINE has been tested across four frontier models on the subject "The Internet":

| Model                 | Structure | Content Depth | Token Output | Grade |
| --------------------- | --------- | ------------- | ------------ | ----- |
| **Claude Sonnet 4.5** | 114/114 ✓ | Excellent     | ~7,800       | A+    |
| **Gemini 3 Pro**      | 114/114 ✓ | Very Good     | ~4,200       | A     |
| **Grok**              | 114/114 ✓ | Very Good     | ~4,800       | A-    |
| **DeepSeek**          | 114/114 ✓ | Good          | ~3,800       | B+    |

**Key Finding:** When properly constrained by the protocol specification, all models produced mathematically correct outputs with zero layer drift.

See [full comparative analysis](./docs/ANALYSIS_REPORT.md) for detailed model performance breakdown.

---

## How It Works

### Input

```
dex(full)["The Internet"]
```

### Output Structure

```markdown
# LAYER 01: VALUES - The Internet

## PHASE 1: PLAN (8 nodes)

1. Definition: A global system of interconnected...
2. Purpose: To democratize access to information...
   ...

## PHASE 2: MVE (3 nodes)

1. VA: Decentralization. Openness. End-to-end principle.
2. HU: "Information wants to be free." - The lived experience...
3. LLM: [Graph: nodes={AS}, edges={BGP}, topology=mesh]

## PHASE 3: EXECUTE (8 nodes)

1. Approach: Maintain through multi-stakeholder governance...
   ...
   _DEXSPINE L0 — Filter Position 01 — 19/114 Nodes Complete_

# LAYER 02: PRINCIPLES - The Internet

...

# LAYER 06: PATTERN - The Internet

...
_DEXSPINE L0 — Filter Position 06 — 114/114 Nodes Complete_
```

**Result:** 8,000-11,000 tokens of structured cognitive architecture.

---

## Use Cases

### 1. System Audits — Find Ghost Nodes

```
dex(full)["Our Production Infrastructure"]
```

Reveals components that exist in execution (Layer 6) but have no defined purpose (Layer 1) or violate stated principles (Layer 2).

### 2. Architectural Decisions — Compare Approaches

```
dex(full)["Monolithic Architecture"]
dex(full)["Microservices Architecture"]
```

Side-by-side comparison across all 6 layers. Identify where Layer 3 (Policy) conflicts with Layer 5 (Procedure).

### 3. Organizational Alignment — Values → Code

```
dex(full)["Our AI Ethics Framework"]
```

Traceable path from abstract values (Layer 1) through concrete procedures (Layer 5) to reusable patterns (Layer 6). Ensures stated ethics are actually enforced.

### 4. Knowledge Transfer — Onboard Teams

```
dex(full)["Incident Response Process"]
```

Complete documentation from "why we do this" (Layer 1) to "exact steps to follow" (Layer 5). Junior engineers get checklists; seniors get architectural context.

### 5. Compliance Documentation — Regulation → Implementation

```
dex(full)["GDPR Compliance Program"]
```

Legal requirements (Layer 3 Policy) linked to actual procedures (Layer 5) and verification methods (Layer 4 Process). Audit-ready documentation.

---

## The Development Story

This protocol emerged from a simple observation: **LLMs lose count**.

In January 2026, while working as a Senior Support Analyst debugging complex FinTech systems, I noticed that LLM-generated documentation was inconsistent. Ask the same question twice, get different structures. No way to verify completeness.

The breakthrough came from root cause analysis training: _force structure first, then fill it_. If you mandate exactly 114 data points across 6 layers, the LLM can't drift. It becomes a deterministic extraction engine.

The protocol went through multiple iterations:

**Week 1 (Jan 2026):** Initial 6-layer concept  
**Week 2:** Added MVE phase for essence extraction  
**Week 3:** Formalized 8:3:8 law (mathematical constraint)  
**Week 4:** Multi-model testing (Claude, Gemini, Grok, DeepSeek)  
**Week 5:** Validation framework and failure mode recovery  
**Feb 2026:** Open source release with dual licensing

Every node name, every layer definition, every constraint was tested empirically. This isn't theoretical. It's battle-tested against frontier models.

---

## Installation & Usage

### Prerequisites

- LLM with ≥16k context window (Claude Sonnet 4.5, Gemini 3 Pro, or equivalent)
- Temperature: 0.0-0.2 (strict adherence mode)
- Extended thinking enabled (if available)

### Quick Start

**The beauty of DEXSPINE is its simplicity:** Attach the protocol file to your LLM chat, then use a single query.

1. **Upload the protocol file** to your LLM interface (Claude, ChatGPT, Gemini, etc.)

   - File: [`specs/DEXSPINE_Full_838.md`](./specs/DEXSPINE_Full_838.md)

2. **Execute with a single query:**

   ```
   dex(full)["Your Subject Here"]
   ```

3. **Validate output:**
   - 6 layers present? (not 5, not 7)
   - Each layer has 19 nodes? (8+3+8)
   - MVE includes LLM pattern node?
   - Total node count = 114?

That's it. No installation. No configuration. Just **attach + query**.

### Example Command (API Use)

For Claude API:

```bash
curl https://api.anthropic.com/v1/messages \
  -H "x-api-key: $ANTHROPIC_API_KEY" \
  -H "content-type: application/json" \
  -d '{
    "model": "claude-sonnet-4-5-20250929",
    "max_tokens": 12000,
    "temperature": 0.1,
    "messages": [{
      "role": "user",
      "content": "Execute DEXSPINE protocol on subject: Our Microservices Platform"
    }]
  }'
```

See [`/examples`](./examples) for complete working examples.

---

## Model-Specific Guidance

### Claude Sonnet 4.5 (Recommended)

- **Strengths:** Exceptional depth, production-ready documentation
- **Settings:** temp=0.1, max_tokens=12000
- **Best for:** Technical documentation, enterprise architecture
- **Output:** ~7,800 tokens of detailed analysis

### Gemini 3 Pro

- **Strengths:** Balanced speed/quality, excellent structure
- **Settings:** temp=0.1-0.15, safety=minimal
- **Best for:** Quick iterations, educational materials
- **Output:** ~4,200 tokens, efficient

### Gemini 3 Flash

- **Strengths:** 2-3x faster than Pro, 85% quality
- **Settings:** temp=0.1
- **Best for:** Rapid prototyping, cost-sensitive applications
- **Output:** ~3,500 tokens

See [Model Comparison Report](./docs/MODEL_COMPARISON.md) for detailed performance analysis.

---

## Advanced Techniques

### Recursive DEXSPINE (Zoom In)

```
Initial: dex(full)["API Security"]
Layer 5 says: "Implement OAuth2 flow"

Zoom In: dex(full)["OAuth2 Implementation Procedure"]
Result: Hypergranular 114-node extraction of OAuth2
```

### Comparative Analysis (Side-by-Side)

```
dex(full)["Current Architecture"]
dex(full)["Proposed Architecture"]

Compare layers 1-6 to identify:
- Value alignment (Layer 1)
- Principle conflicts (Layer 2)
- Policy trade-offs (Layer 3)
- Process complexity (Layer 4)
- Procedure differences (Layer 5)
- Pattern reusability (Layer 6)
```

### Diff Analysis (Evolution Tracking)

```
Q1 2026: dex(full)["Company Values"]
Q3 2026: dex(full)["Company Values"]

Track changes:
- Did values drift? (Layer 1)
- New principles added? (Layer 2)
- Procedures updated? (Layer 5)
```

### Bidirectional Framework Usage

**Decomposition (Top-Down):** Architecting a system from abstract Values down to concrete Patterns

```
dex(full)["New AI Compliance Policy"]
```

_Use when:_ Building something new, establishing governance, designing from first principles

**Recomposition (Bottom-Up):** Auditing a system from observable Patterns back up to Values

```
dex(full)["Legacy Codebase Architecture"]
```

_Use when:_ Understanding existing systems, finding ghost nodes, reverse-engineering decisions

---

## The Cyberpunk Edge

DEXSPINE embodies a cyberpunk philosophy: **build rigid tools to exploit fluid intelligence**.

In the post-training era, you don't own the model. You own the transformation process. DEXSPINE captures that process as a version-controlled, reusable asset. Every extraction becomes institutional knowledge. Every layer becomes a traceable artifact.

This is cognitive infrastructure for an age where intelligence is abundant but structure is scarce.

---

## License & Commercial Use

DEXSPINE is dual-licensed:

### Open Source: GNU AGPL v3

- ✅ Free for open source projects
- ✅ Free for internal business use
- ✅ Free for research and education
- ⚠️ **Network use requires source disclosure**

### Commercial License

- Required for SaaS/proprietary wrappers that don't disclose source
- Required for embedding in closed-source products
- Contact: daniel.cheeseman@me.com

**The AGPL Strategy:** If you build a SaaS tool using DEXSPINE and users interact with it over a network, you must open-source your entire backend OR purchase a commercial license. This ensures the community benefits or the creator gets compensated.

See [`COMMERCIAL_USE.md`](./COMMERCIAL_USE.md) for detailed explanation.

---

## Citation

If you use DEXSPINE in research or publications, please cite:

```bibtex
@software{cheeseman_dexspine_2026,
  author = {Cheeseman, Dan},
  title = {DEXSPINE: Universal Cognitive Extraction Protocol},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/DexRoboKnix/Dex_RoboKnix}},
  version = {1.0.0}
}
```

Or use the [`CITATION.cff`](./CITATION.cff) file for automatic citation generation.

---

## Project Structure

```
Dex_RoboKnix/
├── specs/
│   ├── DEXSPINE_Full_838.md          # Core protocol specification
│   └── DEXSPINE_v1.1_Specification.md # Enhanced version (next release)
├── examples/
│   ├── the_internet.md                # Reference implementation
│   ├── microservices.md               # Architecture example
│   └── incident_response.md           # Process example
├── docs/
│   ├── ANALYSIS_REPORT.md             # Multi-model testing results
│   ├── MODEL_COMPARISON.md            # Vendor-specific guidance
│   └── BEST_PRACTICES.md              # Production usage guide
├── tests/
│   └── validation_suite.md            # Protocol compliance tests
├── README.md                          # This file
├── COMMERCIAL_USE.md                  # Licensing FAQ
├── CITATION.cff                       # Academic citation
├── LICENSE                            # AGPL v3
└── CHANGELOG.md                       # Version history
```

---

## Roadmap

### v1.0.0 (Current - Feb 2026)

- ✅ Core 8:3:8 protocol
- ✅ Multi-model validation
- ✅ Empirical testing report
- ✅ Open source release

### v1.1.0 (Planned - Q2 2026)

- ⏳ Enhanced MVE quality standards
- ⏳ Failure mode recovery prompts
- ⏳ Subject type classification
- ⏳ Token budget guidance
- ⏳ Cross-layer validation automation

### v2.0.0 (Future)

- 🔮 API wrapper for programmatic access
- 🔮 Web interface for non-technical users
- 🔮 Integration with CI/CD pipelines
- 🔮 Diff engine for version tracking
- 🔮 Pattern library (common subjects)

---

## Contributing

We welcome contributions! Areas of interest:

1. **Testing** — Run DEXSPINE on new subjects, report results
2. **Examples** — Add industry-specific examples
3. **Integrations** — Build connectors (Notion, Confluence, etc.)
4. **Documentation** — Improve clarity, add tutorials
5. **Research** — Academic validation, formal verification

See [`CONTRIBUTING.md`](./CONTRIBUTING.md) for guidelines.

---

## FAQ

**Q: Is this just a fancy prompt?**  
A: No. It's a protocol with mathematical constraints. The 8:3:8 law is enforced structurally, not conversationally.

**Q: Why 114 nodes exactly?**  
A: 6 layers × 19 nodes per layer. This prevents hallucination—the LLM can't add layer 7 or skip nodes without breaking the constraint.

**Q: Can I use this commercially?**  
A: Yes, under AGPL v3 (with source disclosure) or commercial license (without disclosure). See [`COMMERCIAL_USE.md`](./COMMERCIAL_USE.md).

**Q: Which LLM works best?**  
A: Claude Sonnet 4.5 for depth, Gemini 3 Flash for speed. All tested models produced correct 114-node outputs.

**Q: How long does execution take?**  
A: 30-60 seconds for most subjects. Output is 8k-11k tokens.

**Q: What if my subject is abstract?**  
A: Execute phases describe conceptual instantiation. Example: For "Trust," Layer 5 describes _how trust is built_, not code.

**Q: Can I modify the protocol?**  
A: Yes (AGPL), but if you change the 8:3:8 structure, it's no longer DEXSPINE. Fork and rename.

**Q: What's the difference between DEX and DEXSPINE?**  
A: DEX is the framework and query language. DEXSPINE is the full 114-node extraction protocol. Think SQL (language) vs. a specific complex query (DEXSPINE).

---

## Support

- **Documentation:** [`/docs`](./docs)
- **Issues:** [GitHub Issues](https://github.com/DexRoboKnix/Dex_RoboKnix/issues)
- **Discussions:** [GitHub Discussions](https://github.com/DexRoboKnix/Dex_RoboKnix/discussions)
- **Commercial:** daniel.cheeseman@me.com
- **Website:** dex-roboknix.com _(coming soon)_

---

## Acknowledgments

Tested and validated by the AI research community. Special thanks to:

- Anthropic (Claude Sonnet 4.5)
- Google DeepMind (Gemini 3 Pro/Flash)
- xAI (Grok)
- DeepSeek (DeepSeek R1)

Built with obsessive attention to detail by humans who debug complex systems for a living.

---

## About the Creator

**Dan Cheeseman** / **Dex RoboKnix** _(The K is silent)_

AI Operations Engineer | Creator of DEXSPINE | DEX838 | DEX

8 years engineering reliability in FinTech and Higher Education. Specializes in root cause analysis, system architecture, and LLM-augmented operations. Created DEXSPINE to bring the rigor of incident response to cognitive extraction.

> _"All data is valid. Transformation creates value."_

- GitHub: [@DexRoboKnix](https://github.com/DexRoboKnix)
- LinkedIn: [Dan Cheeseman](https://linkedin.com/in/dan-cheeseman)
- Email: daniel.cheeseman@me.com

---

**Built by humans. Executed by machines. Validated by both.**

_DEXSPINE v1.0.0 from Dex RoboKnix - February 2026_
