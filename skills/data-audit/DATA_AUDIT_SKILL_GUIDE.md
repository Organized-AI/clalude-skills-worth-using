# Data Audit Skill - Usage Guide

## ✅ Skill Successfully Created!

Your "Data Audit" skill has been created and is now active. It's located at:
- **Active Skill:** `/mnt/skills/user/data-audit/`
- **Packaged File:** `/mnt/user-data/outputs/data-audit.skill` (31 KB)

## 🚀 How to Use the Skill

### Automatic Activation

The skill will automatically activate when you use phrases like:
- "Audit this Meta account"
- "Analyze ad performance"
- "Evaluate tracking setup"
- "Create CAPI recommendations"
- "Generate audit report"
- "Assess campaign performance"

### Example Requests

**Basic Audit:**
```
Audit account act_4178428858845500
```

**Comprehensive Analysis:**
```
Conduct a comprehensive data audit for account act_4178428858845500 
including performance analysis, tracking infrastructure assessment, 
and CAPI implementation recommendations.
```

**Specific Analysis:**
```
Analyze the CAPI setup for this Meta account and tell me if we 
should use one or multiple integrations.
```

## 📋 What the Skill Includes

### 1. SKILL.md (Main Instructions)
Comprehensive workflow for:
- Data collection using Pipeboard Meta MCP tools
- Campaign and performance analysis
- Tracking infrastructure assessment
- Artifact generation (reports, diagrams, checklists)
- CAPI best practices and recommendations

### 2. Reference Files

**meta_best_practices.md**
- One vs. multiple CAPI integrations guidance
- Enhanced matching parameters
- Attribution windows and iOS 14+ impact
- Event mapping and integration architecture
- Performance benchmarks

**audit_template.md**
- Complete audit report structure
- Executive summary format
- Performance snapshot tables
- Critical findings framework
- Phased action plan template

**architecture_template.md**
- ASCII art diagrams for current state
- Data flow visualizations
- Ideal state architecture
- Attribution gap analysis
- Comparative benefits tables

**capi_checklist_template.md**
- Pre-implementation checklist
- Phase-by-phase setup guide
- Testing and validation procedures
- Ongoing maintenance tasks
- Troubleshooting guide

### 3. Example Assets

- `example_audit_challenges_by_marisa.md` - Real audit example
- `example_architecture_challenges_by_marisa.md` - Real architecture diagram

## 🔧 Pipeboard Meta MCP Tools Integration

The skill is fully integrated with all Pipeboard Meta MCP tools:

**Account Operations:**
- `get_ad_accounts()`
- `get_account_info()`
- `get_account_pages()`

**Campaign Analysis:**
- `get_campaigns()`
- `get_campaign_details()`
- `get_adsets()`
- `get_adset_details()`
- `get_ads()`
- `get_ad_details()`
- `get_ad_creatives()`

**Performance Insights:**
- `get_insights()` - With breakdown options
- `bulk_get_insights()` - Parallel fetching

**Search & Discovery:**
- `search()` - Find records
- `fetch()` - Get complete record

## 📊 Generated Artifacts

When you run an audit, the skill will guide creation of:

1. **Comprehensive Audit Report**
   - Executive summary with health score
   - Current performance snapshot
   - Detailed campaign analysis
   - Critical findings (severity-rated)
   - Opportunities for improvement
   - Phased action plan
   - Expected outcomes

2. **Visual Architecture Diagram**
   - Current state visualization
   - Data flow analysis
   - Attribution gap illustration
   - Ideal state with CAPI
   - Comparative benefits

3. **CAPI Implementation Checklist**
   - Step-by-step setup guide
   - Testing procedures
   - Validation criteria
   - Ongoing maintenance

4. **Meta Account Insights Summary**
   - Account metadata
   - Campaign performance tables
   - Key metrics dashboard

## 💡 Best Practices When Using the Skill

### 1. Always Use Sequential Thinking
The skill integrates with sequential thinking for complex analysis:
```
Use sequential thinking to analyze this Meta account
```

### 2. Specify Time Ranges
```
Audit the last 30 days of performance for account act_123456
```

### 3. Request Specific Artifacts
```
Generate a comprehensive audit report and architecture diagram 
for account act_123456
```

### 4. Follow the Workflow
The skill follows a systematic workflow:
- Phase 1: Data Collection
- Phase 2: Analysis & Synthesis
- Phase 3: Artifact Generation
- Phase 4: Recommendations

## 🎯 CAPI Analysis Features

The skill includes comprehensive CAPI analysis:

**Automatic Assessment:**
- One vs. multiple CAPI integrations
- Current tracking infrastructure gaps
- iOS 14+ attribution loss estimation
- Match quality score analysis
- Enhanced matching recommendations

**Best Practice Enforcement:**
- Meta-recommended architectures
- Event deduplication strategies
- Enhanced matching parameters
- Integration patterns (Stape + GHL)

## 📦 Sharing the Skill

You can share the packaged skill file:
- Download: `data-audit.skill` from outputs
- Share with team members
- Import into other Claude Code environments

## 🔄 Updating the Skill

To update the skill:
1. Edit files in `/mnt/skills/user/data-audit/`
2. Re-package: `python /mnt/skills/examples/skill-creator/scripts/package_skill.py /mnt/skills/user/data-audit`

## 🌲 Skill Structure

```
data-audit/
├── SKILL.md (Main instructions)
├── references/
│   ├── meta_best_practices.md
│   ├── audit_template.md
│   ├── architecture_template.md
│   └── capi_checklist_template.md
└── assets/
    ├── example_audit_challenges_by_marisa.md
    └── example_architecture_challenges_by_marisa.md
```

## ✅ Skill Validation

The skill has been validated and packaged successfully:
- ✅ YAML frontmatter validated
- ✅ Description comprehensive
- ✅ All references documented
- ✅ Example assets included
- ✅ Ready for use

## 🚀 Try It Now!

Simply say:
```
Audit Meta account act_4178428858845500
```

The skill will automatically activate and guide you through the complete audit process!

---

**Skill Version:** 1.0  
**Created:** November 4, 2025  
**Package Size:** 31 KB  
**Status:** ✅ Active and Ready