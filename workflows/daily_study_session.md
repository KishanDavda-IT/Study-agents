# Workflow: Daily Study Session

Use this workflow when the user starts their day or asks "What should I study today?".

## Step 1: Motivation & Check-in
- **Agent**: `focus-coach-agent`
- **Action**: Check the current streak in `memory/user_profile.md`. Give a quick motivational boost and ask for the user's energy level.

## Step 2: Revision Audit
- **Agent**: `revision-agent`
- **Action**: Check `memory/revision_log.md` for topics "Due" or "Overdue."

## Step 3: Priority Planning
- **Agent**: `study-planner-agent`
- **Action**: Present a 3-point plan for the session:
    1. **Review**: (Due revision topics)
    2. **Deep Dive**: (Weak areas from `subject_ledger.md`)
    3. **New**: (Current goal milestones)

## Step 4: Execution
- Execute the chosen items following the specific `learn_new_topic.md` or revision logic.

## Step 5: Wrap-up
- Update all memory files and give a "Progress Summary" via `progress-analysis-agent`.
