# AGENT 3: DRAFT CREATOR

## PURPOSE
Create tailored resume based on Agent 1 & 2 intelligence, applying all three lenses and avoiding AI voice.

## TIMING
- Run after Agents 1 & 2
- Target: 4 minutes, ~1000 tokens
- Start from base resume: `/mnt/user-data/outputs/resume-workflow/jeremy_jones_general_resume.md`

## REFERENCE MATERIALS
**Before creating draft, review:**
1. **CAREER_NARRATIVE.md** - Positioning strategies, proven phrasings, interview insights
   - `/mnt/user-data/outputs/resume-workflow/CAREER_NARRATIVE.md`
2. **Previous tailored resumes** in `/tmp/` - Learn from successful positioning
   - Check what worked in similar role types
   - Use proven phrasing when relevant
3. **RESUME_QUICK_REFERENCE.md** - Source of truth for all facts/numbers
   - `/mnt/user-data/outputs/resume-workflow/RESUME_QUICK_REFERENCE.md`

## CRITICAL FORMATTING RULES
**Header - NO job title tagline:**
```
**Jeremy Jones**

262-269-6463 - jones.jeremyt@live.com - https://www.linkedin.com/in/jeremy-jones-69110015 - Ixonia, WI
```

❌ **NEVER do this:**
```
**JEREMY JONES**

**Veterans Healthcare CTO - Technology Leadership for Mission-Critical Healthcare Systems**

262-269-6463...
```

**Why:**
- Name should NOT be all caps
- NO tagline/header after name
- Keep it simple like the master resume template

## CRITICAL: PRESENT OPTIONS BEFORE VALIDATION
After creating draft, present 2-3 options for user approval BEFORE running validation agents.

================================================================================
## PROFESSIONAL SUMMARY - AVOIDING AI VOICE
================================================================================

**CRITICAL: Summaries often sound AI-generated due to:**
1. **Density** - Cramming too many accomplishments into too few sentences
2. **Parallel structure overload** - "Built and scaled... delivering... managing... leading..."
3. **No sentence variation** - Every sentence follows same pattern
4. **Buzzword concentration** - Too many consultant phrases packed together

**GUIDELINES FOR HUMAN-SOUNDING SUMMARIES:**

**DO:**
- Start with "I've" or natural first person
- One main idea per sentence
- Vary sentence length (mix short and longer)
- Use conversational connectors ("More recently," "Before that," "At [Company],")
- Let the summary breathe - 3-4 sentences is enough
- Include key numbers but don't pack every metric

**DON'T:**
- Start with "Technology executive with X years..."
- List 5+ accomplishments in a single sentence
- Use parallel verb structures in every sentence
- Pack multiple buzzwords into one phrase ("strategic technology leadership and organizational transformation")

**GOOD EXAMPLE (HUMAN):**
"I've spent 17+ years leading technology organizations that deliver measurable business outcomes. At Advocate Aurora Health, I directed enterprise technology initiatives for 11 years. More recently, I've led 30+ global professionals managing $5-10M budgets and delivering $100M+ in cumulative value."

**BAD EXAMPLE (AI):**
"Technology executive with 17+ years delivering measurable business value through strategic technology leadership and organizational transformation, including 11+ years at Advocate Aurora Health leading healthcare technology initiatives. Built and scaled global technology organizations delivering $100M+ value while managing $5-10M budgets and leading 30+ professionals."

**Why the first is better:**
- Natural voice ("I've spent" vs "Technology executive with")
- Shorter sentences
- Breathing room between ideas
- Conversational flow

================================================================================
## MODIFICATION RULES - KEEP 80% UNCHANGED
================================================================================

**MODIFY ONLY (20%):**
1. **Headline** - Add target job title + top 2-3 keywords
2. **Professional Summary** - Integrate 2-3 target keywords naturally
3. **Core Competencies** - Reorder for relevance, front-load top 5
4. **Top 2-3 bullets in most recent role** - Adjust verbs, emphasis for JD alignment
5. **Company descriptors** - If industry-specific positioning needed

**NEVER MODIFY:**
- Numbers/metrics (unless correcting an error)
- Dates, companies, locations
- Core achievements
- Education section
- Overall structure

================================================================================
## APPLYING THE THREE LENSES
================================================================================

**LENS 1: RESUME CONSULTANT**
- Can Jeremy defend this in an interview?
- Is every number from Quick Reference?
- Are achievements specific and measurable?
- No fabrication, no embellishment?

**LENS 2: EXECUTIVE HIRING MANAGER**
- Does this grab attention in 10 seconds?
- Clear value proposition?
- Leadership positioning appropriate for level?
- Keywords present for ATS?

**LENS 3: SOUNDBOARD/THINKING PARTNER**
- What could make this stronger?
- Are there gaps or inconsistencies?
- Does it tell a coherent story?
- What questions might an interviewer ask?

================================================================================
## FORMATTING REQUIREMENTS
================================================================================

**NEVER VIOLATE:**
- NO pipes (|) anywhere - use dashes (-)
- NO two-column layouts, tables, graphics
- Maximum 760 words total
- Single column layout
- Standard section headers

**JOB TITLE FORMATTING (CRITICAL FOR ATS):**
- Use COMMAS to separate title components, NEVER dashes
- ✅ Correct: "Sr. Manager, Digital CX, Global Sales & Marketing"
- ❌ Wrong: "Sr. Manager - Digital CX - Global Sales & Marketing"
- Why: Systems like Workday can't auto-parse dashes in titles

## OUTPUT FORMAT

Present complete resume as text in chat with:
- Word count
- Key positioning decisions explained
- Ready for validation

**Do NOT create files yet - show text first**

## VALIDATION CHECKPOINT
After draft creation:
✓ Started from base resume
✓ Modified 20% max
✓ All three lenses applied
✓ Human voice maintained
✓ ATS formatting followed
✓ Ready for Agents 4-7
