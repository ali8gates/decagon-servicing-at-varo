# Build phase (January to February 2026)

## What had to be built

| Piece | Plain description | Source |
|---|---|---|
| Help content | About 60 Varo help articles, turned into about 100 pieces of content, synced from Zendesk, plus short custom answers | Varo: Decagon build review, Feb 26, 2026 |
| Workflows | Step by step instructions Decagon follows, written mostly in plain English with a few fixed rules (Decagon calls these AOPs) | How Decagon works walkthrough, Feb 11, 2026 |
| Connections to Varo systems | Secure links so the agent can read account details and later take actions like closing an account | Decagon Standup, Jan 16, 2026 |
| Security sign-in | Staff log in through Okta; system calls use signed security tokens | Decagon call, Jan 20, 2026 |
| Privacy masking | Personal details are hidden in chat logs using Google's data protection service | Decagon/Varo weekly, Feb 3, 2026 |
| Contact reason tags | Labels that sort each chat by topic so we can report on it | Decagon Lex standup, Feb 2, 2026 |
| Data pipeline | Moving every chat into Varo's data lake so Tableau dashboards can compare Lex and Decagon | Data pipeline planning, Jan 14, 2026 |

## How Decagon answers a question

From the February 11 review (How Decagon works walkthrough, Feb 11, 2026):

1. It rewrites the customer's message to make the intent clear.
2. If the message could mean more than one thing, it asks or narrows it down.
3. It picks the right workflow, if one applies.
4. It looks up the most relevant help articles.
5. A separate answer checker reviews the draft answer against Varo's rules and rewrites it if something is off.

Every step is visible in a trace view, so the team can see exactly why an answer was given.

## Biggest build blocker

Decagon changed the format of its exported data almost weekly, for example renaming a conversation ID field. Each change broke Varo's reports (Decagon Blockers, Jan 29, 2026). The fix was a written process for advance notice of changes (Decagon/Varo weekly, Feb 3, 2026) and, later, keeping a raw copy of the data before reshaping it (Weekly team sync, data product, Jul 8, 2026).
