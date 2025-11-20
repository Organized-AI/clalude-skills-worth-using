---
name: tech-debt-analyzer  
description: Comprehensive codebase health assessment for M&A technical due diligence. Scans for code complexity, technical debt, dependency issues, and generates integration complexity estimates. Provides refactoring roadmaps and technical risk assessment.
---

# Tech Debt Analyzer (M&A Edition)

Technical due diligence tool for assessing codebase quality, identifying technical debt, and estimating integration complexity for acquisition targets.

## Core Capability

Analyzes codebases to assess:
- Code complexity and quality
- Technical debt levels
- Dependency health
- Security vulnerabilities
- Integration complexity
- Refactoring requirements
- Technical risk factors

## Workflow

### 1. Repository Analysis Setup

**Inputs needed:**
- Repository URL or local path
- Primary language(s)
- Technology stack
- Acquisition context (if M&A due diligence)

**If integrated with startup-validator:**
```
Pull context:
- Company name
- Technology stack (from validation)
- Integration requirements
```

### 2. Automated Code Scanning

Perform comprehensive analysis:

#### A. Complexity Analysis
**Scan for:**
- Cyclomatic complexity
- Function/method length
- Class size
- Nesting depth
- Code duplication

**Tools to reference:**
```python
# Example patterns to identify:
- Functions >100 lines
- Complexity score >15
- Duplicate code blocks
- Deep nesting >5 levels
```

#### B. Dependency Audit
**Check:**
- Outdated packages
- Known vulnerabilities
- License conflicts
- Dependency count
- Update frequency

**Package managers:**
- npm (package.json)
- pip (requirements.txt)
- Maven (pom.xml)
- Gradle (build.gradle)

#### C. Code Quality Metrics
**Evaluate:**
- Test coverage
- Documentation quality
- Code comments
- Naming conventions
- Type safety

#### D. Technical Debt Indicators
**Identify:**
- TODO/FIXME comments
- HACK markers
- Deprecated functions
- Dead code
- Magic numbers

### 3. Integration Complexity Assessment

**For M&A due diligence, assess:**

#### Technology Stack Compatibility
- **Compatible**: Same language, similar frameworks
- **Moderate**: Different but interoperable
- **Complex**: Complete rewrite needed

#### Data Integration
- **Database compatibility**
- **API design quality**
- **Data model complexity**
- **Migration requirements**

#### Infrastructure Requirements
- **Cloud platform** (AWS, Azure, GCP)
- **Deployment complexity**
- **Scaling capabilities**
- **DevOps maturity**

### 4. Generate Assessment Report

Output comprehensive analysis:

```
🔧 TECHNICAL DEBT ANALYSIS REPORT
════════════════════════════

Repository: [Name]
Language(s): [Primary languages]
Overall Health Score: [X]/100

COMPLEXITY ANALYSIS
────────────────
• High Complexity Functions: XX
• Average Complexity: X.X
• Code Duplication: XX%
• Lines of Code: XXX,XXX

DEPENDENCY HEALTH
────────────────
• Total Dependencies: XXX
• Outdated: XX (XX%)
• Vulnerabilities: X high, XX medium
• License Issues: X

CODE QUALITY
────────────────
• Test Coverage: XX%
• Documentation: [Excellent/Good/Poor]
• Type Safety: [Strong/Weak/None]
• Code Comments: XX%

TECHNICAL DEBT
────────────────
• TODO/FIXME: XXX items
• Deprecated Code: XX instances
• Dead Code: ~XX files
• Estimated Debt: $XXX,XXX

INTEGRATION COMPLEXITY (M&A)
────────────────
• Overall: [LOW/MEDIUM/HIGH]
• Stack Compatibility: [Compatible/Moderate/Complex]
• Data Migration: [Simple/Moderate/Complex]
• Estimated Timeline: XX weeks
• Integration Cost: $XXX,XXX

CRITICAL ISSUES
────────────────
🔴 HIGH: [Critical issue 1]
🔴 HIGH: [Critical issue 2]
⚠️  MEDIUM: [Moderate concern]

REFACTORING ROADMAP
────────────────
Phase 1 (Weeks 1-4):
- [Action 1]
- [Action 2]

Phase 2 (Weeks 5-12):
- [Action 1]
- [Action 2]

Phase 3 (Weeks 13-24):
- [Action 1]
- [Action 2]

RECOMMENDATIONS
────────────────
1. 🔴 [Priority action]
2. 🔴 [Priority action]
3. 🟡 [Secondary action]
```

## Scoring System

### Overall Health Score (100 points)

**Code Quality (30 points)**
- Test coverage >80%: 10 pts
- Documentation quality: 10 pts
- Naming/structure: 10 pts

**Complexity (25 points)**
- Low average complexity: 10 pts
- Minimal duplication: 8 pts
- Clean architecture: 7 pts

**Dependencies (25 points)**
- Up-to-date packages: 10 pts
- No vulnerabilities: 10 pts
- License compliance: 5 pts

**Technical Debt (20 points)**
- Minimal TODO/FIXME: 8 pts
- No deprecated code: 7 pts
- No dead code: 5 pts

### Health Score Interpretation

**85-100: Excellent** ✅
- Well-maintained codebase
- Low integration risk
- Minimal refactoring needed

**70-84: Good** 🟢
- Generally healthy
- Some cleanup needed
- Moderate integration effort

**50-69: Fair** 🟡
- Significant technical debt
- Refactoring recommended
- High integration complexity

**<50: Poor** 🔴
- Major issues present
- Extensive refactoring required
- Consider rebuild vs. integrate

## Integration with M&A Workflow

```
Workflow:
startup-validator
    ↓ Tech stack identified
tech-debt-analyzer (this skill)
    ↓ Health score: 75/100
    ↓ Integration: MEDIUM complexity
business-fin-analyst
    ↓ Factor in $200K refactoring cost
pitch-deck
    ↓ Include technical assessment
```

## Activation Triggers

- "Analyze technical debt in [repo]"
- "Assess codebase health for [company]"
- "Technical due diligence on [repository]"
- "Integration complexity for [acquisition]"
- "Code quality review"

## Best Practices

### Do:
✅ Run automated tools when possible
✅ Check multiple quality dimensions
✅ Estimate financial impact of debt
✅ Provide specific recommendations
✅ Include refactoring timeline

### Don't:
❌ Skip dependency audit
❌ Ignore security vulnerabilities
❌ Give scores without evidence
❌ Underestimate integration complexity
❌ Forget to check licenses

## Reference Materials

See `references/` for:
- Code complexity metrics guide
- Security vulnerability database
- Refactoring best practices
- Integration patterns

## Tools Integration

When available, reference these tools:
- **Complexity**: radon (Python), ESLint (JS), SonarQube
- **Dependencies**: npm audit, pip-audit, Snyk
- **Coverage**: coverage.py, Istanbul, JaCoCo
- **Security**: Bandit, ESLint Security, OWASP

---

**Enhanced by Organized-AI**
**Based on ailabs-393/ai-labs-claude-skills**
**License: MIT**