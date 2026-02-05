# RESUME WORKFLOW - SETUP INSTRUCTIONS

**AI-Powered Multi-Agent Resume Creation System**

Built for Claude.ai Pro or API

---

## WHAT THIS IS

An AI-powered workflow that creates tailored, ATS-compliant resumes that:
- Are 100% factually accurate (validated against your source documents)
- Sound human, not AI-generated
- Are strategically positioned for each role
- Pass all formatting and compliance checks
- Take under 10 minutes to create

**The system uses 8 specialized AI agents:**
1. **Agent 0:** Workflow supervisor (ensures quality)
2. **Agent 1:** Company & job description intelligence
3. **Agent 2:** Job requirements analysis
4. **Agent 3:** Resume draft creation
5. **Agent 4:** Accuracy validation
6. **Agent 5:** AI detection (ensures human voice)
7. **Agent 6:** Voice scoring
8. **Agent 7:** ATS compliance checking
9. **Agent 8:** Cover letter creation (when needed)

---

## QUICK START (30 Minutes)

### Step 1: Fill in Your Templates (20 minutes)

**A. General Resume Template**
1. Open `TEMPLATE_general_resume.md`
2. Replace all `[bracketed text]` with YOUR information
3. Be specific: include numbers, dates, achievements
4. Save as: `yourname_general_resume.md`

**B. Quick Reference Template**
1. Open `TEMPLATE_quick_reference.md`
2. Fill in YOUR facts exactly as they should appear
3. This is your accuracy validator - be precise
4. Save as: `RESUME_QUICK_REFERENCE.md`

**C. Value Breakdown Template**
1. Open `TEMPLATE_value_breakdown.md`
2. Calculate YOUR documented value delivery
3. Show your math and be conservative
4. Save as: `CUMULATIVE_VALUE_BREAKDOWN.md`

### Step 2: Upload to Claude.ai (5 minutes)

1. Go to https://claude.ai
2. Click "Projects" in left sidebar
3. Click "Create Project"
4. Name it: "Resume Workflow"
5. Click "Add Content" → "Upload files"
6. Upload these files:
   - `yourname_general_resume.md`
   - `RESUME_QUICK_REFERENCE.md`
   - `CUMULATIVE_VALUE_BREAKDOWN.md`
   - `agent_0_supervisor.md` through `agent_8_cover_letter_creator.md` (9 files)
   - `TRIPLE_LENS_FRAMEWORK.md`

### Step 3: Configure Project Instructions (2 minutes)

In your Project settings, add this to "Custom Instructions":

```
You are a resume creation specialist using the Agent 0 Supervisor workflow.

For all resume requests:
1. Run Agent 0 Supervisor workflow
2. Execute agents 1-8 sequentially
3. Validate all outputs
4. Present final resume only after all agents pass

Use the general resume, quick reference, and value breakdown files as source of truth.
```

### Step 4: Test It (3 minutes)

In your project chat, say:

```
Create a resume for [job title] at [company name]

[Paste job description]
```

Watch the agents execute. You should see:
- Agent 1: Company intelligence gathering
- Agent 2: Job description analysis
- Agents 3-7: Draft creation and validation
- Final resume presented after all checks pass

---

## HOW TO USE

### Creating a Tailored Resume

**Step 1: Find a Job**
- Copy the complete job description
- Note the company name and role title

**Step 2: Submit to Claude**
In your Resume Workflow project, say:

```
Create a resume for [Job Title] at [Company Name]

[Paste entire job description here]
```

**Step 3: Review Output**
Claude will present a validated resume showing:
- ✅ Agent 1 Complete: Company intelligence gathered
- ✅ Agent 2 Complete: JD analyzed
- ✅ Agent 3 Complete: Draft created
- ✅ Agent 4 Complete: Accuracy validated (100%)
- ✅ Agent 5 Complete: AI detection passed
- ✅ Agent 6 Complete: Voice score: [X]/12
- ✅ Agent 7 Complete: ATS compliant

**Step 4: Request File Creation** (Optional)
If you want to save the file:
```
Save this resume as a file
```

Claude will create a `.md` file you can download.

**Step 5: Convert to Word/PDF**
- Download the `.md` file
- Convert to `.docx` using Word or Google Docs
- Or convert to PDF using any markdown converter

### Creating a Cover Letter

For executive roles or career transitions:

```
Create a cover letter for the [Company] [Role] position
```

Claude will create a 300-400 word cover letter using the company intelligence and job analysis.

---

## UNDERSTANDING THE WORKFLOW

### What Happens Behind the Scenes

**Agent 0 (Supervisor):**
- Enforces sequential execution
- No shortcuts allowed
- Ensures all validation passes

**Agent 1 (Company Intelligence):**
- Web searches for company info
- Finds revenue, size, recent news
- Identifies strategic priorities
- Creates positioning strategy

**Agent 2 (JD Analysis):**
- Analyzes requirements
- Creates alignment map (Strong/Partial/Gap)
- Prioritizes keywords for ATS
- Provides hiring manager perspective

**Agent 3 (Draft Creator):**
- Starts with your general resume
- Modifies only 20% for this role
- Integrates keywords and positioning
- Applies three-lens framework:
  - Resume Consultant: Can you defend this?
  - Executive Hiring Manager: Does this grab attention?
  - Soundboard: What could be stronger?

**Agent 4 (Accuracy Validator):**
- Checks EVERY number against Quick Reference
- Catches any fabrications
- Must achieve 100% accuracy
- Fails resume if anything doesn't match

**Agent 5 (AI Detection):**
- Reads resume "aloud" mentally
- Checks for AI garbage phrases
- Ensures logical consistency
- Validates claims are defensible

**Agent 6 (Voice Scorer):**
- Scores for human voice (12-point scale)
- Checks conversational tone
- Validates executive language without buzzwords
- Must score 10+/12 to pass

**Agent 7 (ATS Checker):**
- Validates formatting compliance
- Checks word count (≤760 words)
- Ensures no pipes (|), tables, or columns
- Verifies job titles use commas not dashes

**Agent 8 (Cover Letter):**
- Creates cover letters when requested
- Uses company intelligence + JD analysis
- Self-validates before presenting
- 300-400 words max

### The Three-Lens Framework

Every decision uses three perspectives:

**Lens 1: Resume Consultant**
"Can you defend this in an interview?"
- Checks if claims are specific enough
- Validates you can back up every statement
- Ensures nothing fabricated

**Lens 2: Executive Hiring Manager**
"Does this grab attention in 10 seconds?"
- Checks if resume stands out
- Validates executive-level positioning
- Ensures keywords are front-loaded

**Lens 3: Soundboard/Thinking Partner**
"What could make this stronger?"
- Challenges generic language
- Suggests more specific metrics
- Identifies missed opportunities

---

## MAINTENANCE

### When to Update Your Files

**Update `yourname_general_resume.md` when:**
- You complete a new major achievement
- You change jobs or get promoted
- You refine how you describe past work
- You learn to articulate value better

**Update `RESUME_QUICK_REFERENCE.md` when:**
- You change jobs (add new role section)
- Numbers change (new budget, team size)
- You complete quantifiable achievements
- Your terminology preferences change

**Update `CUMULATIVE_VALUE_BREAKDOWN.md` when:**
- You deliver new value (add to total)
- You refine your calculations
- You prepare for interviews (add defense notes)

### Quality Assurance

The system has built-in quality checks:

**Agent 4 catches:**
- Wrong dates or titles
- Fabricated numbers
- Inconsistent facts
- Misremembered details

**Agent 5 catches:**
- AI-generated language
- Corporate buzzwords
- Logical inconsistencies
- Defensive positioning

**Agent 6 catches:**
- Robotic tone
- Lack of conversational flow
- Over-polished language
- Generic executive speak

**Agent 7 catches:**
- ATS-unfriendly formatting
- Word count violations
- Unsupported file structure
- Title formatting issues

---

## TROUBLESHOOTING

### Problem: Resume has wrong facts

**Solution:**
1. Check `RESUME_QUICK_REFERENCE.md` - are your facts correct there?
2. Check `yourname_general_resume.md` - does it match Quick Reference?
3. Agent 4 only passes resumes that match Quick Reference exactly

### Problem: Resume sounds too AI/corporate

**Solution:**
1. Review your `yourname_general_resume.md`
2. Make it more conversational (use "I've" instead of "I have")
3. Remove buzzwords from source resume
4. Agents 5 and 6 will catch AI language if source is clean

### Problem: Resume not passing ATS

**Solution:**
1. Check Agent 7 validation report
2. Common issues:
   - Using pipes (|) in text
   - Two-column layouts
   - Tables or graphics
   - Job titles with dashes instead of commas
3. The system should catch these automatically

### Problem: Resume seems too generic

**Solution:**
1. Agent 2 might not have enough JD details to work with
2. Try providing more context about the role
3. Your general resume might need more specific metrics
4. Add more quantified achievements to source resume

### Problem: Claude says it can't find files

**Solution:**
1. Verify files are uploaded to Project Knowledge
2. Check file names match exactly (case-sensitive)
3. Re-upload if necessary
4. Make sure you're in the "Resume Workflow" project

---

## ADVANCED USAGE

### Creating Multiple Resumes Quickly

For high-volume applications (5-10 per day):

1. Gather all job descriptions first
2. Create resumes in batch:
   ```
   Create resume for Company A [JD]
   Create resume for Company B [JD]
   Create resume for Company C [JD]
   ```
3. Claude will process sequentially
4. Review and save each one

**Target:** Under 10 minutes per resume

### Customizing Agent Behavior

You can modify agent behavior by editing the agent `.md` files:

**Example: Stricter voice scoring**
Edit `agent_6_voice_scorer.md`:
- Change passing score from 10/12 to 11/12
- Add additional voice criteria

**Example: Different word count limit**
Edit `agent_7_ats_checker.md`:
- Change 760-word limit to your preference

**Example: Industry-specific keywords**
Edit `agent_2_jd_analysis.md`:
- Add industry-specific keyword lists
- Customize for your target sector

### Using for Different Experience Levels

The system works for any level:

**Individual Contributor (IC):**
- Focus more on technical details
- Include hands-on achievements
- Less emphasis on team management

**Manager/Director:**
- Balance technical and leadership
- Include team sizes and budgets
- Show both execution and strategy

**VP/C-Suite:**
- Pure strategy and business outcomes
- Minimal technical detail
- Board-level thinking

Adjust your `general_resume.md` accordingly.

---

## SYSTEM REQUIREMENTS

**Required:**
- Claude.ai Pro account ($20/month) OR Claude API access
- Web browser (Chrome, Firefox, Safari, Edge)
- Markdown viewer or converter (for final files)

**Optional but Recommended:**
- Microsoft Word (for .docx conversion)
- Google Docs (alternative converter)
- LinkedIn Premium (for better job search)

**Usage Metrics:**
- Average: 1,500-2,000 tokens per resume
- Time: 8-12 minutes per resume
- Cost: Included in Pro subscription or ~$0.03-0.05 per resume via API

---

## BEST PRACTICES

### Writing Your General Resume

**Do:**
- Be specific with numbers (team size, budget, users)
- Use leadership language (Led, Directed, Managed)
- Focus on business outcomes, not technical tasks
- Include scale indicators in every bullet
- Write conversationally ("I've" not "I have")

**Don't:**
- Use corporate buzzwords (synergy, leverage, utilize)
- Write in third person
- Be vague about scope ("large team" → "30+ professionals")
- Lead with technology instead of business value
- Fabricate or exaggerate

### Positioning for Different Roles

**For higher-level roles:**
- Lead with strategy and business outcomes
- De-emphasize technical details
- Show P&L responsibility
- Include C-suite interactions

**For career transitions:**
- Emphasize transferable skills
- Show regulated environment experience
- Highlight business partnerships
- Position gaps honestly

**For stretch roles:**
- Lead with scope, not title
- Show you've done the work even if title doesn't reflect it
- Emphasize scale of responsibility
- Include "acted as de facto [role]" if true

---

## FAQ

**Q: Can I use this for cover letters?**
A: Yes, Agent 8 creates cover letters. Just say "Create a cover letter for [Company] [Role]"

**Q: How do I know if my resume is ATS-compliant?**
A: Agent 7 validates this automatically. If it passes Agent 7, it's ATS-compliant.

**Q: Can I customize the workflow?**
A: Yes, you can edit any agent `.md` file to change behavior. Just be careful not to break the validation logic.

**Q: What if I don't have $100M in value like the examples?**
A: That's fine! Document YOUR actual value. The system works with any level of achievements. Be honest and conservative.

**Q: Can I use this for LinkedIn optimization?**
A: The system is designed for resumes, but your `general_resume.md` can inform your LinkedIn profile. The core achievements are the same.

**Q: How often should I update my source files?**
A: Update when you complete major achievements, change jobs, or refine your value calculations. Quarterly review is a good cadence.

**Q: What if I'm early career with limited achievements?**
A: Focus on what you HAVE done. Even small projects can be quantified. The system works for any career stage.

**Q: Can multiple people use this system?**
A: Yes! Each person needs their own Claude project with their own source files. The agent files are universal.

---

## SUPPORT & FEEDBACK

**Found a bug?**
- Open an issue on GitHub
- Include the agent that failed and error message

**Have a suggestion?**
- Open a feature request on GitHub
- Describe the improvement and use case

**Want to contribute?**
- Fork the repository
- Submit pull requests for improvements
- Share your agent customizations

---

## WHAT'S NEXT?

**After creating your first resume:**
1. Apply to 5-10 jobs using your tailored resumes
2. Track which versions get interviews
3. Refine your general resume based on feedback
4. Update your value calculations as you learn to defend them better

**Advanced workflows to explore:**
- Batch processing (10 resumes in 90 minutes)
- Industry-specific customizations
- Executive positioning for C-suite roles
- Career transition strategies

---

**You're ready to go. Start with the Quick Start section and create your first tailored resume in under 30 minutes.**
