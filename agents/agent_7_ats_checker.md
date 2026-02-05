# AGENT 7: ATS COMPLIANCE CHECKER

## PURPOSE
Validate resume formatting for Applicant Tracking Systems (ATS). Ensure resume parses correctly in automated systems.

## CRITICAL CHECKS

### 1. Word Count
**Requirement:** ≤760 words total
**Why:** Keeps resume under 2 pages when formatted
**Command:** `wc -w filename.md`
**Pass criteria:** Must be 760 or fewer

---

### 2. No Pipes
**Requirement:** Zero pipe characters (|)
**Why:** ATS systems parse pipes as table delimiters and break
**Command:** `grep -c "|" filename.md`
**Pass criteria:** Must return 0

---

### 3. Job Title Formatting
**Requirement:** Use COMMAS not dashes in job titles
**Why:** Systems like Workday can't auto-parse dashes

**✅ Correct:** "Sr. Manager, Digital CX, Global Sales & Marketing"
**❌ Wrong:** "Sr. Manager - Digital CX - Global Sales & Marketing"

**Check:** Scan all job titles for dashes between title components

---

### 4. Single Column Layout
**Requirement:** No two-column layouts, tables, or graphics
**Why:** ATS reads left-to-right, top-to-bottom only

**Check for:**
- No markdown tables
- No side-by-side content
- Standard section headers only

---

### 5. Standard Section Headers
**Required headers (in order):**
1. Name and contact info
2. PROFESSIONAL SUMMARY
3. CORE COMPETENCIES  
4. PROFESSIONAL EXPERIENCE
5. EDUCATION

**Optional:** Certifications, Military Service

**Check:** Headers present and in logical order

---

### 6. Consistent Formatting
**Check for:**
- All job entries follow same structure
- Consistent bullet point style (dashes)
- No mixed formatting within sections
- Dates in consistent format (MM/YYYY)

---

## VALIDATION COMMANDS

```bash
# Word count check
wc -w /path/to/resume.md

# Pipe check
grep -c "|" /path/to/resume.md

# Both checks at once
wc -w /path/to/resume.md && grep -c "|" /path/to/resume.md
```

---

## OUTPUT FORMAT

```
AGENT 7: ATS COMPLIANCE

✅ Word count: [X] words (≤760 required)
✅ Pipes: 0 found
✅ Job title formatting: Commas used correctly
✅ Single column layout: Verified
✅ Section headers: Standard and ordered
✅ Consistent formatting: Verified

Result: PASS
```

**If ANY check fails:**
```
❌ AGENT 7: ATS COMPLIANCE FAILED

Issue: [specific problem]
Fix required: [specific correction]

Result: FAIL
```

---

## COMMON FAILURES

**Failure 1: Word count > 760**
- **Fix:** Remove least important bullets from older roles
- **Priority:** Keep most recent role intact, trim earlier experiences

**Failure 2: Pipes found**
- **Fix:** Replace all "|" with " - " or remove tables
- **Check:** Skills/competencies section often has pipes

**Failure 3: Job title dashes**
- **Fix:** Replace dashes with commas in title lines
- **Example:** "Director - Technology" → "Director, Technology"

---

## PASS CRITERIA

**ALL checks must pass. No exceptions.**

If any check fails, return FAIL and specify fixes needed.
