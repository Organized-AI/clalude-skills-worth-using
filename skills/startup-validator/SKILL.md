---
name: startup-validator
description: Comprehensive startup validation for M&A due diligence. Scores companies against acquisition rubrics, identifies red flags, assesses strategic fit, and generates board-ready recommendations - no questions asked.
license: MIT
allowed-tools: [view, file_create]
metadata:
  version: 1.0.0
  enhanced_for: M&A due diligence
  organization: Organized-AI
  source: Enhanced from ailabs-393/ai-labs-claude-skills
  updated: 2025-11-19
---

# Startup Validator

## Overview

Comprehensive startup validation system for M&A due diligence. Automatically scores acquisition targets against industry rubrics, identifies strategic fit, assesses risks, and generates executive recommendations.

## Core Capability

**"No Questions Asked" Validation**
- Provide company brief → Get complete validation report
- Automatic scoring across 4 dimensions
- Strategic fit analysis
- Risk assessment matrix
- Board-ready recommendations

## Activation Phrases

```
"Validate this startup for acquisition: [company brief]"
"Score [company] against M&A rubrics"
"Generate due diligence checklist for [company]"
"Assess strategic fit with [target company]"
```

## Validation Framework

### 4-Dimension Scoring System

#### 1. Market Opportunity (25 points)
- TAM analysis (>$1B preferred)
- Market growth rate (>15% YoY)
- Competitive positioning
- Timing and market readiness

#### 2. Financial Health (25 points)
- Revenue metrics (ARR, growth rate)
- Profitability (gross margin >60%)
- Unit economics (LTV/CAC >3x)
- Path to profitability

#### 3. Strategic Fit (25 points)
- Synergy potential (>$5M)
- Customer overlap
- Technology compatibility
- Cultural alignment

#### 4. Team & Execution (25 points)
- Founder experience
- Key hires and retention (>90%)
- Execution track record
- Team completeness

### Scoring Interpretation
```
90-100: ⭐⭐⭐⭐⭐ Excellent acquisition target
75-89:  ⭐⭐⭐⭐   Good target, some concerns
60-74:  ⭐⭐⭐     Proceed with caution
<60:    ⭐⭐       High risk, investigate further
```

## Reference Materials

Load additional context from:
- `references/frameworks.md` - Complete validation frameworks
- `references/scoring-rubrics.md` - Industry benchmarks
- `references/due-diligence-checklist.md` - Comprehensive checklists

## Integration Points

### With Other Skills
```
Complete M&A Analysis:
├─ startup-validator → Validate target
├─ business-fin-analyst → Analyze financials  
├─ tech-debt-analyzer → Assess codebase
└─ pitch-deck → Generate acquisition proposal
```

## Example Usage

```
User: "Validate this startup for acquisition:
Company: DataFlow Analytics
ARR: $2.5M, Growth: 120% YoY
Team: 15 people, Customers: 150 enterprise"

Claude: [Generates complete validation report with scoring]
```

## Credits

**Enhanced by:** Organized-AI  
**Original Source:** ailabs-393/ai-labs-claude-skills  
**License:** MIT