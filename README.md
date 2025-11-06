# Claude Skills Worth Using

A curated collection of production-ready Claude skills, configurations, and best practices for effective AI-assisted workflows.

## 📁 Repository Structure

```
claude-skills-worth-using/
├── README.md                # This file
├── skills/                  # Claude skills and workflows
│   ├── data-audit/         # Meta Ads data audit skill
│   ├── weekly-planner/     # Energy-based weekly planning system
│   ├── cc-session-manager/ # Claude Code session scheduler
│   └── posthog-wizard/     # AI-First CLI patterns from PostHog Wizard
├── config/                  # Configuration files and preferences
│   └── user-preferences.md # Claude behavior configurations
├── examples/                # Example artifacts and outputs
│   └── artifacts/          # Sample generated artifacts
└── docs/                    # Additional documentation
```

## 🎯 Featured Skills

### 🗓️ Weekly Planner

**Sustainable productivity framework with energy-based scheduling**

A comprehensive weekly planning system that manages 2-3 weekly anchors, protects sacred morning practice, and leverages evening time for learning - all while preventing burnout.

**Key Features:**
- 🔴🟡🟢 Energy-based task scheduling (Drain/Neutral/Energize)
- 📊 2-3 weekly anchors with P0/P1/P2 priorities
- ⏰ Sacred morning practice protection (until 1pm)
- 🌙 Evening learning time (7pm-9pm, 1-2 hours)
- 📈 Friday Strategic Growth System reviews
- 🧠 Full memory integration for continuous improvement

**Activation:**
```
"Plan my week"
"I completed [task]"
"Weekly review"
```

**Tools Required:** Memory System, Conversation Search

[→ View Weekly Planner Documentation](./skills/weekly-planner)

---

### ⏱️ CC Session Manager

**Intelligent Claude Code session scheduler with token optimization**

Automatically analyzes your calendar, parses conversation history, predicts token usage, and schedules optimal 5-hour Claude Code sessions - no questions asked.

**Key Features:**
- 📅 macOS Calendar (iCal) integration
- 📊 JSONL conversation file analysis
- 🎯 Token usage prediction
- 🤖 Automatic 5-hour session scheduling
- 📈 Visualization of usage patterns
- ⚡ Zero-configuration operation

**Activation:**
```
"Schedule my Claude Code sessions"
"Plan coding time"
```

**Tools Required:** Python 3.8+, macOS Calendar access

[→ View CC Session Manager Documentation](./skills/cc-session-manager)

---

### 📊 Data Audit

**Comprehensive Meta Ads account auditing and analysis**

Performs deep-dive audits of Meta advertising accounts, including campaign performance, tracking infrastructure, CAPI implementation, and strategic recommendations.

**Key Features:**
- 📊 Campaign and ad performance analysis
- 🔧 Tracking infrastructure assessment
- 🔄 CAPI (Conversions API) implementation guidance
- 📋 Automated report generation
- 🏗️ Architecture diagrams and recommendations
- 📈 ROI and optimization insights

**Activation:**
```
"Audit Meta account act_1234567890"
"Analyze campaign performance"
```

**Tools Required:** Pipeboard Meta MCP Server

[→ View Data Audit Documentation](./skills/data-audit)

---

### 🎯 PostHog Wizard

**AI-First CLI patterns from PostHog Wizard**

Learn and apply patterns from PostHog Wizard for building AI-first developer tools with deterministic LLM prompting, MCP management, and agent rules generation.

**Key Features:**
- 🎯 Deterministic Prompting patterns (force structured JSON)
- 🔧 LLM Query Wrappers (centralized API calls)
- 📋 Agent Rules Generation (create `.cursor/rules` files)
- 🔌 MCP Server Management (programmatic installation)
- 📊 CLI Analytics integration
- 🏗️ AI-First Architecture patterns

**Activation:**
```
"PostHog Wizard patterns"
"CLI wizard architecture"
"Deterministic prompting"
"MCP management"
```

**Tools Required:** None (knowledge skill)

[→ View PostHog Wizard Documentation](./skills/posthog-wizard)

---

## 🚀 Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Organized-AI/clalude-skills-worth-using.git
   cd clalude-skills-worth-using
   ```

2. **Choose a skill:**
   ```bash
   cd skills/weekly-planner  # or data-audit, cc-session-manager, posthog-wizard
   ```

3. **Read the documentation:**
   - `SKILL.md` - Core skill instructions
   - `README.md` - Detailed usage guide
   - Reference materials (if included)

4. **Use in Claude:**
   - Copy skill to your Claude Project
   - Use activation phrases
   - Let the skill work automatically

## 📋 Requirements

### All Skills:
- Claude Account (Sonnet 4.5 or newer recommended)
- Enable Claude Projects for memory management

### Weekly Planner:
- Memory System enabled
- Conversation Search capability

### CC Session Manager:
- Python 3.8+
- macOS (for iCal integration)
- Access to Claude conversation JSONL exports

### Data Audit:
- Pipeboard Meta MCP Server installed
- Meta Ads account access

### PostHog Wizard:
- None (knowledge-only skill)
- Optional: Understanding of CLI development

## 📚 Skill Documentation

Each skill includes comprehensive documentation:

| File | Purpose |
|------|---------|
| `SKILL.md` | Core skill logic and workflows |
| `README.md` | User guide and examples |
| `references/` | Templates and best practices (if applicable) |
| `examples/` | Sample outputs and use cases |

## 🔧 MCP Servers

Recommended MCP servers for enhanced functionality:

- **Pipeboard Meta**: Meta Ads API integration
- **GitHub**: Repository management
- **Google Workspace**: Sheets, Docs, Calendar
- **Memory**: Knowledge graph and entity management
- **Sequential Thinking**: Enhanced reasoning workflows

## 📊 Skills Comparison

| Skill | Memory | File System | Calendar | Python | MCP Servers |
|-------|--------|-------------|----------|--------|-------------|
| Weekly Planner | ✅ | - | - | - | - |
| CC Session Manager | Recommended | - | ✅ (macOS) | ✅ | - |
| Data Audit | Recommended | - | - | - | ✅ Pipeboard Meta |
| PostHog Wizard | - | - | - | - | - |

## 💡 Example Workflows

### Weekly Planner

**You:** "Let's plan this week"

**Claude:**
```
"Let's plan your week! Quick questions:

1. What are your 2-3 ANCHOR projects this week?
2. What's the ONE outcome that would make this week a win?
..."

[Generates complete weekly plan with energy-mapped tasks]
```

### CC Session Manager

**You:** "Schedule my Claude Code sessions"

**Claude:**
```
[Immediately analyzes calendar and conversation history]

"📅 Claude Code Session Schedule

Scheduled Sessions:
📅 Monday, Nov 11 | 2:00 PM - 7:00 PM
   Token Budget: 30,000
   Projects: API Development

✅ Calendar events created successfully!"
```

### Data Audit

**You:** "Audit Meta account act_1234567890"

**Claude:**
```
[Automatically fetches and analyzes account data]

"🔍 Meta Ads Account Audit

Performance Summary:
- Total Spend: $125,430
- ROAS: 3.2x
- Campaigns Analyzed: 12
..."
```

### PostHog Wizard

**You:** "Show me PostHog Wizard's deterministic prompting pattern"

**Claude:**
```
[Retrieves and explains the pattern from PostHog Wizard]

"PostHog Wizard uses a deterministic prompting approach to force structured JSON responses...
```

## 🎯 Feature Matrix

| Feature | Weekly Planner | CC Session Manager | Data Audit | PostHog Wizard |
|---------|----------------|-------------------|-----------|----------------|
| Automation Level | High | Complete | Complete | N/A (Knowledge) |
| Memory Required | Yes | Recommended | Recommended | No |
| Platform | Any | macOS | Any | Any |
| Setup Time | 5 min | 10 min | 2 min | 0 min |
| Best For | Productivity | Code Planning | Marketing Analysis | CLI Development |

## 🤝 Contributing

This is an internal Organized AI repository. Contributions should follow these guidelines:

- **Skills**: Must include SKILL.md, README.md, and usage guide
- **Documentation**: Clear, concise, with examples
- **Testing**: Verify skill works with target MCP servers
- **Structure**: Follow existing directory patterns

### Skill Best Practices

- ✅ Start with clear activation phrases
- ✅ Include comprehensive workflows
- ✅ Provide templates and examples
- ✅ Document tool dependencies
- ✅ Test with real-world scenarios
- ✅ Follow "no questions asked" principle where appropriate

## 🧠 Memory Management

- Create entities for projects, people, and organizations
- Use relations to connect related concepts
- Store observations for key facts and details
- Regular memory updates after significant conversations

## 📁 File Organization

- Group related files in directories
- Use descriptive filenames
- Include README in each directory
- Keep artifacts separate from core skills

## 🎓 Getting Started Guide

### New to Claude Skills?

- Start with **Weekly Planner** - easiest setup, immediate value
- Add **Data Audit** if you work with Meta Ads
- Add **PostHog Wizard** if you're building CLI tools
- Implement **CC Session Manager** for advanced automation

### Already Using Skills?

- Combine **Weekly Planner** with **CC Session Manager** for complete workflow automation
- Use **Data Audit** insights to inform weekly anchors
- Apply **PostHog Wizard** patterns to build your own CLI tools
- Build on these foundations to create your own skills

### Want to download individual skills?

Each skill directory is self-contained and can be used independently.

## 📄 License

Internal use for Organized AI. All rights reserved.

## 🔗 Links

- **Organization**: [Organized AI](https://github.com/Organized-AI)
- **Website**: [organized.ai](https://organized.ai)

## 🎭 Design Philosophy

These skills embody three core principles:

- **Automation Over Configuration**: Skills should "just work" with minimal setup
- **Intelligence Over Options**: Skills make smart decisions instead of asking questions
- **Memory Over Repetition**: Skills learn and improve with each use

The goal is to make AI assistance feel like working with an experienced colleague who knows you, your patterns, and your preferences.

---

**Last Updated:** November 6, 2025  
**Maintained By:** Organized AI Team  
**Version:** 2.1.0 (Now with 4 production-ready skills!)
