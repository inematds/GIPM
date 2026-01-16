# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GIPM (Método de Criação de Projetos com IA) is a methodology framework for building AI-driven projects with governance, auditability, and scalability. The project defines how to conceive, build, govern, and evolve projects where AI is a controlled component rather than the decision-maker.

## Core Methodology Principles

The method follows these invariant principles:
1. **API-first** - All capabilities exposed via APIs
2. **Backend orchestrates, AI executes** - AI never controls flow
3. **Two-phase rule** - AI generates structure, system generates artifacts
4. **Total persistence** - Everything is stored and auditable
5. **Modularity and anti-lock-in** - Components are replaceable

### Three-Layer Architecture

1. **Human Decision Layer** - Defines objectives, limits, success criteria (never delegated to AI)
2. **System Layer (Orchestration)** - Validates states, controls flow, applies rules
3. **AI Layer (Cognition)** - Analyzes, structures, synthesizes (never controls flow)

## Project Structure

```
GIPM/
├── .bmad-core/           # BMad Method configuration and workflows
│   ├── agents/           # Specialist agent definitions (analyst, architect, dev, etc.)
│   ├── tasks/            # Task definitions for the method
│   ├── templates/        # Document templates (PRD, architecture, stories)
│   ├── workflows/        # Greenfield/brownfield workflow definitions
│   └── core-config.yaml  # Project configuration
├── doc/                  # Method documentation
│   └── metodo_de_projetos_com_ia_versao_1.md  # Core method definition (v1.2)
├── ref/                  # Reference implementation docs (Dashboard Mastery example)
└── .claude/commands/BMad/  # Claude Code slash commands for BMad agents/tasks
```

## BMad Method Integration

This project uses BMad Method for AI-assisted project orchestration.

### BMad Orchestrator (`/BMad:agents:bmad-orchestrator`)

The **BMad Orchestrator** is the master coordinator that provides a unified interface to all BMad capabilities. Its role:

- **Workflow Coordination** - Guides users through greenfield/brownfield workflows
- **Agent Transformation** - Dynamically transforms into any specialist agent on demand
- **Resource Loading** - Loads agents, tasks, templates only when needed (lazy loading)
- **State Tracking** - Tracks current context and guides to next logical steps

**Orchestrator Commands** (all prefixed with `*`):
- `*help` - Show available commands, agents, and workflows
- `*agent [name]` - Transform into a specialist agent
- `*workflow [name]` - Start a specific workflow
- `*workflow-guidance` - Interactive workflow selection
- `*task [name]` - Execute a specific task
- `*status` - Show current context and progress
- `*kb-mode` - Load BMad knowledge base for methodology questions

### Specialist Agents

Access via `/BMad:agents:<name>` or `*agent <name>` when in Orchestrator mode:

| Agent | Role | Key Deliverables |
|-------|------|------------------|
| `analyst` | Business Analyst | Requirements, user research, PRD |
| `architect` | Software Architect | System design, tech stack, architecture docs |
| `dev` | Developer | Code implementation, story execution |
| `pm` | Project Manager | Planning, timelines, risk management |
| `po` | Product Owner | Backlog, prioritization, acceptance criteria |
| `qa` | QA Engineer | Test plans, quality gates, validation |
| `sm` | Scrum Master | Sprint planning, ceremonies, process |
| `ux-expert` | UX Designer | User experience, UI patterns, design systems |
| `bmad-master` | BMad Expert | Deep methodology questions, customization |

### Workflows

Defined in `.bmad-core/workflows/`:

| Workflow | Purpose |
|----------|---------|
| `greenfield-fullstack` | New full-stack application from scratch |
| `greenfield-ui` | New frontend/UI application |
| `greenfield-service` | New backend service |
| `brownfield-fullstack` | Enhance existing full-stack app |
| `brownfield-ui` | Enhance existing frontend |
| `brownfield-service` | Enhance existing backend |

### Tasks

Common tasks available via `*task <name>`:
- `create-doc` - Create documents from templates
- `create-next-story` - Generate next user story
- `review-story` - Review and validate stories
- `qa-gate` - Execute quality gate checklist
- `document-project` - Generate project documentation

## Configuration

Key settings in `.bmad-core/core-config.yaml`:
- PRD and architecture documents use sharded structure (in `docs/prd/` and `docs/architecture/`)
- Stories location: `docs/stories/`
- QA files: `docs/qa/`

## Reference Implementation

The `ref/` folder contains documentation for "Dashboard Mastery" - a reference implementation demonstrating the method. Key standards:
- Uses Tailwind CSS with dark mode
- Three learning tracks (Fundamentos/Emerald, Técnicas/Blue, Avançado/Purple)
- Consistent component patterns documented in `FEP_STYLE_REFERENCE.md` and `LAYOUT_REFERENCE.md`

## Language

Project documentation is primarily in **Brazilian Portuguese**. Method concepts and principles should be maintained in Portuguese for consistency.
