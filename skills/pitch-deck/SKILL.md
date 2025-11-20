---
name: pitch-deck
description: Professional pitch deck generation for M&A acquisitions, startup fundraising, and executive presentations with auto-population from analysis data
license: MIT
allowed-tools: [bash, file_create, str_replace, view]
---

# Pitch Deck Generator

Creates professional, board-ready pitch decks for M&A acquisitions, startup fundraising, and executive summaries with automatic data population.

## Core Capability

**Professional Decks in Minutes** - Provide context → Get complete presentation automatically.

## Activation

```
"Generate M&A acquisition deck for [company]"
"Create fundraising presentation"
"Build executive summary deck"
```

## Deck Types

### M&A Acquisition Deck (12-15 slides)
1. Executive Summary
2. Target Company Overview  
3. Market Opportunity
4. Financial Performance
5. Strategic Rationale
6. Synergy Analysis
7. Valuation
8. Integration Plan
9. Risk Assessment
10. Deal Structure
11. Timeline
12. Recommendation

### Startup Fundraising Deck (10-12 slides)
1. Cover
2. Problem
3. Solution
4. Market Opportunity
5. Product
6. Traction
7. Business Model
8. Competition
9. Team
10. Financials
11. Ask

### Executive Summary Deck (5-7 slides)
1. Overview
2. Key Metrics
3. Strategic Highlights
4. Financials
5. Recommendations

## Auto-Population

Automatically pulls data from:
- **startup-validator** → Validation scores, strategic fit
- **business-fin-analyst** → Financial metrics, projections
- **tech-debt-analyzer** → Technical assessment

## Reference Materials

- `references/manda-template.md` - M&A acquisition template
- `references/fundraising-template.md` - Startup pitch template
- `references/design-guidelines.md` - Professional design standards
- `assets/slide-layouts.md` - Layout templates

## Example

```
User: "Generate M&A acquisition deck for DataFlow Analytics"

Claude: [Creates complete 15-slide deck with:
- Auto-populated financials from analysis
- Strategic rationale
- Synergy calculations  
- Professional formatting
- Board-ready presentation]
```

---

**Source:** Enhanced from ailabs-393/ai-labs-claude-skills  
**License:** MIT  
**Maintained by:** Organized-AI