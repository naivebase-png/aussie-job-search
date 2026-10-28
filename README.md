# Aussie Job Search – a Claude skill

An Australian job search assistant for Claude. It finds roles on Australian job boards, checks them against your profile, writes Australian-style resumes, cover letters and government selection criteria responses, and keeps a tracker of your applications.

## What it does

| Command | What it does |
|---|---|
| `setup` | Builds your profile from your resume (roles, location, salary, work rights, clearances) |
| `search [query]` | Finds current roles on Seek, LinkedIn, APSJobs, state government boards and more |
| `match [ad]` | Rates your fit for a job ad and lists gaps |
| `resume [ad]` | Tailors your resume to Australian conventions |
| `cover-letter [ad]` | Writes a one-page cover letter for the role |
| `criteria [ad]` | Drafts selection criteria responses for public sector roles (STAR format) |
| `tracker` | Keeps a spreadsheet of applications, closing dates and follow-ups |
| `automate` | Sets up a recurring search with a daily digest |
| `insights` | Reviews your results and suggests changes |

Plain-English requests work too, e.g. "find hybrid data analyst roles in Melbourne over $110k".

## Install

**Claude apps (claude.ai / desktop):** download this repository as a ZIP, keep only the `aussie-job-search` folder, zip that folder and upload it in Claude's skills settings.

**Claude Code:** copy the `aussie-job-search` folder into `~/.claude/skills/` (for you) or `.claude/skills/` in a project (for everyone on the project).

Then ask Claude something like "find Head of Data roles in Melbourne" or run `/aussie-job-search help`.

## Ground rules built into the skill

- Never invents job listings, salaries or any of your experience; missing facts are left as marked placeholders.
- Only shows listings it actually retrieved, with links.
- Doesn't log in to job boards or get around sign-in walls or CAPTCHAs.
- Never submits an application or contacts an employer without your explicit approval.
- Visa, pay and legal questions get general information plus a link to the official source (Home Affairs, Fair Work Ombudsman). Not legal or migration advice.

## Sites it searches

Seek, LinkedIn Jobs, Indeed Australia, Jora, CareerOne, Adzuna; APSJobs and the NSW, VIC, QLD, WA, SA, TAS, ACT and NT government job boards; GradConnection, Prosple, EthicalJobs, Pro Bono Australia; health, mining and company careers pages; and recruitment agencies such as Hays, Robert Walters, Michael Page, Randstad and Hudson.
