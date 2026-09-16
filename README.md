# CV Optimizer Gem

> An AI-powered CV review system built for the Israeli job market. Scores CVs on a research-backed 100-point model, matches them to job descriptions, and gives brutally honest, actionable feedback — like a senior headhunter who tells you the truth.

---

## What This Is

This repository contains the complete instruction set and reference documents for a **Google Gemini Gem** that acts as a Senior Talent Acquisition Specialist and Headhunter.

The Gem:
- Analyzes CVs using a structured 100-point scoring model
- Matches CVs against job descriptions (two separate scores)
- Rewrites summaries, headlines, and bullet points — without inflating experience
- Audits LinkedIn profiles for recruiter search visibility
- Writes targeted cover letters
- Supports a Career Direction mode for candidates who are stuck or burned out

Designed for the **Israeli job market** — Hebrew-first, ATS-aware, dugri in tone.

---

## How It Works

The Gem operates in four modes:

| Mode | When to use |
|---|---|
| `SCORING` | Upload a CV — get a full score, breakdown, and ranked fixes |
| `JOB_MATCH` | Upload a CV + job description — get CV Quality score and Match to Role score |
| `REWRITE` | Request improved phrasing for your summary, headline, or bullet points |
| `CAREER_DIRECTION` | When you're stuck, sending applications with no responses, or need real direction |

---

## The Scoring Model

CVs are scored on **100 points** across 7 research-backed categories:

| Category | Points |
|---|---:|
| Job-specific relevance | 25 |
| Achievement evidence | 20 |
| Ownership and career logic | 15 |
| ATS integrity | 15 |
| Human scan and hierarchy | 10 |
| Israeli localization | 10 |
| Trust and hygiene | 5 |

Score bands:

| Score | Meaning |
|---|---|
| 90-100 | Exceptional — submit now |
| 85-89 | Interview-ready |
| 75-84 | Competitive but needs work |
| 65-74 | Generic or under-evidenced |
| 50-64 | Significant problems — reconstruct |
| 0-49 | Non-converting — fix fundamentals first |

---

## Repository Structure

```
cv-optimizer/
│
├── README.md                          # You are here
│
├── cv-review.md                       # Master document — full unified system
│
├── gem/                               # Gem-ready files
│   ├── gem-instructions.md            # → Paste into Gem instruction window
│   ├── scoring-skill.md               # → Upload as reference document
│   ├── cv-review-guidelines.md        # → Upload as reference document
│   ├── output-template.md             # → Upload as reference document
│   └── career-direction.md            # → Upload as reference document
│
├── 0-100 scoring model.md             # Source: full research-backed scoring framework
└── High-Conversion CV Architecture    # Source: Israeli market & gender-neutral CV research
    for Female Individual Contributors
    in Israel.md
```

---

## Setting Up the Gem

1. Go to [gemini.google.com](https://gemini.google.com) and open **Gems**
2. Create a new Gem
3. Copy the contents of `gem/gem-instructions.md` into the **Instructions** field
4. Upload the following files as **Reference Documents**:
   - `gem/scoring-skill.md`
   - `gem/cv-review-guidelines.md`
   - `gem/output-template.md`
   - `gem/career-direction.md`
5. Save and start the Gem

---

## Using the Gem

**To score a CV:**
> Upload or paste your CV. The Gem will analyze it and return a full score, breakdown by category, key weaknesses, and ranked fixes.

**To match a CV to a job:**
> Share your CV and paste the job description. You'll get two scores: CV Quality and Match to Role, plus a keyword gap table.

**To rewrite:**
> Ask the Gem to rewrite your summary, headline, or specific bullet points. It will follow the No-Inflation Rule — it will never elevate your seniority or invent experience.

**To get career direction:**
> Tell the Gem you're struggling. It will switch modes and ask you the right questions before giving you a clear, honest direction.

---

## Design Principles

- **No flattery.** If your CV is weak, the Gem says so.
- **No inflation.** Rewrites never upgrade your seniority or invent results.
- **No ATS-hostile design.** No tables, graphics, icons, or Canva-style layouts will ever be recommended.
- **No bias.** The scoring model does not penalize for gender, name, military non-service, gaps, immigrant status, or unconventional career paths.
- **Honest triage.** When a CV is bad, you get the top 3 things to fix — not a 20-point list.

---

## Language

- Default responses: **Hebrew**
- Switch to English on request
- If your CV is in English: analysis in Hebrew, rewrite examples in English

---

## Built On

- [0-100 Scoring Model](./0-100%20scoring%20model.md) — research-backed framework referencing ATS vendor documentation, Israeli employment law, selection research, and cognitive scanning studies
- [High-Conversion CV Architecture](./High-Conversion%20CV%20Architecture%20for%20Female%20Individual%20Contributors%20in%20Israel.md) — Israeli market nuances, ATS behavior, gender-neutral design, IC-specific language patterns

---

## Contributing

Pull requests are welcome. If you identify scoring logic gaps, outdated ATS behavior, or Israeli market changes, open an issue or submit a fix directly.

---

## License

MIT — use it, adapt it, build on it.

---

*Built for job seekers who want honest feedback, not a pep talk.*
