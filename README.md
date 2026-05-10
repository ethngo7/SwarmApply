# SwarmApply (AI Hackathon Submission) 🐝

> One prompt. Full job search, automated.

SwarmApply is a multi-agent career automation swarm built on 
[OpenSwarm](https://openswarm.com). Instead of spending 45 minutes 
per application researching companies, tailoring resumes, finding 
recruiters, and writing cold emails — SwarmApply does all of it 
autonomously with a single prompt.

## Demo

<div align="center">

<img src="https://raw.githubusercontent.com/ethngo7/SwarmApply/main/screenshots/subagents-working" width="800"/>
<p><em>Sub-agents working in parallel on the canvas</em></p>

<img src="https://raw.githubusercontent.com/ethngo7/SwarmApply/main/screenshots/Custom-modes" width="800"/>
<p><em>Custom Modes powering each specialized agent</em></p>

<img src="https://raw.githubusercontent.com/ethngo7/SwarmApply/main/screenshots/agent-in-Gmail" width="800"/>
<p><em>Agent autonomously composing a Gmail draft</em></p>

</div>

## How It Works

One prompt triggers a coordinated swarm of 5 specialized AI agents:

Example prompt: "find me the most compatible jobs within the SF Bay Area that require 0-2 years of experiences; open to new grads"

## Agents

| Mode | Role |
|------|------|
| Orchestrator | Master controller — sequences and spawns all sub-agents |
| Job Searcher | Browses Wellfound, LinkedIn, Indeed for matching roles |
| Resume Tailor | Rewrites resume bullets to match the specific job description |
| Email Hunter | Finds the real recruiter or hiring manager's email |
| Cold Email Drafter | Writes a personalized <100 word cold email |

See the [`/modes`](./modes) folder for all agent system prompts.

## Setup

### Prerequisites
- [OpenSwarm](https://openswarm.com) installed
- API keys or direct LLM account connections
- Google Workspace MCP connected (for Gmail)

### Installation

1. Download OpenSwarm
2. Go to **Modes** → create 5 new Modes
3. Copy-paste each prompt from the `/modes` folder, or create your own!!
4. Create one **Orchestrator** agent 
5. Type your job search query and let it run


## Further Improvements
- [ ] Fix Gmail draft saving via MCP
- [ ] Add Email Follow Up agent
- [ ] Add Interview Prep agent
- [ ] Resume stored as reusable Skill
- [ ] Auto-apply to Workday/Greenhouse
- [ ] InsForge backend for application tracking (database)
- [ ] Zeabur deployment for one-click sharing


## Built at 
**Build Smth AI-Native Hackathon @Cal** — May 2026

**Sponsors:** [OpenSwarm](https://openswarm.com) · [Retell](https://retellai.com) · [InsForge](https://insforge.com) · [Zeabur](https://zeabur.com) · [Entelligence AI](https://entelligence.ai) · [PixVerse](https://pixverse.ai) · [Klarity Health](https://klarity.health)

## Devpost Submission
- [DevPost Submission](https://devpost.com/software/swarmapply?_gl=1*lrkf9c*_gcl_au*OTcxOTU3NjMxLjE3NzgyNzY5ODg.*_ga*MTkwNzU3NTcxNS4xNzc4Mjc2OTg4*_ga_0YHJK3Y10M*czE3NzgzOTE2MDMkbzUkZzEkdDE3NzgzOTE2MTckajQ2JGwwJGgw)

## Author
[Ethan Ngo](https://github.com/ethngo7)
