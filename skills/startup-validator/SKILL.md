---
name: startup-validator
description: Comprehensive startup validation for M&A due diligence with automated scoring, strategic fit analysis, and board-ready recommendations
license: MIT
allowed-tools: [bash, file_create, str_replace, view]
---

# Startup Validator

Comprehensive startup validation system for M&A due diligence. Automatically scores acquisition targets against industry rubrics, identifies strategic fit, assesses risks, and generates executive recommendations.

## Core Capability

**"No Questions Asked" Validation** - Provide company brief → Get complete validation report automatically.

## Activation

```
"Validate this startup for acquisition: [company brief]"
"Score [company] against M&A rubrics"
"M&A validation for [company name]"
```

## Validation Framework

### 4-Dimension Scoring (100 points total)

1. **Market Opportunity** (25 pts): TAM, growth rate, positioning
2. **Financial Health** (25 pts): Revenue, margins, unit economics
3. **Strategic Fit** (25 pts): Synergies, customer overlap, tech compatibility
4. **Team & Execution** (25 pts): Founders, retention, track record

### Scoring Interpretation
- 90-100: ⭐⭐⭐⭐⭐ Excellent acquisition target
- 75-89: ⭐⭐⭐⭐ Good target, some concerns
- 60-74: ⭐⭐⭐ Proceed with caution
- <60: ⭐⭐ High risk

## Integration Points

Works with:
- **business-fin-analyst** → Financial validation
- **pitch-deck** → Acquisition proposals
- **tech-debt-analyzer** → Technical assessment

## Reference Materials

Load additional context from:
- `references/validation-frameworks.md` - Complete rubrics
- `references/industry-benchmarks.md` - Sector metrics
- `assets/due-diligence-template.md` - Checklist template

## Example Output

```
📊 STARTUP VALIDATION REPORT
Company: DataFlow Analytics
Overall Score: 82/100 ⭐⭐⭐⭐

DIMENSION SCORES
Market Opportunity:    22/25
Financial Health:      20/25  
Strategic Fit:         21/25
Team & Execution:      19/25

RECOMMENDATION: GOOD ACQUISITION TARGET
✅ Strong revenue growth (120% YoY)
✅ Enterprise customer base
⚠️  Need deeper tech assessment

[Complete analysis follows...]
```

---

**Source:** Enhanced from ailabs-393/ai-labs-claude-skills  
**License:** MIT  
**Maintained by:** Organized-AI