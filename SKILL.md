---
name: job-fit-check
description: Evaluate a job opportunity for a specific job seeker. Researches the company (legitimacy, funding, growth, team structure, leadership, culture signals), checks the posting or recruiter for red flags, compares it against the seeker's resume and personal constraints, gives 1-5 fit scores with a verdict, and drafts the outreach (subject, DM, comment, questions to ask). Use whenever the user shares a job post, LinkedIn hiring post, JD, recruiter message, screenshot of a job listing, or a company name and asks whether to apply, whether it is legit, whether they are a fit, what the company or culture is like, or how to respond or reach out, even if they never say "fit check".
---

# Job Fit Check

Help a job seeker decide whether an opportunity is worth their time and, if it is, respond well. The value is an honest, sourced read of the company and the role set against *this person's* resume and priorities. A flattering answer that sends someone into a bad fit is worse than no answer, so be candid, and say plainly when something could not be verified.

## Scope: who this skill serves

Built for people applying to **private-sector, resume-based roles in any industry**, at any seniority, who can provide a job post (or company name), their resume, and their constraints. Written in English. It is deliberately not built to cover every hiring process, so keep it fast and focused.

It is **not designed for** the following. If the opportunity is one of these, say so in one line at the start, and either decline the parts that do not fit or run only the steps that still apply (legitimacy and company research usually still do):
- Government, public-sector and civil service posts (fixed eligibility rules, exams, formal notifications)
- Licensed or regulated roles where a licence or registration is the main gate (for example nursing, law, aviation, teacher certification). The skill does not check licences or eligibility.
- Academic and research appointments (publications and a different process)
- Gig, freelance, contract and executive search
- Regions where public company records are limited: research will be thinner and more scores will be low confidence. Say so.

Company research depth varies by company type. It is strongest for startups, growth-stage and listed companies, where funding news or filings are public. It is thinner for small private firms, family businesses and agencies, where little is public: say so, mark affected scores low confidence or Not scored, and do not guess. It has been tested mainly on funded and growth-stage companies, so do not claim equal strength elsewhere.

## 1. Gather inputs

You need three things. Check the conversation, uploaded files, and any project files before asking.

1. **The opportunity**: post text, screenshot, URL, recruiter message, or just a company name. Read screenshots directly. If a URL is given, fetch it.
2. **The seeker's resume**: use the one they provide or that is in the project. Treat it as the source of truth for what they have done. If there is none, ask for it once.
3. **The seeker's constraints**: personal priorities that shape the verdict and the outreach. Do not assume these. If you do not already know them, ask once, in a single short message, and offer sensible examples:
   - Career direction and focus areas (for example, "stay in data analytics, move toward a team lead role")
   - Hard filters: location, remote or hybrid, minimum pay, seniority range, industries to avoid
   - Portfolio, profile or work samples link to use in outreach, if relevant to the role (optional)
   - Outreach preferences (for example, "offer a walkthrough call", tone, length)
   - Anything else they treat as non-negotiable

   If the environment has persistent memory, reuse constraints from earlier chats and save new ones. Otherwise carry them through the conversation. Constraints belong to the seeker; never carry one person's constraints into another person's check.

## 2. Extract the role

Pull out: title, level, years of experience asked, location and work mode, must-haves vs nice-to-haves, pay if stated, who posted it (hiring manager, recruiter, agency, company page), how to apply, and what is missing. Missing details are signals in themselves.

## 3. Check legitimacy and transparency

Read `references/legitimacy-checklist.md` and apply it. In short: is the company real, is the poster traceable to it, does the post give enough detail to be a real opening, and are there scam or low-quality patterns (fees, vague "work from home" with no employer, personal email domains, pressure tactics)? Also give a freshness read (Current / Unclear / Likely stale) as described in the checklist, since a real company can still leave a filled or inactive role posted. Distinguish "could not verify" from "looks fake", and "unclear" from "stale". Absence of evidence on a small team or new function is common and is not a red flag by itself.

## 4. Research the company

Use web search. Run separate searches rather than one combined query, and follow the source priority in `references/sources.md` (official and primary sources first, then established press, then databases, then review sites). Cover:

- What the company does, size, stage, funding, growth direction, recent news. For startups and growth-stage companies, funding rounds and growth news are the main signal. For established or listed companies, use filings, earnings, layoff or hiring-freeze news and leadership changes instead. Do not treat missing funding data as a concern for an established company.
- Leadership of the relevant function (for example engineering, marketing, finance, operations) and recent appointments
- The poster or recruiter: role, tenure, whether they appear tied to the company
- Team structure: is this function core to the business or a support function, a new team or an established one, how big, who it reports to
- Culture signals: employee reviews, interview experiences, leadership statements. Review sites are often thin or skewed, so report only what you actually found, note sample size, and mark confidence as low when data is sparse.

Never invent details to fill a gap. State what you could not find. Paraphrase sources, keep any quote very short, and cite web-sourced claims.

## 5. Compare against the seeker

Read the JD the way a screener would, using only what the posting states. Companies rarely publish their screening tools, cutoffs, applicant volume or hiring bar, so never claim to know them.

- **Must-have coverage**: for each required item in the JD, mark **Covered**, **Partly** or **Missing**, and cite the resume line that supports it. Separate "required" from "preferred" when the JD does.
- **Knock-out risks the JD states openly**: years of experience, seniority, location or work mode, required tools or domains. Say whether each is firm or soft (a "2-4 years" range is usually soft; a regulated-domain requirement may not be).
- **Wording gaps**: JD terms the seeker has real experience in but the resume does not say. Suggest rewording only for experience the resume already supports. Never suggest adding keywords, years, titles or results the seeker cannot back up.
- **Likely interview probes**: the two or three questions a hiring manager would reasonably ask about the biggest gaps, with the honest evidence the seeker can bring.
- **Constraint check**: does the role respect the seeker's hard filters and career direction?

State a weak screening read plainly, once. It means a risk, not that the seeker is unfit. Where the risk is high, say so and suggest a direct route (a DM to the poster, a referral) as an option.

## 6. Score and verdict

Read `references/scoring-rubric.md`. Score each category 1 to 5 and give a confidence level (high, medium, low) because some scores rest on thin evidence:

- Role match
- Legitimacy and transparency
- Company stability and growth
- Team and function maturity
- Culture signals
- Alignment with the seeker's constraints

Screening risk feeds the **Role match** score. Do not add a separate screening or ATS score and do not predict pass or fail. Do not just average. State the overall verdict in one line using one of: **Apply**, **Apply with a tailored angle**, **Verify first**, **Skip**, and the one or two reasons that drove it. A single severe issue (probable scam, a broken hard filter) can override good scores elsewhere.

## 7. Output: chat first, report on request

Default to a short chat answer. Keep it scannable, lead with the verdict, and avoid walls of text. Use this order:

1. Verdict and the one-line reason
2. Scores (a compact table with 1-5 and confidence)
3. Company and legitimacy: the few facts that matter, with sources, plus a one-line freshness read (Current / Unclear / Likely stale)
4. Fit with your resume: must-have coverage, stated knock-out risks, wording gaps, likely interview probes
5. Red flags and unknowns, including what cannot be known about the company's screening
6. Questions to ask the recruiter or hiring manager. Include "what are the must-haves, the interview stages, and is automated screening used?" only when the JD does not answer them. When freshness is unclear or likely stale, include "is this role still open, when was it opened, and where is the process now?"
7. "Verify it yourself": 3 to 5 sources from `references/sources.md` most relevant to this opportunity, with links, so the seeker can cross-check key claims (company registry, careers page, poster's profile, a review site)
8. Outreach draft (see below)

State each fact once. Do not repeat the score table in prose, restate the verdict, or add encouragement. See `references/worked-example.md` and `references/worked-example-analytics.md` for the target format and tone, including how to handle an unnamed employer.

End by offering a one-page fit report. Produce the report only when the seeker asks, using whatever document tool or skill is available (a Word or PDF file, or a doc), in the same order, kept to one page.

## 8. Outreach drafts

Offer when the verdict is Apply, Apply with a tailored angle, or Verify first. Draft, in order of usefulness:

- **Subject line** (three options, pick one as the recommendation). Name the role and the strongest match.
- **DM or email**: short, specific to the role, two or three concrete matches from the resume, the seeker's portfolio or profile link if they have one, and any offer the seeker asked for (such as a call to walk through their work). Ask one or two practical questions if the post left gaps (location, work mode, team).
- **Public comment** (if the post invites comments): two lines, then move to DM.

Use the seeker's own link and preferences from their constraints. Keep the tone confident and honest; do not hide a gap in years, but do not lead with it. Match the length to the channel.

## 9. Logging

If persistent memory or notes are available, record the lead briefly: role, company, source, date, contact, verdict, and next step. Record what the seeker told you or decided, not your research.

## Conduct

- The resume and constraints are the seeker's private data. Use them only for this check and do not repeat sensitive personal details in outreach unless the seeker wants them.
- Keep to the facts you found. When a conclusion rests on thin evidence, say so.
- Be direct. No promises, no predictions of outcomes (never "you will pass" or "good chance"), no false hope, and no encouraging filler. If the fit is poor, the verdict says so plainly.
- Respect the seeker's decision. If they choose to apply despite a weak score, help them do it well and note what to watch for.
