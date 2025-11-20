---
name: pitch-deck
description: Professional pitch deck generation for M&A acquisitions, startup fundraising, and executive presentations. Auto-populates from financial analysis data, includes industry templates, and creates board-ready slides with strategic narrative.
---

# Pitch Deck Generator

Creates professional, data-driven presentations for M&A acquisitions, startup fundraising, and executive summaries.

## Core Capability

Generates complete pitch decks with:
- Strategic narrative and story flow
- Auto-populated financial data
- Professional design guidelines
- Industry-specific templates
- Board-ready formatting

## Deck Types

### M&A Acquisition Deck (12-15 slides)
**Use for:** Board presentations, acquisition proposals

1. Cover slide
2. Executive summary
3. Market opportunity
4. Target company overview
5. Financial performance
6. Strategic rationale
7. Synergy analysis
8. Valuation analysis
9. Integration plan
10. Risk assessment
11. Management & team
12. Financial projections
13. Deal structure
14. Timeline & next steps
15. Recommendation

### Startup Fundraising Deck (10-12 slides)
**Use for:** Investor pitches, fundraising rounds

1. Cover slide
2. Problem
3. Solution
4. Market opportunity
5. Product
6. Traction
7. Business model
8. Go-to-market
9. Competition
10. Team
11. Financials
12. Ask

### Executive Summary (5-7 slides)
**Use for:** Quick overviews, status updates

1. Cover
2. Key highlights
3. Financial snapshot
4. Strategic priorities
5. Risk & mitigation
6. Recommendations
7. Next steps

## Workflow

### 1. Deck Type Selection

Ask user (if not specified):
- "What type of deck do you need?"
  - M&A acquisition
  - Startup fundraising
  - Executive summary
  - Custom

### 2. Data Collection

**If integrated with other skills:**
```
Pull from startup-validator:
- Validation score
- Strategic fit analysis
- Risk assessment

Pull from business-fin-analyst:
- Financial metrics
- Valuation models
- Growth projections

Pull from tech-debt-analyzer:
- Technical health score
- Integration complexity
```

**If standalone:**
Gather from user:
- Company name and description
- Key metrics (revenue, growth, etc.)
- Strategic rationale
- Financial data
- Risk factors

### 3. Generate Slide Content

For each slide, create:
- **Title**: Clear, action-oriented
- **Key Message**: One main point
- **Data**: Specific numbers
- **Visual**: Chart or diagram description
- **Speaker Notes**: Additional context

### 4. Design Guidelines

Apply professional standards:
- **Typography**: Sans-serif for headings, serif for body (if formal)
- **Color Scheme**: Primary (brand), secondary (data), accent (calls to action)
- **Layout**: Consistent margins, clear hierarchy
- **Data Visualization**: Clean charts, minimal decoration
- **White Space**: Generous, uncluttered

## Output Format

Provide slide-by-slide content:

```
SLIDE 1: [TITLE]
────────────────────
TITLE: [Slide title]

CONTENT:
• [Bullet point 1]
• [Bullet point 2]
• [Bullet point 3]

KEY METRIC: [Large number/stat]

VISUAL SUGGESTION: [Chart type - bar/line/pie]
- [Data series 1]
- [Data series 2]

SPEAKER NOTES:
[Additional context for presenter]

────────────────────
```

## Integration Examples

### Example 1: M&A Acquisition Deck

```
Workflow:
1. startup-validator scores target: 82/100
2. business-fin-analyst provides valuation: $20-25M
3. pitch-deck generates acquisition proposal

Result:
✅ 15-slide deck
✅ Auto-populated with validation data
✅ Financial charts included
✅ Risk matrix visualized
✅ Board-ready presentation
```

### Example 2: Fundraising Deck

```
User input:
- Company: DataFlow Analytics
- Stage: Series A
- Raising: $5M
- Traction: $2.5M ARR, 120% growth

Result:
✅ 12-slide investor deck
✅ Problem/solution narrative
✅ Market sizing
✅ Traction metrics highlighted
✅ Team backgrounds
✅ Financial projections
```

## Best Practices

### Content
✅ **One key message per slide**
✅ **Data-driven** (include specific numbers)
✅ **Visual focus** (charts > bullets)
✅ **Concise** (max 6 bullets per slide)
✅ **Action-oriented** titles

### Design
✅ **Consistent** layout across slides
✅ **Professional** color scheme
✅ **Readable** font sizes (28pt+ for body)
✅ **High-contrast** text and background
✅ **Quality** images and charts

### Storytelling
✅ **Clear narrative** arc
✅ **Logical flow** between slides
✅ **Compelling** opening
✅ **Strong** close with clear ask
✅ **Anticipated** objections addressed

## Activation Triggers

- "Generate M&A acquisition deck for [company]"
- "Create fundraising pitch deck"
- "Build executive summary presentation"
- "Make board presentation for [topic]"
- "Pitch deck for [company/product]"

## Templates

Access detailed templates in:
- `references/manda_acquisition_template.md`
- `references/startup_fundraising_template.md`
- `references/executive_summary_template.md`
- `references/design_guidelines.md`

## Customization

### Brand Colors
Set your color scheme:
- Primary: #[HEX]
- Secondary: #[HEX]
- Accent: #[HEX]
- Background: #[HEX]

### Fonts
- Headlines: [Font name]
- Body: [Font name]
- Data: [Monospace font]

### Logo Placement
- Bottom right corner
- Consistent across all slides
- Appropriate size (not dominating)

## Notes

- Output is slide content, not PowerPoint file
- User creates actual slides in their tool
- Provides complete content + design guidance
- Can be exported to Google Slides, PowerPoint, Keynote
- Focus on content quality and narrative flow

---

**Enhanced by Organized-AI**
**Based on ailabs-393/ai-labs-claude-skills**
**License: MIT**