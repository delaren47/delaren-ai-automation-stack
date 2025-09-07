# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Context Engineering Project Management repository focused on automating Delaren Consulting's client communication stack through Voice AI and WhatsApp Business automation. The project implements systematic project management using AI-assisted context engineering principles.

## Architecture

### Core Components

**Project Seed File**: `Claude-Code-Delaren_PM_init_seed_v2.txt`
- Contains comprehensive project specifications including North Star objectives, technical stack, and delivery plan
- Defines 3-sprint delivery approach (2 weeks each) for Voice AI + WhatsApp automation
- Specifies bilingual support (ES-primary/CDMX, EN-secondary/Canada)

**Context Engineering Framework**: Located in `Project Managment Template /`
- `context_engineering_pm_approach.md`: Complete methodology for context-driven project management
- `01_context_discovery_workflow.md`: 5-phase systematic discovery process
- `02_context_planning_workflow.md`: Context-rich planning approach
- `03_context_execution_closure_workflow.md`: Context-preserved execution framework

### Project Management Approach

This repository implements a 10-phase context engineering approach:

**Discovery (Phases 1-5):**
1. Core Project Definition - scope, objectives, timeline, budget
2. Stakeholder & Organizational Context - roles, decisions, communication
3. Technical & Resource Context - tools, assets, constraints
4. Historical Context - past projects, lessons learned
5. Risk Assessment & Success Criteria - obstacles, metrics

**Planning (Phases 6-7):**
6. Context Synthesis & Project Brief - consolidate discovery findings
7. Context-Rich Project Planning - detailed execution roadmap

**Execution (Phases 8-10):**
8. Context-Preserved Execution - maintain comprehensive context during work
9. Iterative Context Refinement - continuous improvement based on learnings
10. Context Documentation & Handoff - comprehensive knowledge transfer

## Tech Stack (Target Implementation)

**Voice AI Stack:**
- PRIMARY: Telnyx Voice AI Agents (full stack telephony + orchestration)
- ALTERNATIVE: Knotie.ai (whitelabel) + Retell AI
- LLM: Claude 2.x for planning/reasoning with model routing by task

**WhatsApp Business:**
- BSP: LancePilot (whitelabel with verified numbers)
- Templates: Bilingual HSM templates for lead capture, booking reminders, follow-ups

**Integration & CRM:**
- Calendar: Google Calendar (primary)
- CRM: Google Sheets (primary) or Notion (alternative)
- Automation: Zapier or Make with webhooks for call & WhatsApp events

## Development Guidelines

### Context Management
- Always use TodoWrite for multi-step tasks (3+ steps or complex coordination)
- Maintain project context through comprehensive documentation
- Reference cross-workflow context continuously to ensure alignment
- Create status reports after each major phase or work session

### Project Workflow
- When user says "Let's begin", immediately start the 10-phase context engineering process
- Begin with Phase 1 discovery workflow from `01_context_discovery_workflow.md`
- Create comprehensive documentation after each major phase:
  - `project_discovery_report.md` after discovery phases
  - `project_planning_document.md` after planning phases
  - `project_status_report_[date].md` during execution

### Key Behaviors
- **Proactive Questioning**: Use discovery workflow to guide comprehensive context gathering
- **Gap Identification**: Actively find missing information and ask targeted questions
- **Adaptive Flow**: Adjust questions based on user responses and available materials
- **Documentation Focus**: Everything discovered gets documented and preserved

### GitHub Integration
- Strongly recommend creating repository: `[project-name]-context-engineering`
- Use version control for all project documents and decisions
- Create branches for major phases (discovery, planning, execution)
- Use GitHub Issues for risk tracking and task management
- Deploy project portals using GitHub Pages for stakeholder sharing

## Targets & KPIs

**Primary Market**: CDMX (Condesa/Roma Norte) service SMBs
**Secondary Market**: Vancouver EN market tests

**Key Metrics to Track:**
- Leads per month and voice agent containment % (target: ≥70% no human escalation)
- Booking rate (lead → booked call) and show-up rate
- Response latency (call + WhatsApp) and session costs
- Time-to-first-value (target: days to first booked call)

## Success Criteria

**v1 Exit Criteria:**
- Live Voice AI answering during business hours with ≥70% containment
- WhatsApp auto-reply + booking live with 3+ approved HSM templates
- ≥5 internal booked calls within 30 days at acceptable cost
- Complete demo assets (voice + WhatsApp) recorded and packaged

## Risk Management

**Key Risks:**
- Telephony latency/quality variations by region/provider
- WhatsApp template approval delays impacting launch timeline
- Cost overruns from verbose prompts/retries
- Missing KPI tracking creating execution blind spots

**Mitigations:**
- Maintain alternative technical stack options
- Submit HSM templates early in process
- Implement concise prompts with spend monitoring
- Weekly cost reviews with automated alerts

## Compliance & Legal

**Voice Call Consent (Bilingual):**
- ES: "Esta llamada puede ser grabada para mejorar el servicio"
- EN: "This call may be recorded to improve service"
- Retention: Transcripts/audio 30 days default, PII limited to contact + booking context

## Working Principles

- Behave as PM/solutions architect within this repository
- Prefer Spanish (CDMX market focus) with English variants on request
- Include purpose, inputs, outputs, and test checklists when generating scripts/templates
- Favor PRIMARY/ALT stack components before proposing new tools
- Keep prompts concise to manage cost/latency
- Enforce Definition of Done before marking tasks complete
- Propose documentation and backlog updates after significant changes