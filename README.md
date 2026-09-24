# Student Well-being — AI Nexus

**PS-011 · Human Development, Health & Social Impact**

An early-support system that helps identify students who may need help, and connects them with the right campus resources — before a quiet struggle becomes a crisis.

🔗 **Live site:** _add your Netlify URL here once deployed_

## The problem

Four pressures build up silently during a semester, and most institutions have no data-driven way to notice until a student is already in crisis:

- **Academic pressure** — heavy workloads, exams and grade anxiety
- **Financial stress** — tuition, hostel fees and daily expenses
- **Social isolation** — peer friction and lack of belonging
- **Hidden struggles** — no early, data-driven way to spot at-risk students

## The solution

A four-step early-intervention pipeline that turns everyday student data into timely, human support:

1. **Collect signals** — attendance, grade trends, LMS activity, optional mood check-ins
2. **Analyze & detect** — an ML model scores risk patterns across academic, financial and social indicators
3. **Alert & triage** — counsellors get a prioritized, privacy-respecting dashboard
4. **Connect support** — students are matched to counselling, financial aid or peer groups

Every risk score is an outreach signal, never an automated diagnosis — a counsellor makes the final call.

## What's in this website

A single-page, static pitch site (`index.html`) covering:

- Problem statement and proposed solution
- **A working interactive demo** — adjustable sliders simulate a student's attendance, submissions, mood and LMS activity, and the page computes a live risk score and recommended action in the browser (no backend needed)
- Tech stack, system architecture, trust & governance principles, and roadmap
- Team credits

## Tech stack

| Layer | Choice |
|---|---|
| Frontend | React (planned for the full product) |
| Backend | FastAPI |
| Data / ML | Python, scikit-learn-style risk scoring, pandas for analytics |
| Database | Secure, access-controlled student data store |
| This pitch site | Plain HTML, CSS and JavaScript — no build step, no dependencies |

## Running it locally

No install required — it's a single static file.

```bash
# open directly
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# or serve it locally
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

This is a static site, so any static host works. Fastest option — Netlify manual deploy:

1. Go to [app.netlify.com](https://app.netlify.com) → **Add new site → Deploy manually**
2. Drag the folder containing `index.html` onto the upload box
3. Netlify gives you a live `.netlify.app` URL in seconds

(Vercel, GitHub Pages, and Cloudflare Pages work the same way — just point them at this folder.)

## Team AI Nexus

| Name | Role | Reg. No. |
|---|---|---|
| Vidhi Gupta | Leader · Project Coordination | RA2681242030003 |
| Anant Jain | AI / ML & Backend | RA2681242030016 |
| Mahi Verma | Research & Documentation | RA2681242030043 |
| Tanshi | Frontend & UI | RA2681242030011 |

## Status

Built for NEXXATHON Round 1 — Idea Pitching. Round 2 will layer in the live product: real student sign-in, an actual counsellor dashboard, and a trained risk model behind the demo shown here.
