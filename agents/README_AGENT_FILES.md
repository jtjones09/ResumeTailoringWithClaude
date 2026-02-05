# AGENT FILES - MANUAL STEP REQUIRED

## Important Note

The 9 agent files (agent_0 through agent_8) and the TRIPLE_LENS_FRAMEWORK.md file are currently in your Claude Project Knowledge and need to be exported manually.

## How to Get These Files:

### Option 1: Download from Project (Recommended)
1. Go to your Claude Project
2. Click "Knowledge" tab
3. Download each file:
   - agent_0_supervisor.md
   - agent_1_company_jd_intelligence.md
   - agent_2_jd_analysis.md
   - agent_3_draft_creator.md
   - agent_4_accuracy_validator.md
   - agent_5_read_what_you_wrote.md
   - agent_6_voice_scorer.md
   - agent_7_ats_checker.md
   - agent_8_cover_letter_creator.md
   - TRIPLE_LENS_FRAMEWORK.md

4. Move them to the `agents/` directory
5. Move TRIPLE_LENS_FRAMEWORK.md to `frameworks/` directory

### Option 2: Ask Claude to Recreate
Ask Claude in your project:
```
Please create all 9 agent files and save them to /mnt/user-data/outputs/resume-workflow/agents/

Also create TRIPLE_LENS_FRAMEWORK.md and save to /mnt/user-data/outputs/resume-workflow/frameworks/
```

## Files Needed:

**In `agents/` directory:**
1. agent_0_supervisor.md
2. agent_1_company_jd_intelligence.md
3. agent_2_jd_analysis.md
4. agent_3_draft_creator.md
5. agent_4_accuracy_validator.md
6. agent_5_read_what_you_wrote.md
7. agent_6_voice_scorer.md
8. agent_7_ats_checker.md
9. agent_8_cover_letter_creator.md

**In `frameworks/` directory:**
1. TRIPLE_LENS_FRAMEWORK.md

## Once You Have All Files:

Your directory structure should look like:
```
resume-workflow/
├── README.md ✓
├── SETUP_INSTRUCTIONS.md ✓
├── TEMPLATE_general_resume.md ✓
├── TEMPLATE_quick_reference.md ✓
├── TEMPLATE_value_breakdown.md ✓
├── agents/
│   ├── agent_0_supervisor.md [NEED]
│   ├── agent_1_company_jd_intelligence.md [NEED]
│   ├── agent_2_jd_analysis.md [NEED]
│   ├── agent_3_draft_creator.md [NEED]
│   ├── agent_4_accuracy_validator.md [NEED]
│   ├── agent_5_read_what_you_wrote.md [NEED]
│   ├── agent_6_voice_scorer.md [NEED]
│   ├── agent_7_ats_checker.md [NEED]
│   └── agent_8_cover_letter_creator.md [NEED]
└── frameworks/
    └── TRIPLE_LENS_FRAMEWORK.md [NEED]
```

Then you're ready to publish to GitHub!
