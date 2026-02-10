# Contributing to DEXSPINE

Thank you for considering contributing to DEXSPINE! This document provides guidelines and information for contributors.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Process](#development-process)
- [Style Guidelines](#style-guidelines)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

---

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inclusive environment for all contributors, regardless of experience level, background, or identity.

### Expected Behavior

- Be respectful and considerate in communication
- Welcome newcomers and help them get started
- Focus on what is best for the community and the project
- Show empathy towards other community members
- Give and receive constructive feedback graciously

### Unacceptable Behavior

- Harassment, discrimination, or personal attacks
- Trolling, insulting/derogatory comments
- Publishing others' private information without permission
- Other conduct which could reasonably be considered inappropriate

### Enforcement

Violations can be reported to: danielcheeseman@me.com

---

## How Can I Contribute?

### 1. Testing & Validation

**What we need:**

- Test DEXSPINE on new subjects (systems, processes, concepts)
- Run protocol on local models (Llama 3, Mistral, Qwen, etc.)
- Identify edge cases that break the 114-node structure
- Validate cross-layer coherence

**How to help:**

1. Run `dex(full)["Your Subject"]` on your preferred model
2. Validate output using the checklist in `specs/DEXSPINE_Full_838.md`
3. Open an issue if:
   - Node count ≠ 114
   - Layers ≠ 6
   - Structure drifts
   - Cross-layer coherence breaks
4. Include subject, model, settings, and full output

**Example Issue Title:**

```
[Testing] Structure Drift on DeepSeek with Subject "Kubernetes"
```

---

### 2. Examples & Use Cases

**What we need:**

- Industry-specific examples (FinTech, Healthcare, EdTech, etc.)
- Process documentation (CI/CD, incident response, onboarding)
- Organizational architecture (governance, culture, values)
- Abstract concepts (trust, innovation, leadership)

**How to help:**

1. Run DEXSPINE on your chosen subject
2. Create file in `/examples/[category]/[subject].md`
3. Include metadata:
   ```markdown
   # DEXSPINE Extraction: [Subject]

   **Model:** Claude Sonnet 4.5
   **Temperature:** 0.1
   **Date:** 2026-02-10
   **Token Count:** ~8,200
   **Industry:** FinTech / Healthcare / etc.
   ```
4. Submit pull request with example

**Bonus:** If your example reveals ghost nodes, architectural conflicts, or other insights, add a "Key Findings" section.

---

### 3. Documentation

**What we need:**

- Tutorials for beginners
- Advanced techniques and patterns
- Integration guides (Langchain, LlamaIndex, etc.)
- Translations (non-English documentation)
- Video walkthroughs or screencasts
- Improved clarity in existing docs

**How to help:**

1. Identify documentation gaps
2. Write new content or improve existing
3. Follow style guidelines (see below)
4. Submit pull request to `/docs/[category]/[filename].md`

**High-Priority Docs:**

- "DEXSPINE for Beginners" tutorial
- Integration with popular frameworks
- Common pitfalls and troubleshooting
- Case studies from production use

---

### 4. Code & Tooling

**What we need:**

- API wrapper for programmatic access
- Web interface for non-technical users
- CI/CD integration plugins (GitHub Actions, GitLab CI)
- Diff engine for tracking evolution
- Validation automation
- Format converters (Markdown → JSON, YAML, etc.)

**How to help:**

1. Check existing issues tagged `enhancement` or `help wanted`
2. Comment on issue to claim it
3. Fork repository
4. Develop feature following style guidelines
5. Write tests if applicable
6. Update documentation
7. Submit pull request

**Tech Stack Preferences:**

- **API:** Python (FastAPI preferred), documented with OpenAPI
- **CLI:** Python or Node.js, follow POSIX conventions
- **Web:** React or Vue, minimize dependencies
- **CI/CD:** GitHub Actions preferred
- **Tests:** pytest for Python, Jest for JS

---

### 5. Research & Analysis

**What we need:**

- Formal verification of 8:3:8 structure
- Academic papers using DEXSPINE methodology
- Comparative studies (DEXSPINE vs other frameworks)
- Performance benchmarks across models
- Cognitive science analysis of layer architecture

**How to help:**

1. Conduct research using DEXSPINE
2. Publish findings (arXiv, conferences, journals)
3. Cite using `CITATION.cff`
4. Share preprint/final paper in an issue or PR
5. We'll link to your research from README

---

### 6. Bug Reports

**What we need:**

- Clear, reproducible bug reports
- Edge cases that break the protocol
- Model-specific failures
- Documentation errors

**How to report:**

1. Check if issue already exists
2. Open new issue with template:

   ```markdown
   **Bug Description:**
   [What went wrong?]

   **Subject:**
   [What subject were you extracting?]

   **Model:**
   [Which LLM? Version? Settings?]

   **Expected Behavior:**
   [What should have happened?]

   **Actual Behavior:**
   [What actually happened?]

   **Steps to Reproduce:**

   1. Step one
   2. Step two
   3. ...

   **Output:**
   [Paste relevant output or attach file]

   **Environment:**

   - OS: [Windows/Mac/Linux]
   - Model API/Local: [API or local install?]
   - Temperature: [0.0-1.0]
   - Max Tokens: [limit]
   ```

---

### 7. Feature Requests

**What we need:**

- Use cases not currently supported
- Quality-of-life improvements
- Integration ideas
- Tooling suggestions

**How to request:**

1. Open issue tagged `enhancement`
2. Describe the problem you're solving
3. Propose a solution (optional but helpful)
4. Explain impact: who benefits, how often, etc.

**Example:**

```markdown
**Problem:**
When running DEXSPINE on multiple subjects for comparison, there's no automated diff tool to highlight differences between layers.

**Proposed Solution:**
A CLI tool that takes two DEXSPINE outputs and generates a side-by-side diff, highlighting where layers diverge.

**Impact:**

- Architectural decision-making (compare approaches)
- Evolution tracking (same subject over time)
- Expected usage: ~50% of users doing comparative analysis
```

---

## Development Process

### Setting Up Your Environment

1. **Fork the repository:**

   ```bash
   gh repo fork dex-roboknix/dexspine-universal
   ```

2. **Clone your fork:**

   ```bash
   git clone https://github.com/YOUR-USERNAME/dexspine-universal.git
   cd dexspine-universal
   ```

3. **Create a branch:**

   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make changes and test:**

   - Follow style guidelines
   - Test thoroughly
   - Update documentation

5. **Commit and push:**

   ```bash
   git add .
   git commit -m "feat: your feature description"
   git push origin feature/your-feature-name
   ```

6. **Open Pull Request:**
   - Use PR template (provided)
   - Reference related issues
   - Request review

---

## Style Guidelines

### Markdown

- Use `#` headers (not underlines)
- Code blocks with language tags: ` ```python `
- Lists with `-` (not `*` or `1.`)
- Keep line length ≤100 characters where practical
- Use **bold** for emphasis, not _italics_ (unless quoting)
- Include TOC for docs >500 words

### Code

**Python:**

- Follow PEP 8
- Use type hints
- Docstrings for all functions (Google style)
- Max line length: 100 characters
- Use `black` for formatting

**JavaScript:**

- Follow Airbnb style guide
- Use ESLint
- Prefer functional components (React)
- Use Prettier for formatting

### Documentation

- **Audience:** Assume intermediate technical knowledge
- **Tone:** Professional but approachable (no jargon without definition)
- **Examples:** Always include concrete examples
- **Structure:** Problem → Solution → Impact pattern
- **Links:** Use relative links for internal docs

---

## Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

### Format

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

### Types

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation only
- `style`: Code style (formatting, no logic change)
- `refactor`: Code change (no feat/fix)
- `test`: Adding or updating tests
- `chore`: Maintenance (deps, config, etc.)

### Examples

**Good:**

```
feat(validation): add cross-layer coherence checker

Implements automated validation that checks whether Layer 5 procedures
actually implement Layer 4 processes.

Closes #42
```

**Bad:**

```
updated stuff
```

---

## Pull Request Process

### Before Submitting

- [ ] Code follows style guidelines
- [ ] Documentation updated (if applicable)
- [ ] Tests pass (if applicable)
- [ ] Changelog updated (under `[Unreleased]`)
- [ ] Commit messages follow convention
- [ ] Branch is up to date with `main`

### PR Template

```markdown
## Description

[What does this PR do? Why?]

## Type of Change

- [ ] Bug fix (non-breaking)
- [ ] New feature (non-breaking)
- [ ] Breaking change (fix/feature that changes existing behavior)
- [ ] Documentation update

## Related Issues

Closes #[issue number]

## Testing

[How did you test this? What models/subjects did you use?]

## Checklist

- [ ] My code follows style guidelines
- [ ] I have updated documentation
- [ ] I have added tests (if applicable)
- [ ] All tests pass
- [ ] I have updated CHANGELOG.md
```

### Review Process

1. **Automated Checks:** CI/CD runs (when implemented)
2. **Maintainer Review:** 1-2 maintainers review code
3. **Feedback:** Address any requested changes
4. **Approval:** Maintainer approves
5. **Merge:** Squash & merge to `main`

**Timeline:** We aim to review PRs within 5 business days.

---

## Community

### Communication Channels

- **GitHub Issues:** Bug reports, feature requests
- **GitHub Discussions:** Questions, ideas, show-and-tell
- **Email:** danielcheeseman@me.com (Code of Conduct issues)

### Getting Help

**New to open source?**

- Read [First Contributions](https://github.com/firstcontributions/first-contributions)
- Look for issues tagged `good first issue`
- Ask questions in GitHub Discussions

**Stuck on something?**

- Check existing issues and discussions
- Open a discussion with `[Question]` prefix
- Be specific: include context, what you've tried, and where you're stuck

### Recognition

Contributors are recognized in:

- `CONTRIBUTORS.md` (auto-generated from commits)
- Release notes (for significant contributions)
- README acknowledgments section (for major features)

---

## License

By contributing to DEXSPINE, you agree that your contributions will be licensed under:

- **Code & Documentation:** AGPL v3
- **Examples & Tests:** AGPL v3

You retain copyright on your contributions but grant an irrevocable license to the project.

---

## Questions?

- **General:** Open a GitHub Discussion
- **Security:** danielcheeseman@me.com
- **Licensing:** danielcheeseman@me.com
- **Commercial:** danielcheeseman@me.com

---

**Thank you for contributing to DEXSPINE!**

Your work helps make LLMs more reliable and structured. Every test, example, bug report, and PR matters.

_Last Updated: February 2026_
