# Contributing to Resume Workflow

Thank you for considering contributing to Resume Workflow! This document provides guidelines for contributing to the project.

## How to Contribute

### Reporting Bugs

If you find a bug, please open an issue with:
- **Clear title** describing the problem
- **Steps to reproduce** the issue
- **Expected behavior** vs actual behavior
- **Agent involved** (which agent failed or behaved unexpectedly)
- **Example input** (if possible, sanitized of personal info)

### Suggesting Features

Feature requests are welcome! Please open an issue with:
- **Clear description** of the feature
- **Use case** - why would this be valuable?
- **Proposed implementation** (if you have ideas)
- **Examples** of how it would work

### Submitting Pull Requests

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Follow the existing code style
   - Update documentation if needed
   - Test your changes

4. **Commit with clear messages**
   ```bash
   git commit -m "Add feature: description of what you did"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Open a Pull Request**
   - Describe what you changed and why
   - Reference any related issues
   - Include before/after examples if applicable

## Development Guidelines

### Agent Development

When modifying or creating agents:

**Structure:**
- Use clear section headers
- Include examples
- Document all parameters
- Explain the "why" not just the "what"

**Testing:**
- Test with multiple resume types (IC, Manager, Director, VP, C-suite)
- Test with different industries
- Verify accuracy validation still works
- Check for unintended side effects

**Documentation:**
- Update agent-specific docs in the .md file
- Update SETUP_INSTRUCTIONS.md if workflow changes
- Add examples to README.md if helpful

### Template Development

When improving templates:

**Clarity:**
- Use clear placeholder text
- Provide examples inline
- Explain why each section matters

**Accessibility:**
- Keep instructions simple
- Accommodate different experience levels
- Avoid jargon where possible

### Framework Development

When modifying the Three-Lens Framework or creating new frameworks:

**Consistency:**
- Ensure compatibility with existing agents
- Don't break validation logic
- Test extensively before PR

**Documentation:**
- Explain the reasoning behind the framework
- Provide examples of application
- Show before/after comparisons

## Code Style

### Markdown Files

**Headers:**
- Use `#` for main titles
- Use `##` for major sections
- Use `###` for subsections
- Use `####` sparingly

**Lists:**
- Use `-` for unordered lists
- Use `1.` for ordered lists (auto-numbering)
- Indent nested lists with 2 spaces

**Code Blocks:**
```markdown
Use fenced code blocks with language hints:
```python
def example():
    return "like this"
\```
```

**Emphasis:**
- Use `**bold**` for important terms
- Use `*italic*` for emphasis
- Use `code` for file names, commands, variables

### Agent File Structure

```markdown
# AGENT X: [Name]

## PURPOSE
[One paragraph explaining what this agent does]

## TIMING
[When this agent runs in the workflow]

## PROCESS
[Step-by-step what the agent does]

## OUTPUT FORMAT
[What the agent produces]

## VALIDATION CRITERIA
[How to know if the agent succeeded]

## EXAMPLES
[Show input and output examples]
```

## Testing

### Before Submitting PR

Test your changes with:

1. **Multiple resume types**
   - Entry-level (2-5 years experience)
   - Mid-career (5-10 years)
   - Senior (10-15 years)
   - Executive (15+ years)

2. **Different scenarios**
   - Career transitions
   - Stretch roles (applying above current level)
   - Industry changes
   - Gap explanations

3. **Edge cases**
   - Very short career history
   - Very long career history (20+ years)
   - Non-traditional backgrounds
   - Military transitions

4. **Validation**
   - Agent 4 still catches inaccuracies
   - Agent 5 still catches AI language
   - Agent 6 scoring still works
   - Agent 7 ATS compliance passes

### Test Checklist

- [ ] Tested with 3+ different resumes
- [ ] All agents execute in correct order
- [ ] Validation agents catch intended issues
- [ ] Output format is correct
- [ ] Documentation updated
- [ ] No personal information in commits
- [ ] Examples are sanitized

## Areas We'd Love Help With

### High Priority

1. **Industry-Specific Customizations**
   - Healthcare
   - Financial services
   - Technology/SaaS
   - Manufacturing
   - Government/Military

2. **Additional Validation Agents**
   - Keyword density checker
   - Readability scorer
   - Equity language validator
   - Skills gap identifier

3. **Career Level Templates**
   - Entry-level positioning
   - Mid-career positioning
   - Executive positioning
   - Career transition templates

### Medium Priority

4. **LinkedIn Integration**
   - Profile optimization agent
   - Headline generator
   - About section creator
   - Skills validator

5. **Interview Prep**
   - Question generator based on resume
   - STAR method formatter
   - Weakness reframing
   - Salary negotiation prep

6. **Network Outreach**
   - Connection request templates
   - InMail templates
   - Coffee chat request templates
   - Referral request templates

### Future Enhancements

7. **Portfolio Generation**
   - Project showcase pages
   - Case study formatter
   - GitHub profile optimizer

8. **Application Tracking**
   - Status tracker
   - Follow-up reminders
   - Interview scheduler
   - Offer comparison tool

## Community

### Code of Conduct

Be respectful, inclusive, and constructive:

**Do:**
- Help others learn
- Give constructive feedback
- Celebrate contributions
- Ask questions
- Share your success stories

**Don't:**
- Be dismissive or rude
- Share personal information without consent
- Submit AI-generated contributions without review
- Spam or promote unrelated products

### Getting Help

**Questions about contributing?**
- Open a Discussion on GitHub
- Tag your issue with `question`
- Reach out to maintainers

**Stuck on something?**
- Check existing Issues and Discussions
- Review SETUP_INSTRUCTIONS.md
- Ask in Discussions - we're here to help!

## Recognition

Contributors will be:
- Listed in CONTRIBUTORS.md
- Mentioned in release notes
- Credited in documentation (where applicable)

Significant contributions may result in:
- Co-maintainer status
- Invitation to steering committee
- Feature in blog posts/articles

## License

By contributing, you agree that your contributions will be licensed under the MIT License (same as the project).

---

## Questions?

Open an issue or discussion - we're happy to help you contribute!

**Thank you for making Resume Workflow better!** 🎉
