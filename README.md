# Delta911

**Live demo:** https://claude.ai/artifact/2hJqrzwKqr1ZJniXYSiiLw

## All three hackathon prototypes

- [Lume Host Stand](https://claude.ai/artifact/6nJLPbVyaKm9xERGnJzfbZ) (Challenge 1: Resy goes offline, host stand floor plan) · [repo](https://github.com/mz462/resy-offline-host-stand)
- [Final Buzzer Map](https://claude.ai/artifact/PpAobzRDSrPcYSV9ptZ5Ev) (Challenge 2: MSG egress planner) · [repo](https://github.com/mz462/final-buzzer-map)
- [Delta911](https://claude.ai/artifact/2hJqrzwKqr1ZJniXYSiiLw) (Challenge 3: 911 call-surge triage) · [repo](https://github.com/mz462/delta911)


**Every surge call gets answered. Only new information reaches a dispatcher.**

AI triage console for 911 call centers (PSAPs) during call surges. Each call is transcribed, its facts are diffed against the incident's known facts, and:

- **Duplicates** are clustered and answered with a dispatcher-approved broadcast. The line is held and the caller keeps their place. The AI never hangs up.
- **New life-safety facts** (person trapped, wheelchair user inside, suspect direction) are flagged to a human and appended to the live incident brief.
- **Different incident types at the same corner** (fire vs stabbing) are never auto-merged; one tap splits them.
- **Two-layer scoring:** incident severity (people at risk + can it spread) and call priority (severity + new facts). Impact = people at risk, never neighborhood. No voice-stress scoring.
- **Regional compliance toggle:** where a human must answer every call, the AI only groups duplicates and a dispatcher answers the group with one tap.

## Run
Open `index.html` in a browser and press **Play**. The demo pauses for you to **Confirm & broadcast** the fire and **Split** the stabbing. All calls are scripted mock data.

Built for the Plug and Play × PMAI Hackathon, Challenge 3 (911 call surges).
