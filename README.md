# Claude Skills Worth Using

A curated collection of Claude skills, configurations, and best practices for effective AI-assisted workflows.

## 📚 Repository Structure

```
claude-skills-worth-using/
├── README.md                          # This file
├── skills/                            # Claude skills and workflows
│   └── data-audit/                    # Meta Ads data audit skill
├── config/                            # Configuration files and preferences
│   └── user-preferences.md            # Claude behavior configurations
├── examples/                          # Example artifacts and outputs
│   └── artifacts/                     # Sample generated artifacts
└── docs/                              # Additional documentation
```

## 🎯 What's Inside

### Skills

#### Data Audit Skill
A comprehensive skill for auditing Meta Ads accounts, including:
- Campaign and ad performance analysis
- Tracking infrastructure assessment
- CAPI (Conversions API) implementation guidance
- Automated report generation
- Architecture diagrams and recommendations

**Tools Required:** Pipeboard Meta MCP Server

[View Data Audit Skill →](./skills/data-audit/)

### Configuration

#### User Preferences
Customized Claude behavior protocols including:
- Memory management workflows
- Filesystem access patterns
- Project-specific behaviors
- Tool usage protocols

[View Configuration →](./config/user-preferences.md)

### Examples

Real-world artifacts generated using these skills:
- Meta account audits
- Asana project insights
- Pixel tracking checklists
- Visual architecture diagrams

[View Examples →](./examples/)

## 🚀 Getting Started

### Prerequisites

1. **Claude Account**: Access to Claude (Sonnet 4.5 or newer recommended)
2. **MCP Servers**: Relevant MCP servers installed for your use case
3. **Project Setup**: Enable Claude Projects for optimal memory management

### Using a Skill

1. Navigate to the skill directory
2. Read the `SKILL.md` file
3. Copy the skill content or reference it in your Claude Project
4. Follow the usage guide for activation phrases

### Example: Data Audit Skill

```bash
# Add to your Claude Project or conversation
"Audit Meta account act_1234567890"
```

Claude will automatically:
- Fetch account data using Pipeboard Meta tools
- Analyze campaigns, ad sets, and ads
- Generate comprehensive audit artifacts
- Provide actionable recommendations

## 📖 Documentation

Each skill includes:
- **SKILL.md**: Main skill instructions and workflows
- **README.md**: Overview and quick start guide
- **Usage Guide**: Detailed activation and customization
- **Examples**: Real-world outputs and artifacts
- **References**: Templates, checklists, and best practices

## 🛠️ Tools & Integrations

### Supported MCP Servers

- **Pipeboard Meta**: Meta Ads API integration
- **GitHub**: Repository management
- **Google Workspace**: Sheets, Docs, Calendar
- **Memory**: Knowledge graph and entity management
- **Sequential Thinking**: Enhanced reasoning workflows

### Required Tools

- Memory management (for persistent context)
- File system access (for local operations)
- Web search (for research and validation)

## 🤝 Contributing

This is an internal Organized AI repository. Contributions should follow these guidelines:

1. **Skills**: Must include SKILL.md, README.md, and usage guide
2. **Documentation**: Clear, concise, with examples
3. **Testing**: Verify skill works with target MCP servers
4. **Structure**: Follow existing directory patterns

## 📝 Best Practices

### Memory Management

- Create entities for projects, people, and organizations
- Use relations to connect related concepts
- Store observations for key facts and details
- Regular memory updates after significant conversations

### Skill Development

- Start with clear activation phrases
- Include comprehensive workflows
- Provide templates and examples
- Document tool dependencies
- Test with real-world scenarios

### File Organization

- Group related files in directories
- Use descriptive filenames
- Include README in each directory
- Keep artifacts separate from core skills

## 🔗 Related Resources

- [Anthropic Documentation](https://docs.anthropic.com)
- [MCP Specification](https://modelcontextprotocol.io)
- [Claude Projects Guide](https://docs.claude.com/projects)
- [Organized AI GitHub](https://github.com/Organized-AI)

## 📄 License

Internal use for Organized AI. All rights reserved.

## 📧 Contact

- **Organization**: Organized AI
- **GitHub**: [@Organized-AI](https://github.com/Organized-AI)
- **Website**: [organized.ai](https://organized.ai)

---

**Last Updated**: November 4, 2025  
**Maintained By**: Organized AI Team  
**Version**: 1.0.0
