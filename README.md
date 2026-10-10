# Aangan Studio — Enquiry Dashboard & Phone Voice Bot

Founder's Office case 03 (MESA AI, Cohort C4): every incoming call to Aangan Studio answered at once, checked against the studio's five rules, booked, and handed to a designer with everything already asked.

## What's here

| Path | What it is |
| --- | --- |
| `index.html` | The dashboard as a static page (deployed on Vercel). Channel filter, weekly targets, 1-hour reply check, the five checks, nine checks, services and the stack. |
| `data/enquiries.csv` | The 40 anonymised September 2026 enquiries, coded by outcome, reply time and the five checks. |
| `db/schema.sql`, `db/seed.sql` | The Neon `enquiries` table and the September rows. |
| `voicebot/system-prompt.md` | The prompt for the Vaani Labs phone agent. |

## Notes

- This public copy shows a fixed snapshot of the data. The studio's own dashboard reads the Neon table live.
- The internal pricing guide is deliberately **not** in this repo: its figures must never reach a client.
- Never commit a database connection string. Store it as an environment variable in Vercel.

## Stack

Vaani Labs (calls) · Gemini Flash (call sorting) · Cal.com / Calendly / Google Calendar (booking) · Neon (call log) · HubSpot (deals) · Telegram (designer handoff) · Vercel (hosting) · GitHub (code).
