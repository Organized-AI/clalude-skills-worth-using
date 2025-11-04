# Data Audit Skill

A comprehensive Claude skill for conducting Meta Ads account audits using the Pipeboard Meta MCP integration.

## Overview

This skill enables Claude to perform systematic, data-driven audits of Meta advertising accounts. It combines live API access with best practices for tracking implementation, CAPI setup, and campaign optimization.

## Files

- **`data-audit.skill`** - The complete skill definition with prompts, triggers, and workflows
- **`DATA_AUDIT_SKILL_GUIDE.md`** - Detailed guide for using the skill effectively

## Activation Phrases

The skill automatically triggers when you use phrases like:
- "Audit this Meta account"
- "Analyze ad performance"
- "Evaluate tracking setup"
- "Create CAPI recommendations"
- "Generate audit report"
- "Assess campaign performance"

## Features

### Live Data Collection
- Real-time Meta Ads API access via Pipeboard MCP
- Account structure analysis
- Campaign performance metrics
- Pixel configuration review
- CAPI implementation assessment

### Comprehensive Artifacts
1. **Executive Summary** - High-level findings and recommendations
2. **Meta Account Insights** - Detailed account structure and performance
3. **Asana Project Insights** - Task management and project tracking
4. **Comprehensive Audit** - Full analysis with what's wrong and what's next
5. **Visual Architecture** - System diagrams and data flow
6. **Pixel Audit Checklist** - Implementation verification and testing

### Best Practices Integration
- One CAPI per pixel/dataset methodology
- Event deduplication strategies
- Enhanced matching parameters
- Attribution recovery optimization
- Stape container recommendations

## Requirements

- Pipeboard Meta MCP server configured and running
- Meta Ads account access
- Valid access token

## Usage

Simply ask Claude to audit a Meta account and provide the account ID:

```
Audit act_4178428858845500 and create a comprehensive report
```

Claude will:
1. Gather account data using Pipeboard Meta MCP
2. Analyze campaign structure and performance
3. Evaluate tracking implementation
4. Generate comprehensive artifacts
5. Provide actionable recommendations

## Example Use Cases

- **Client Onboarding**: Conduct initial account audit before taking over management
- **Performance Review**: Quarterly or monthly account health checks
- **Tracking Audit**: Verify pixel and CAPI implementation
- **Campaign Optimization**: Identify improvement opportunities
- **Compliance Review**: Ensure proper setup and data handling

## Integration

This skill works seamlessly with:
- Pipeboard Meta MCP for live API access
- Stape MCP for server-side tracking configuration
- Asana for project management
- Your existing audit workflows

## Learn More

See the `/examples/artifacts/` directory for real audit examples from client projects.