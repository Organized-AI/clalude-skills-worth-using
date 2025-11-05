# ⏱️ Claude Code Session Manager

> Intelligent scheduling system that analyzes your calendar, predicts token usage, and automatically schedules optimal 5-hour Claude Code sessions.

## 🎯 Overview

The CC Session Manager automates the planning of Claude Code sessions by:
1. Analyzing your macOS Calendar (iCal) for available time blocks
2. Parsing Claude conversation JSONL files to understand usage patterns
3. Predicting token consumption based on historical data
4. Scheduling optimal 5-hour coding sessions
5. Creating calendar events automatically

## ✨ Key Features

- **Calendar Integration**: Direct macOS Calendar (iCal) access and event creation
- **Token Analysis**: Parses Claude conversation JSONL files for usage patterns
- **Smart Predictions**: Machine learning-based token usage forecasting
- **Automatic Scheduling**: Creates 5-hour Claude Code session blocks
- **Visualization**: Generates charts showing usage patterns and projections
- **Zero Configuration**: Works immediately with no setup questions

## 🚀 Quick Start

### Prerequisites

- macOS (for iCal integration)
- Python 3.8+
- Access to Claude conversation JSONL export files

### Installation

```bash
# Clone the repository
git clone https://github.com/Organized-AI/clalude-skills-worth-using.git
cd clalude-skills-worth-using/skills/cc-session-manager

# Install dependencies
pip install -r requirements.txt

# Make scripts executable
chmod +x setup.sh

# Run setup
./setup.sh
```

### Usage

**Simply tell Claude:**
```
"Schedule my Claude Code sessions"
```

Claude will immediately:
1. Access your calendar
2. Analyze your conversation history
3. Calculate token usage
4. Schedule optimal sessions
5. Create calendar events
6. Show you the complete schedule

**No questions asked. No configuration needed. Just instant analysis and scheduling.**

## 📊 How It Works

### 1. Calendar Analysis

```python
# Automatically scans your iCal calendar
- Identifies free time blocks
- Respects existing commitments
- Looks for 5+ hour availability windows
- Prioritizes weekday afternoons/evenings
```

### 2. Token Usage Analysis

```python
# Parses JSONL conversation files
- Extracts message lengths
- Calculates token counts per conversation
- Identifies usage patterns by day/time
- Computes average session consumption
```

### 3. Predictive Scheduling

```python
# Machine learning predictions
- Forecasts token usage for upcoming sessions
- Optimizes session timing based on patterns
- Ensures you stay within Claude Code limits
- Maximizes productive coding time
```

### 4. Automatic Event Creation

```python
# Creates calendar events
- 5-hour blocks labeled "Claude Code Session"
- Includes token budget in description
- Sets reminders 15 minutes before
- Syncs across all Apple devices
```

## 📝 Example Output

```
📅 Claude Code Session Schedule

Analysis Complete:
- Calendar availability analyzed
- 12 JSONL conversation files parsed
- Total tokens used (last 30 days): 847,392
- Average session usage: 28,246 tokens

Scheduled Sessions:

📅 Monday, Nov 11 | 2:00 PM - 7:00 PM
   Token Budget: 30,000
   Projects: API Development, Database Migration

📅 Wednesday, Nov 13 | 1:00 PM - 6:00 PM
   Token Budget: 30,000
   Projects: Frontend Refactor, Testing

📅 Friday, Nov 15 | 3:00 PM - 8:00 PM
   Token Budget: 30,000
   Projects: Documentation, Code Review

Total Scheduled: 15 hours
Projected Token Usage: 90,000
Remaining Budget: 60,000 (buffer)

✅ Calendar events created successfully!
```

## 🛠️ Python Scripts

### scheduler.py
Main orchestration script that:
- Coordinates all analysis components
- Makes final scheduling decisions
- Creates calendar events

### token_analyzer.py
JSONL file parser that:
- Extracts message data
- Calculates token usage
- Generates usage statistics

### calendar_integration.py
macOS Calendar interface that:
- Reads existing events
- Finds available time blocks
- Creates new session events

### predictor.py
Machine learning module that:
- Analyzes historical patterns
- Predicts future token usage
- Optimizes session timing

### visualizations.py
Chart generation for:
- Token usage over time
- Session duration patterns
- Availability heatmaps

## 📋 Configuration (Optional)

While the skill works with zero configuration, you can customize:

```python
# config.py (optional)

SESSION_DURATION = 5  # hours
TOKEN_BUDGET_PER_SESSION = 30000
PREFERRED_START_TIMES = ["13:00", "14:00", "15:00"]
MINIMUM_GAP_BETWEEN_SESSIONS = 24  # hours
WEEKDAYS_ONLY = True
CALENDAR_NAME = "Work"  # or None for default
```

## 📊 Visualization Examples

### Token Usage Timeline
```
       Token Usage Per Day (Last 30 Days)
50K ┊███▀
    ┊  ████▀
40K ┊    ████▀
    ┊      ████▀
30K ┊        ████▀
    ┊──────────────────────
    Week 1  Week 2  Week 3  Week 4
```

### Availability Heatmap
```
        MON  TUE  WED  THU  FRI
9am     ░░░  ░░░  ███  ░░░  ░░░
1pm     ███  ███  ░░░  ███  ███  <- Best times
5pm     ███  ░░░  ███  ███  ░░░

███ = Available  ░░░ = Busy
```

## 🔗 Integration with Other Tools

### With Weekly Planner Skill
```
Combines with weekly-planner to:
- Align Claude Code sessions with weekly anchors
- Coordinate deep work blocks
- Track learning time in evening sessions
```

### With Memory System
```
Stores:
- Session productivity metrics
- Token usage patterns
- Optimal scheduling preferences
- Project correlations with token usage
```

## 📚 Technical Details

### JSONL File Format

Expected format from Claude conversation exports:
```json
{
  "uuid": "conversation-id",
  "name": "Conversation Title",
  "created_at": "2025-11-01T10:30:00Z",
  "updated_at": "2025-11-01T12:45:00Z",
  "chat_messages": [
    {
      "uuid": "message-id",
      "text": "message content",
      "sender": "human",
      "created_at": "2025-11-01T10:30:00Z"
    }
  ]
}
```

### Token Calculation

Approximate formula used:
```python
tokens = len(text.split()) * 1.3  # rough approximation
# More sophisticated tokenization available in full implementation
```

### Calendar Event Structure

```applescript
tell application "Calendar"
    tell calendar "Work"
        make new event with properties {
            summary: "Claude Code Session",
            start date: date "Monday, November 11, 2025 at 2:00:00 PM",
            end date: date "Monday, November 11, 2025 at 7:00:00 PM",
            description: "Token Budget: 30,000\nProjects: API Dev, Testing"
        }
    end tell
end tell
```

## ⚠️ Limitations

- **macOS Only**: iCal integration requires macOS
- **JSONL Required**: Needs exported Claude conversation files
- **5-Hour Blocks**: Optimized for Claude Code's 5-hour session structure
- **Token Estimates**: Predictions are approximations, not guarantees

## 👥 Who This Is For

- **Claude Code Users**: Maximize productive session time
- **Busy Developers**: Automatically find optimal coding windows
- **Token Optimizers**: Stay within limits without manual tracking
- **Calendar Power Users**: Integrate AI coding into existing workflows

## 📚 Advanced Usage

### Dry Run Mode
```bash
# Preview schedule without creating events
python scheduler.py --dry-run
```

### Custom Date Range
```bash
# Schedule for next 2 weeks
python scheduler.py --weeks 2
```

### Specific Projects
```bash
# Focus on particular projects
python scheduler.py --projects "API Dev,Testing"
```

## 🔧 Troubleshooting

### Issue: Calendar events not appearing
**Solution**: Check Calendar.app permissions in System Settings > Privacy & Security

### Issue: JSONL files not found
**Solution**: Ensure files are in `~/Documents/Claude_Conversations/` or specify path

### Issue: Token predictions seem off
**Solution**: More historical data improves accuracy - run with at least 10+ conversations

## 💬 Philosophy

**The goal is to remove friction from Claude Code usage.**

Instead of:
1. Manually checking calendar
2. Guessing token availability
3. Creating events one by one
4. Hoping you scheduled optimally

You get:
1. Instant analysis
2. Data-driven predictions
3. Automatic scheduling
4. Optimized session timing

**Just tell Claude to schedule, and it happens.**

## 🔗 Related Skills

- **weekly-planner**: Coordinate with weekly anchors and deep work blocks
- **data-audit**: Use similar pattern analysis techniques
- **Memory System**: Store and learn from session patterns

---

**Version**: 1.0.0  
**Last Updated**: November 4, 2025  
**Platform**: macOS (iCal required)  
**Maintained By**: Organized AI

---

**Remember**: This skill embodies the principle of "just do it" - no questions, no options, just immediate, intelligent action.