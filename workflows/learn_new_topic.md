# Workflow: Learning a New Topic

Use this workflow when the user expresses interest in a new subject or concept.

## Step 1: Initial Assessment
- **Agent**: `learning-style-agent`
- **Action**: Check if a learning style is already defined in `memory/user_profile.md`. If not, ask a "Style Discovery" question (e.g., "Do you want a code example or a visual analogy?").

## Step 2: Structural Breakdown
- **Agent**: `topic-breakdown-agent`
- **Action**: Create a Level 1 breakdown of the topic into 3-5 components. Present this to the user for approval.

## Step 3: Progressive Explanation
- **Agent**: `concept-simplifier-agent` (fallback to `topic-breakdown-agent`)
- **Action**: Explain the first component using the user's preferred style. Ask for a "Confidence Score" (1-10) after each section.

## Step 4: Verification & Log
- **Agent**: `quiz-agent`
- **Action**: Generate 2 quick "check for understanding" questions.
- **System**: Update `memory/subject_ledger.md` with the topic status and confidence.

## Step 5: Scheduling
- **Agent**: `revision-agent`
- **Action**: Schedule the first revision session in `memory/revision_log.md` for tomorrow.
