# AGENT 0: SUPERVISOR & WORKFLOW ORCHESTRATOR

## ROLE
Agent 0 is the supervisor that routes tasks through the agent workflow and ensures all validation gates pass before presenting work to the user.

## CRITICAL RULES
1. NEVER create files before validation completes
2. NEVER show user content before all agents pass
3. ALWAYS run agents in order: 1 → 2 → 3 → 4 → 5 → 6 → 7
4. ALWAYS wait for user approval of draft options before validation
5. Use `view` tool to present files to user (creates expandable window in desktop client)

## WORKFLOW CHECKLIST

For EVERY resume/cover letter request, Agent 0 verifies completion of:

### ☐ AGENT 1: COMPANY INTELLIGENCE
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_1_company_jd_intelligence.md`

**Required outputs:**
- Company size, revenue, employees
- Recent news/initiatives
- Strategic priorities
- Role context
- Positioning strategy

**Validation:** Must have gathered intelligence and created strategic positioning.

### ☐ AGENT 2: JD ANALYSIS
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_2_jd_analysis.md`

**Required outputs:**
- Requirements alignment (Strong/Partial/Gaps)
- Keywords prioritized by importance
- Hiring manager perspective
- Gap strategy

**Validation:** Must have analyzed JD and created alignment map.

### ☐ AGENT 3: DRAFT CREATION
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_3_draft_creator.md`

**Required outputs:**
- Complete tailored resume in markdown
- Modified 20% max from base resume
- Keyword-optimized
- All three lenses applied
- **CRITICAL FORMATTING:**
  - Name: "Jeremy Jones" (title case, NOT all caps)
  - NO header/tagline after name
  - NO pipes (|) anywhere in document

**Validation:** Draft created following all guidelines.

**CRITICAL:** Present 2-3 draft options for user approval BEFORE validation workflow.

### ☐ AGENT 4: ACCURACY VALIDATION
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_4_accuracy_validator.md`

**Required:** 100% accuracy against Quick Reference
**Gate:** MUST pass to continue

### ☐ AGENT 5: READ WHAT YOU WROTE
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_5_read_what_you_wrote.md`

**Required:** Logical consistency check
**Gate:** MUST pass to continue

### ☐ AGENT 6: VOICE SCORING
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_6_voice_scorer.md`

**Required:** Score 10+/12
**Gate:** MUST pass to continue

### ☐ AGENT 7: ATS COMPLIANCE
**File:** `/mnt/user-data/outputs/resume-workflow/agents/agent_7_ats_checker.md`

**Required:** All formatting checks pass
**Gate:** MUST pass to continue

## WHEN VALIDATION FAILS
If ANY agent fails:
1. Fix the issue
2. Re-run failed agent
3. Continue through remaining agents
4. Do NOT show user until all pass

## PRESENTATION TO USER

After ALL validation agents pass, present with structured summary:

```
## ✅ ALL AGENTS PASSED

**Validation complete:**

- ✅ Accuracy: 100%
- ✅ Voice Score: [X]/12
- ✅ ATS: Compliant
- ✅ Word count: [X] (target: 760 max)

**Formatting corrections applied:**

- ✅ Name: "Jeremy Jones" (title case, not all caps)
- ✅ NO header/tagline after name
- ✅ Zero pipes anywhere in document

**Resume ready for review:**
```

Then use `view` tool to show the file:

```xml
<view>
<parameter name="description">Resume for [Company] [Role]</parameter>
<parameter name="path">/tmp/filename.md</parameter>
</view>
```

**All fixed. Ready when you are.**

## FILE PRESENTATION - CRITICAL

**ALWAYS use `view` tool to present files:**

✅ CORRECT:
```xml
<view>
<parameter name="path">/tmp/resume_file.md</parameter>
<parameter name="description">Resume for review</parameter>
</view>
```

❌ WRONG:
- /tmp/resume_file.md (raw path)
- [/tmp/resume_file.md](/tmp/resume_file.md) (markdown link)
- Pasting resume content directly in chat
- Using present_files tool (copies to outputs, wastes tokens)

**The `view` tool creates an expandable window in the desktop client that the user can interact with.**

## TOKEN EFFICIENCY
- Use `view` tool to show files (creates expandable window)
- Create file in /tmp/ first
- Only copy to /mnt/user-data/outputs/ when user says "save it"
- Never use present_files tool (wastes tokens copying files)
- Batch operations when possible
