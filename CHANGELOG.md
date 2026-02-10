# Changelog

All notable changes to DEXSPINE will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned for v1.1.0
- Enhanced MVE quality standards with examples
- Failure mode recovery prompts
- Subject type classification guide
- Token budget guidance and warnings
- Cross-layer validation automation
- Model-specific optimization refinements

### Under Consideration
- API wrapper for programmatic access
- Web interface for non-technical users
- Integration examples (Langchain, LlamaIndex)
- Local model testing (Llama 3, Mistral, Qwen)
- Pattern library (pre-built common subjects)
- Diff engine for tracking evolution over time

---

## [1.0.0] - 2026-02-10

### Added - Initial Public Release

#### Core Protocol
- **8:3:8 Law Implementation** - Rigid mathematical structure (8 Plan + 3 MVE + 8 Execute = 19 nodes per layer)
- **6-Layer Architecture** - Values, Principles, Policy, Process, Procedure, Pattern
- **114-Node Extraction** - Complete cognitive architecture across all layers
- **MVE Phase** - Value Essence, Human Insight, LLM Pattern nodes for essence extraction

#### Validation Framework
- Multi-model empirical testing across Claude Sonnet 4.5, Gemini 3 Pro, Grok, and DeepSeek
- Structural compliance validation (100% across all tested models)
- Comprehensive analysis report comparing model performance
- Model-specific optimization guides for each tested platform

#### Documentation
- `DEXSPINE_Full_838.md` - Complete protocol specification
- `README.md` - Project overview, installation, usage examples
- `COMMERCIAL_USE.md` - Dual-license explanation and FAQ
- `CITATION.cff` - Academic citation metadata
- `ANALYSIS_REPORT.md` - Multi-model validation findings
- `MODEL_COMPARISON.md` - Vendor-specific guidance

#### Examples
- "The Internet" - Reference implementation (8,000+ tokens)
- Validation test suite for protocol compliance
- Usage patterns (system audits, comparative analysis, constitutional design)

#### Licensing
- GNU AGPL v3 for open source and internal use
- Commercial licensing option for proprietary/SaaS applications
- Copyright protection with brand attribution requirements

#### Repository Structure
- `/specs` - Protocol specifications
- `/examples` - Reference implementations
- `/docs` - Analysis reports and guides
- `/tests` - Validation suite

### Technical Specifications
- **Input Syntax:** `dex(full)["Subject"]`
- **Output Format:** Structured Markdown with 114 nodes
- **Token Range:** 8,000-11,000 tokens (subject-dependent)
- **Requirements:** LLM with ≥16k context window, temperature 0.0-0.2
- **Model Tiers:** S (Claude, Gemini Pro), A (Gemini Flash, Claude Haiku), B (older models)

---

## Version History Notes

### Versioning Strategy
- **Major (X.0.0)** - Breaking changes to core 8:3:8 structure or layer definitions
- **Minor (1.X.0)** - New features, enhanced validation, additional examples
- **Patch (1.0.X)** - Bug fixes, documentation improvements, typo corrections

### Breaking Change Policy
Changes to the 8:3:8 law or the 6-layer architecture would constitute breaking changes requiring a major version bump. We are committed to maintaining backward compatibility within the v1.x series.

### Release Cadence
- **Major releases:** As needed (infrequent, signaled well in advance)
- **Minor releases:** Quarterly (Q2, Q3, Q4 2026)
- **Patch releases:** As needed (bug fixes, doc improvements)

---

## How to Contribute to This Changelog

When submitting pull requests, please:

1. Add a brief description under `[Unreleased]` in the appropriate category:
   - `Added` for new features
   - `Changed` for changes to existing functionality
   - `Deprecated` for soon-to-be-removed features
   - `Removed` for removed features
   - `Fixed` for bug fixes
   - `Security` for vulnerability patches

2. Use this format:
   ```markdown
   - **Feature Name** - Brief description (#PR_NUMBER)
   ```

3. We'll move items from `[Unreleased]` to a versioned section upon release.

---

## Archive

### Pre-Release Development (2025-12 to 2026-01)
- Conceptual development and early testing
- Multi-model validation experiments
- 8:3:8 law formalization
- Layer definition refinement

---

**Maintained by:** Dan Cheeseman / Dex Roboknix  
**Repository:** https://github.com/dex-roboknix/dexspine-universal  
**License:** AGPL v3 + Commercial
