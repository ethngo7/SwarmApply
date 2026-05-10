# SwarmApply (AI Hackathon Submission) 🐝

> One prompt. Full job search, automated.

SwarmApply is a multi-agent career automation swarm built on 
[OpenSwarm](https://openswarm.com). Instead of spending 45 minutes 
per application researching companies, tailoring resumes, finding 
recruiters, and writing cold emails — SwarmApply does all of it 
autonomously with a single prompt.

## Demo

![Job Search](https://raw.githubusercontent.com/ethngo7/swarmapply/main/screenshots/subagents-working.png)
![Agents Running](https://raw.githubusercontent.com/ethngo7/swarmapply/main/screenshots/Custom-modes.png)
![Cold Email Output](https://raw.githubusercontent.com/ethngo7/swarmapply/main/screenshots/agent-in-Gmail.png)

## How It Works

One prompt triggers a coordinated swarm of 5 specialized AI agents:

## Agents

| Mode | Role |
|------|------|
| Orchestrator | Master controller — sequences and spawns all sub-agents |
| Job Searcher | Browses Wellfound, LinkedIn, Indeed for matching roles |
| Resume Tailor | Rewrites resume bullets to match the specific job description |
| Email Hunter | Finds the real recruiter or hiring manager's email |
| Cold Email Drafter | Writes a personalized <100 word cold email |

## Setup

### Prerequisites
- [OpenSwarm](https://openswarm.com) installed
- Anthropic API key or Claude Pro account
- Google Workspace connected in OpenSwarm Actions (for Gmail)

### Installation
1. Clone this repo
2. Open OpenSwarm
3. Go to **Modes** → create 5 new Modes
4. Copy-paste each prompt from the `/modes` folder
5. Spawn one **Orchestrator** agent on your canvas
6. Type your job search query and let it run

## Tech Stack
- [OpenSwarm](https://openswarm.com) — multi-agent orchestration
- Claude Sonnet 4.6 — powers all agents
- Google Workspace MCP — Gmail draft integration

## Roadmap
- [ ] Fix Gmail draft saving via MCP
- [ ] Add Follow Up agent
- [ ] Add Interview Prep agent
- [ ] Add Negotiate agent
- [ ] Resume stored as reusable Skill
- [ ] Auto-apply to Workday/Greenhouse
- [ ] InsForge backend for application tracking
- [ ] Zeabur deployment for one-click sharing

Built at **Build Smth AI-Native Hackathon @Cal** — May 2026

**Sponsors:** [OpenSwarm](https://openswarm.com) · [Retell](https://retellai.com) · [InsForge](https://insforge.com) · [Zeabur](https://zeabur.com) · [Entelligence AI](https://entelligence.ai) · [PixVerse](https://pixverse.ai) · [Klarity Health](https://klarity.health)

## Author
[Ethan Ngo](https://github.com/ethngo7)
