# AI-Powered Resume Workflow

**Create tailored, ATS-compliant resumes in under 10 minutes using Claude.ai**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude.ai](https://img.shields.io/badge/Built%20for-Claude.ai-blue)](https://claude.ai)

---

## 🎯 What This Does

An AI-powered multi-agent system that creates professional, tailored resumes that are:

✅ **100% Factually Accurate** - Validated against your source documents  
✅ **Human Voice** - Not AI-generated corporate speak  
✅ **ATS-Compliant** - Passes applicant tracking systems  
✅ **Strategically Positioned** - Customized for each role  
✅ **Fast** - Under 10 minutes per resume  

Built for **Claude.ai Pro** or API access.

---

## 🚀 Quick Start (30 Minutes)

### 1. Clone This Repository
```bash
git clone https://github.com/yourusername/resume-workflow.git
cd resume-workflow
```

### 2. Fill in Your Templates
- `TEMPLATE_general_resume.md` → Your complete career history
- `TEMPLATE_quick_reference.md` → Your facts for accuracy checking
- `TEMPLATE_value_breakdown.md` → Your quantified achievements

Rename after filling:
- `yourname_general_resume.md`
- `RESUME_QUICK_REFERENCE.md`
- `CUMULATIVE_VALUE_BREAKDOWN.md`

### 3. Upload to Claude.ai
1. Create a new **Project** in Claude.ai
2. Name it "Resume Workflow"
3. Upload all `.md` files to Project Knowledge
4. Add custom instructions (see [SETUP_INSTRUCTIONS.md](SETUP_INSTRUCTIONS.md))

### 4. Create Your First Resume
```
Create a resume for Senior Director of Technology at Microsoft

[Paste job description]
```

Watch the 8-agent workflow execute and validate your resume automatically.

---

## 🤖 How It Works

The system uses **8 specialized AI agents** that run sequentially:

| Agent | Function | Output |
|-------|----------|--------|
| **Agent 0** | Workflow Supervisor | Enforces quality, no shortcuts |
| **Agent 1** | Company Intelligence | Web research on company/role |
| **Agent 2** | JD Analysis | Requirements alignment map |
| **Agent 3** | Draft Creator | Tailored resume (modifies 20% max) |
| **Agent 4** | Accuracy Validator | 100% fact-checking |
| **Agent 5** | AI Detection | Removes AI-generated language |
| **Agent 6** | Voice Scorer | Ensures human tone (10+/12 required) |
| **Agent 7** | ATS Checker | Validates formatting compliance |
| **Agent 8** | Cover Letter | Creates cover letters when needed |

### The Three-Lens Framework

Every decision is evaluated through three perspectives:

1. **Resume Consultant** - "Can you defend this in an interview?"
2. **Executive Hiring Manager** - "Does this grab attention in 10 seconds?"
3. **Soundboard** - "What could make this stronger?"

---

## 📊 Features

### Accuracy & Quality
- **Validation Against Source** - Every fact checked against your Quick Reference
- **No Fabrication** - Agent 4 rejects any unverifiable claims
- **Human Voice Detection** - Agents 5 & 6 catch AI-generated corporate speak
- **ATS Compliance** - Agent 7 ensures formatting passes applicant tracking systems

### Strategic Positioning
- **Company Intelligence** - Automated web research on target company
- **Keyword Optimization** - JD analysis extracts and prioritizes keywords
- **Gap Strategy** - Honest positioning for career transitions or stretch roles
- **Executive Language** - Uses bold claims when justified by facts

### Efficiency
- **Fast** - Under 10 minutes per tailored resume
- **Consistent** - Same input + same JD = same output every time
- **Batch Processing** - Create 5-10 resumes per session
- **Token Efficient** - ~1,500-2,000 tokens per resume

---

## 📁 Repository Structure

```
resume-workflow/
├── README.md                          # This file
├── SETUP_INSTRUCTIONS.md              # Detailed setup guide
├── LICENSE                            # MIT License
├── .gitignore                        # Git ignore rules
│
├── templates/                         # Fill these out first
│   ├── TEMPLATE_general_resume.md    # Your master resume
│   ├── TEMPLATE_quick_reference.md   # Facts for validation
│   └── TEMPLATE_value_breakdown.md   # Interview prep
│
├── agents/                            # The 8-agent system
│   ├── agent_0_supervisor.md         # Workflow enforcer
│   ├── agent_1_company_jd_intelligence.md
│   ├── agent_2_jd_analysis.md
│   ├── agent_3_draft_creator.md
│   ├── agent_4_accuracy_validator.md
│   ├── agent_5_read_what_you_wrote.md
│   ├── agent_6_voice_scorer.md
│   ├── agent_7_ats_checker.md
│   └── agent_8_cover_letter_creator.md
│
├── frameworks/                        # Decision framework
│   └── TRIPLE_LENS_FRAMEWORK.md
│
└── examples/                          # Example outputs
    ├── example_resume.md
    └── example_cover_letter.md
```

---

## 💡 Use Cases

### Job Seekers
- **High-Volume Applications** - Create 5-10 tailored resumes daily
- **Career Transitions** - Position for roles outside your industry
- **Executive Roles** - Strategic positioning for C-suite/VP roles

### Recruiters & Career Coaches
- **Client Services** - Fast, high-quality resume creation
- **Template Management** - Consistent quality across clients
- **Value Demonstration** - Show quantified achievements

### Teams & Organizations
- **Internal Mobility** - Help employees apply for internal roles
- **Outplacement Services** - Support laid-off employees
- **Career Development** - Teach quantified achievement thinking

---

## 🎓 Examples

### Before (Generic Resume)
```
• Managed technology projects and led team initiatives
• Worked with stakeholders to deliver solutions
• Improved processes and reduced costs
```

### After (Tailored & Validated)
```
• Directed team to build analytical capabilities analyzing distributor 
  transactions in SAP, identifying hidden revenue leakage from upsells. 
  Recovered $27M in annual revenue.
• Managed strategic vendor partnerships across Salesforce ecosystem, 
  negotiating contracts that delivered 30% reduction in licensing costs.
• Led crisis response deploying mobile health screening solution in 30 days, 
  generating $1M+ monthly savings across 40,000+ healthcare workforce.
```

**Key Differences:**
- Specific numbers (not "reduced costs" but "$27M")
- Defensible claims (can explain in interview)
- Business outcomes (not just activities)
- Leadership language (Directed, Managed, Led)

---

## 🔧 Requirements

**Required:**
- **Claude.ai Pro** ($20/month) OR Claude API access
- Web browser (Chrome, Firefox, Safari, Edge)
- Markdown editor (VSCode, Typora, or any text editor)

**Optional:**
- Microsoft Word or Google Docs (for .docx conversion)
- Markdown to PDF converter

**System:**
- No installation needed
- Works entirely in Claude.ai
- Files stored in your Claude Project

---

## 📖 Documentation

- **[SETUP_INSTRUCTIONS.md](SETUP_INSTRUCTIONS.md)** - Complete setup guide (30 min)
- **[TRIPLE_LENS_FRAMEWORK.md](frameworks/TRIPLE_LENS_FRAMEWORK.md)** - Decision framework
- **Agent Documentation** - Each agent has inline docs in its `.md` file

---

## 🤝 Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

**Areas for contribution:**
- Additional agent customizations
- Industry-specific templates
- Alternative validation strategies
- Integration with other AI platforms
- Example resumes and case studies

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

Built by someone who got tired of:
- Spending hours customizing each resume
- AI tools that fabricate accomplishments
- Generic resumes that don't stand out
- Wondering if resumes would pass ATS
- Corporate buzzword-filled AI outputs

This system solves all of those problems.

---

## ⚠️ Disclaimer

**This tool helps you create resumes, but it doesn't:**
- Guarantee job offers (networking and skills still matter)
- Write resumes for you (you must fill in the templates)
- Replace human judgment (you review all outputs)
- Fabricate achievements (100% accuracy validation)

**Use responsibly:**
- Only include facts you can defend in interviews
- Be conservative with value calculations
- Review and approve every resume before sending
- Remember: The best resume is one that represents YOU accurately

---

## 📊 Stats

- **Development Time:** 40+ hours of prompt engineering
- **Resumes Created:** 100+ (during development)
- **Average Time:** 8-12 minutes per resume
- **Accuracy Rate:** 100% (by design - Agent 4 rejects inaccurate resumes)
- **ATS Pass Rate:** ~95% (based on testing)

---

## 🗺️ Roadmap

**v1.1 (Current)**
- ✅ 8-agent validation system
- ✅ Three-lens framework
- ✅ Cover letter generation
- ✅ ATS compliance checking

**v1.2 (Coming Soon)**
- [ ] LinkedIn profile optimization agent
- [ ] Interview prep generator
- [ ] Salary negotiation guidance
- [ ] Network outreach templates

**v2.0 (Future)**
- [ ] API integration for job boards
- [ ] Auto-apply functionality
- [ ] Portfolio website generation
- [ ] Video interview prep

---

## 💬 Support

**Questions? Issues?**
- Open an [Issue](https://github.com/yourusername/resume-workflow/issues)
- Check [Discussions](https://github.com/yourusername/resume-workflow/discussions)
- Review [SETUP_INSTRUCTIONS.md](SETUP_INSTRUCTIONS.md)

**Want to share your success?**
- We'd love to hear your story!
- Tag us if you get hired using this system
- Share your customizations

---

## 🌟 Star This Repository

If this tool helps you land your next role, please:
- ⭐ Star this repository
- 🔄 Share with job seekers
- 💬 Leave feedback
- 🤝 Contribute improvements

---

**Built with ❤️ and Claude.ai**

*"The best resume is one that represents you accurately and lands interviews. This system helps you create exactly that."*
