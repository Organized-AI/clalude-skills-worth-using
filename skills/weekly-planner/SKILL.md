---
name: weekly-planner
description: >
  Comprehensive weekly planning system that manages default_user's Weekly Planning System using 
  energy-based task scheduling, progress tracking, and strategic review cycles. Use when the user 
  wants to start a new week and generate a weekly plan, update progress on current week tasks, 
  save completed tasks to memory, trigger Friday Strategic Growth System review, check weekly 
  anchor progress, ask about their weekly plan or schedule, or reference their planning methodology.
---

# Weekly Planner

## Overview

This skill manages default_user's Weekly Planning System - a sustainable productivity framework designed to scale output without burnout. The system uses energy-based scheduling (Drain/Neutral/Energize tasks), 2-3 weekly anchors, and continuous improvement through weekly reflection.

## Workflow Decision Tree

When this skill triggers, follow this decision tree:

1. **Is it Sunday or Monday, OR does the user explicitly request a new weekly plan?**
   - YES → Go to [Generate New Weekly Plan](#generate-new-weekly-plan)
   - NO → Continue to step 2

2. **Is the user reporting completed tasks or progress?**
   - YES → Go to [Update Weekly Progress](#update-weekly-progress)
   - NO → Continue to step 3

3. **Is it Friday, OR does the user request a weekly review?**
   - YES → Go to [Conduct Strategic Growth System Review](#conduct-strategic-growth-system-review)
   - NO → Continue to step 4

4. **Is the user asking about their current plan, schedule, or tasks?**
   - YES → Go to [Display Current Week Status](#display-current-week-status)
   - NO → Provide general weekly planning guidance

## Generate New Weekly Plan

**When:** Sunday/Monday at start of new week, or when user explicitly requests it

**Process:**

1. **Retrieve memory** using conversation_search for:
   - Previous week's data (if exists)
   - Active projects and their status
   - Learning goals and progress
   - Strategic connections and upcoming meetings

2. **Ask key planning questions:**
   ```
   Let's plan your week! Quick questions:
   
   1. What are your 2-3 ANCHOR projects this week? (Top priorities)
   2. What's the ONE outcome that would make this week a win?
   3. Any key meetings, calls, or deadlines I should know about?
   4. Learning focus this week? (Python/Next.js/Spanish/Other)
   5. Anything from last week that needs to carry over?
   ```

3. **Generate the weekly plan** using references/weekly-template.md structure:
   - Define 2-3 Weekly Anchors (P0/P1 priority)
   - Map tasks to energy levels (Drain/Neutral/Energize)
   - Schedule deep work blocks (afternoons: 1pm-6pm)
   - Plan evening learning time (7pm-9pm, starting 1hr → 2hrs)
   - Include strategic tasks and connections

4. **Present plan in two formats:**
   - Markdown file for reference
   - Interactive React artifact (optional, if user wants it)

5. **Save to memory** using memory operations:
   - Week number and dates
   - All anchors and their tasks
   - Estimated vs actual time allocations
   - Energy level predictions

**Philosophy to maintain:**
- Sacred morning practice until 1pm (non-negotiable foundation)
- Quality over quantity (20 focused hours > 40 fragmented hours)
- Evening time = competitive advantage (learning while others rest)
- Drain tasks early in week when energy is high
- Neutral tasks mid-week
- Energize tasks as rewards

## Update Weekly Progress

**When:** User reports completed tasks, time spent, or energy levels

**Process:**

1. **Capture progress data:**
   - Task(s) completed ✅
   - Actual time spent vs estimated
   - Actual energy level vs predicted
   - Any insights or observations
   - Next planned action

2. **Update memory** with progress using memory operations

3. **Provide quick feedback:**
   ```
   ✅ Progress saved!
   
   Today's completion: [Task name]
   Time: [X]hrs (estimated [Y]hrs)
   Energy: [Actual level] (predicted [Y])
   
   [If ahead of schedule]: You're ahead of schedule! 🚀
   [If behind schedule]: Still on track for the week's anchors.
   [If energy mismatch]: Note: This task felt [different than expected].
   
   Tomorrow: [Next scheduled task]
   ```

4. **Calculate anchor progress:**
   - Update completion percentages
   - Project completion dates
   - Flag if any anchor is at risk

## Conduct Strategic Growth System Review

**When:** Friday evening, or when user explicitly requests review

**Process:**

1. **Retrieve week's data** from memory:
   - All completed tasks
   - Time estimates vs actuals
   - Energy predictions vs actuals
   - Learning time invested
   - Insights captured

2. **Present Strategic Growth System review** using references/strategic-growth-system.md:
   ```
   ## Your Week [X] Review
   
   ### Anchor Completion
   - Anchor 1: [Status and outcome]
   - Anchor 2: [Status and outcome]
   
   ### What Worked
   - [Patterns of success]
   - [Efficient areas]
   
   ### What to Improve
   - [Challenges faced]
   - [Inefficient areas]
   
   ### Key Insights
   - [Time estimation accuracy]
   - [Energy level patterns]
   - [Learning integration]
   
   ### Next Week Experiments
   - [Suggested adjustments]
   - [New approaches to try]
   ```

3. **Prompt for user input:**
   ```
   30-min reflection time:
   
   1. What was your biggest win this week?
   2. What drained your energy most?
   3. What would you change about next week's plan?
   4. How did your morning practice quality affect your deep work?
   5. What did you learn from evening learning time?
   ```

4. **Save review to memory** and prepare for next week's planning

5. **Ask:** "Ready to plan next week, or would you like to wait until Sunday/Monday?"

## Display Current Week Status

**When:** User asks about their current plan, progress, or schedule

**Process:**

1. **Retrieve current week data** from memory

2. **Display concise status:**
   ```
   ## Week [X] Status
   
   **Anchor 1:** [Name] - [X]% complete
   - ✅ [Completed tasks]
   - 🔄 [In progress]
   - ⏳ [Remaining]
   
   **Anchor 2:** [Name] - [X]% complete
   - ✅ [Completed tasks]
   - 🔄 [In progress]
   - ⏳ [Remaining]
   
   **Today:** [Current day]
   **Scheduled:** [Today's deep work task]
   **Evening:** [Today's learning focus]
   ```

3. **Provide next action:**
   - What should be worked on next
   - Any tasks that need attention
   - Upcoming deadlines or meetings

## References

This skill includes detailed reference materials that are loaded when needed:

### references/weekly-template.md
The complete weekly planning template structure including:
- Anchor project format
- Energy-based task categorization
- Daily schedule blocks
- Learning time integration
- Strategic connections section

**Load when:** Generating new weekly plans

### references/strategic-growth-system.md
The Friday evening review framework including:
- Reflection prompts
- Success pattern identification
- Improvement opportunities
- Experimentation guidelines

**Load when:** Conducting weekly reviews

### references/planning-philosophy.md
Core principles and philosophy of the Weekly Planning System:
- Sacred morning practice foundation
- Energy management strategies
- Quality over quantity principles
- Continuous improvement methodology

**Load when:** User asks about planning methodology or needs guidance