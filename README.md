# job-fit-check

A Claude skill that helps a job seeker decide whether an opportunity is worth applying to, and how to respond. It is built for private-sector, resume-based roles in any industry. Company research is strongest for startups, growth-stage and listed companies, where funding news or filings are public, and thinner for small private firms, where it says so. Share a job post, a recruiter message, or a company name, and it checks the company, checks the posting for red flags, compares the role against **your** resume and priorities, scores the fit, and drafts the outreach.

It is built to be direct. It reports what it could verify, what it could not, and where the evidence is thin. It does not promise outcomes.

## What it does

- **Reads the role**: title, level, years asked, location, must-haves, and what the post leaves out.
- **Checks legitimacy and freshness**: is the company real, is the poster traceable to it, does the post show scam or low-quality patterns, and does the role look still open or stale (a real company can leave a filled or inactive post up).
- **Researches the company**: funding, size, growth, leadership of the relevant function, team structure, and culture signals from reviews, with the number of reviews stated.
- **Compares against your resume**: each must-have marked Covered, Partly or Missing with the resume line behind it, stated knock-out risks (years, location, required tools), JD terms you have experience in but your resume does not use, and likely interview questions about your gaps.
- **Scores 1 to 5** across six categories, each with a confidence level, and gives one verdict: Apply, Apply with a tailored angle, Verify first, or Skip.
- **Drafts outreach**: subject line options, a DM or email, a short public comment, and questions to ask the recruiter.
- **Lists sources to verify yourself**: registries, careers pages, profiles and review sites, so you can cross-check key claims.

## Who it is for

Job seekers applying to private-sector, resume-based roles, in any industry and at any seniority, who can provide a job post (or company name), their resume and their priorities. It works in English. Company research is strongest for startups, growth-stage and listed companies, and thinner for small private firms, family businesses and agencies, where it says so and marks affected scores low confidence or Not scored. I have tested it mainly on funded and growth-stage companies.

## Limitations: roles it is not designed for

To stay fast and focused, the skill does not try to cover every hiring process. It is not designed for:
- Government, public-sector and civil service posts (fixed eligibility rules, exams, formal notifications)
- Licensed or regulated roles where a licence or registration is the main gate, such as nursing, law, aviation or teacher certification. It does not check licences or eligibility.
- Academic and research appointments
- Gig, freelance, contract and executive search

For these, it says so up front and runs only the steps that still apply, usually the legitimacy and company checks.

**Regional coverage:** source lists lean toward India, the UK, the US and a few other English-speaking markets (the registries listed also include Canada, Australia, Singapore and the EU). In other regions, expect thinner research and more low-confidence scores. The skill says so when this applies.

## What it does not do

- It does not know any company's screening tools, cutoffs, applicant volume or hiring bar. These are rarely public. The skill reads only what the job description states.
- It does not predict pass or fail, and it does not give a separate ATS score.
- It does not add keywords, years, titles or results you cannot back up. It only suggests rewording experience your resume already supports.
- It cannot tell for certain whether a role is still open. Many posts show no date, so freshness is often "unclear". It reports the evidence and suggests asking the recruiter.
- It does not guarantee its research. It depends on what web search finds. Verify important facts with the sources it lists.

## Platforms

Built and tested in Claude only. The skill uses the SKILL.md format, which other AI tools also read, but I have not tested it elsewhere. It needs web search for the company research, and file creation for the optional one-page report. If you try it on another tool, please say which one in your feedback.

## Requirements

- A Claude plan with skills available and **Code execution and file creation** turned on (Settings > Capabilities on Free, Pro and Max plans).
- Web search turned on, for company research.

## Install

1. Download `job-fit-check.skill` from the [Releases](../../releases) page of this repository. Do not use GitHub's "Download ZIP" button, as it adds an outer folder that can make the upload fail.
2. In Claude, open **Customize > Skills**, click **+**, then **Create skill**, then **Upload a skill**.
3. Upload the file. If it asks for a ZIP, rename `job-fit-check.skill` to `job-fit-check.zip` and upload that.
4. Make sure the skill is toggled on.

Custom skills you upload are private to your account.

Not comfortable with GitHub, or the download is not working? Message me and I will send a Google Drive link.

## Use

Start a new chat, attach your resume, and paste or upload a job post:

> Use job-fit-check on this role. [post, screenshot, or recruiter message]

On first use it asks for your **constraints** once: career direction, hard filters (location, remote, pay, seniority), an optional portfolio, profile or work-samples link to use in outreach, outreach preferences, and anything non-negotiable. Nothing about any one person is built into the skill.

You get a short chat answer. Ask for the one-page report if you want it saved.

## Output order

1. Verdict and one-line reason
2. Scores (1 to 5, with confidence)
3. Company and legitimacy
4. Fit with your resume
5. Red flags and unknowns
6. Questions to ask
7. Verify it yourself (sources and links)
8. Outreach draft

## Related skills

Other skills help with parts of the job search, mostly resume tailoring, ATS-style matching, cover letters and interview prep. This one is built for the step before: deciding whether to apply, and checking the company and poster first. They can be used together.

Examples found through public search. They are not affiliated with this project, and I have not reviewed or tested them, so check each before use:
- [Resume Tailoring Skill](https://github.com/varunr89/resume-tailoring-skill): tailors a resume to a job description, with company and role research.
- [Resumeskills](https://github.com/paramchoudhary/resumeskills): a set of resume skills, including a job description analyzer with match scores and gaps.
- [Job Seeker Claude Skills](https://blog.asadfaizee.is-a.dev/posts/claude-skills-for-job-seekers/): resume, cover letter, interview prep and tracking.
- [Claude Code Playbooks guide for job seekers](https://www.claudecodehq.com/blog/claude-skills-job-seekers): six skills covering the search from resume to interview.

## Files

- `SKILL.md`: the workflow
- `references/scoring-rubric.md`: how each category is scored
- `references/legitimacy-checklist.md`: legitimacy and scam checks
- `references/sources.md`: source priority and sources to verify with
- `references/worked-example.md`: sample output, design role
- `references/worked-example-analytics.md`: sample output, non-design role with an unnamed employer (illustrative)

## Privacy

Your resume and constraints are used only for the check. The skill does not repeat sensitive personal details in outreach unless you want them.

## Feedback

I would value your feedback: what worked, what was wrong, and what was missing. Two ways to share it:
- **Feedback form:** https://forms.gle/xUXaGwNz1mTVYXqr5
- **GitHub:** open an issue using the "Feedback" template.

Please leave out your resume and personal details. Describe what the skill said and what you expected. Feedback is used to improve the skill, and I log the changes I make in response. I will only quote you if you tick the consent box on the form.

Created by Bhawanakumari Rajeshkumar. Built and tested first on product design roles; the format applies to other private-sector roles within the limits above.

