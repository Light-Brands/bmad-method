# BMAD Method Interaction Guide

A quick-reference cheat sheet for developers working with the BMAD (Breakthrough Method of Agile AI-Driven Development) framework.

---

## Getting Started

| What You Want              | What to Say/Do                          |
| -------------------------- | --------------------------------------- |
| Get guidance anytime       | `/bmad-help`                            |
| Ask what to do next        | `/bmad-help what should I do next?`     |
| See available workflows    | `/bmad-help what can I do?`             |
| Install BMAD               | `npx bmad-method install`               |

> **When in doubt, run `/bmad-help`** — it detects what you've already done and recommends the right next step.

---

## Quick Flow (Bug Fixes & Small Features)

Three commands, start to finish:

1. **`/quick-spec`** (or `[TS]`) — Create a focused tech spec
2. **`/quick-dev`** (or `[QD]`) — Implement end-to-end
3. **`/code-review`** (or `[CR]`) — Validate quality

---

## Full Method — Phase by Phase

### Phase 1: Analysis (Optional)

| Command          | Shortcut    | What It Does                                     |
| ---------------- | ----------- | ------------------------------------------------ |
| `/brainstorm`    | `[BP]`      | 60+ ideation techniques with guided selection    |
| `/research`      | `[MR/DR/TR]`| Market, Domain, or Technical research            |
| `/create-brief`  | `[CB]`      | Capture strategic vision and MVP scope           |

### Phase 2: Planning

| Command              | Shortcut | What It Does                                        |
| -------------------- | -------- | --------------------------------------------------- |
| `/create-prd`        | `[CP]`   | Build Product Requirements Document via guided interview |
| `/create-ux-design`  | `[CU]`   | Create UX specifications and interaction design     |

### Phase 3: Solutioning

| Command                          | Shortcut | What It Does                                      |
| -------------------------------- | -------- | ------------------------------------------------- |
| `/create-architecture`           | `[CA]`   | Technical decisions, ADRs, system design           |
| `/create-epics-and-stories`      | `[CE]`   | Break PRD into implementable work units            |
| `/check-implementation-readiness`| `[IR]`   | Gate check — validates alignment before coding     |

### Phase 4: Implementation

| Command            | Shortcut | What It Does                                |
| ------------------ | -------- | ------------------------------------------- |
| `/sprint-planning` | `[SP]`   | Initialize sprint tracking (one-time setup) |
| `/create-story`    | `[CS]`   | Prepare next story with full context        |
| `/dev-story`       | `[DS]`   | Implement story code and tests              |
| `/code-review`     | `[CR]`   | Multi-faceted quality review                |
| `/automate`        | `[QA]`   | Generate API/E2E tests                      |
| `/retrospective`   | `[ER]`   | Epic-level lessons learned review           |

---

## Anytime Commands (Use in Any Phase)

| Command                      | Shortcut | What It Does                                    |
| ---------------------------- | -------- | ----------------------------------------------- |
| `/bmad-help`                 | —        | Context-aware intelligent guidance              |
| `/document-project`          | `[DP]`   | Analyze existing codebase, generate docs        |
| `/correct-course`            | `[CC]`   | Handle mid-sprint scope changes                 |
| `/party-mode`                | `[PM]`   | Multi-agent collaborative discussion            |
| `/create-diagram`            | —        | Excalidraw diagrams (flowcharts, wireframes, ERDs) |
| `/shard-document`            | `[SD]`   | Split large docs for token efficiency           |
| `/adversarial-review`        | `[AR]`   | Cynical, forced-criticism review                |
| `/editorial-review-prose`    | `[EP]`   | Copy editing                                    |
| `/editorial-review-structure`| `[ES]`   | Document structure optimization                 |

---

## Agent Personas

Each workflow is backed by a specialized agent persona:

| Agent             | Name    | Role                                              |
| ----------------- | ------- | ------------------------------------------------- |
| Product Manager   | John    | Requirements discovery, PRDs, stakeholder alignment |
| Business Analyst  | Mary    | Market research, brainstorming, product briefs    |
| System Architect  | Winston | Tech decisions, scalability, ADRs                 |
| Senior Developer  | Amelia  | Code implementation, test-first development       |
| Scrum Master      | Bob     | Sprint planning, story prep, retrospectives       |
| UX Designer       | Sally   | User experience, interaction design               |
| QA Engineer       | Quinn   | Test automation, API/E2E testing                  |
| Quick Flow Dev    | Barry   | Rapid end-to-end implementation                   |
| Tech Writer       | Paige   | Documentation specialist                          |
| BMad Master       | —       | Orchestrator across all agents                    |

---

## Party Mode (Multi-Agent Collaboration)

Start with **`/party-mode`** to bring all agents into one conversation. This is useful for:

- Big decisions with trade-offs
- Brainstorming sessions
- Post-mortems and retrospectives
- Cross-functional problem-solving

Exit with: `*exit`, `goodbye`, `end party`, or `quit`

---

## Typical Workflow Sequences

### New product or platform

```
/create-prd
/create-architecture
/create-epics-and-stories
/sprint-planning
/create-story
/dev-story
/code-review
(repeat /create-story -> /dev-story -> /code-review for each story)
/retrospective
```

### Existing codebase, small change

```
/document-project
/quick-spec
/quick-dev
/code-review
```

### Bug fix in known codebase

```
/quick-spec
/quick-dev
/code-review
```

### Not sure what to do

```
/bmad-help
```

---

## Slash Command Quick Reference

```
/bmad-help                      Get guidance on what to do next
/quick-spec                     Fast tech-spec for small changes
/quick-dev                      Implement quick spec
/brainstorm                     60+ ideation techniques
/create-brief                   Product brief (analysis phase)
/create-prd                     Product Requirements Document
/create-ux-design               UX design specifications
/create-architecture            Architecture and technical decisions
/create-epics-and-stories       Break PRD into implementable work
/check-implementation-readiness Gate check before coding
/sprint-planning                Initialize sprint tracking
/create-story                   Prepare story for dev
/dev-story                      Implement story code and tests
/code-review                    Validate code quality
/automate                       Generate tests (QA agent)
/retrospective                  Epic completion review
/correct-course                 Handle mid-sprint changes
/document-project               Analyze existing codebase
/party-mode                     Multi-agent collaboration
/create-diagram                 Excalidraw diagrams
/shard-document                 Split large docs
/adversarial-review             Forced-criticism review
/editorial-review-prose         Copy editing
/editorial-review-structure     Document structure optimization
```

---

## Key Best Practices

- **Start a fresh chat for each workflow** to avoid context limits.
- **`/bmad-help` is your first stop** — it detects context and guides you.
- Each phase produces documents that feed into the next phase (context engineering).
- Architecture docs prevent agent conflicts (e.g., one agent using REST while another uses GraphQL).
- For multi-epic projects, never skip the solutioning phase.
- Use `/document-project` before working on an existing codebase so agents understand your conventions.
- Use `/shard-document` on large docs to reduce token usage.
- Consider running `/adversarial-review` on critical specs — it forces genuine analysis instead of rubber-stamp approvals.

---

## Resources

- **Documentation**: [docs.bmad-method.org](http://docs.bmad-method.org)
- **Discord**: [discord.gg/gk8jAdXWmj](https://discord.gg/gk8jAdXWmj)
- **GitHub**: [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD)
- **YouTube**: [@BMadCode](https://youtube.com/@BMadCode)
