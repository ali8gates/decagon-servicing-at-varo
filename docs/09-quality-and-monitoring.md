# Quality checks and monitoring

## Before a change goes live

* **Standard test questions.** A lean set of about 30 help article questions plus key scenarios, run before each release so a fix in one place does not break another (Varo: Decagon build review, Feb 26, 2026).
* **Why only about 30.** Because both the answer and the grader are automated, some tests fail randomly. A set of 300 would create noise and slow the team down (Varo: Decagon build review, Feb 26, 2026).

## After it is live

| Check | What it does | Source |
|---|---|---|
| Daily sample review | People who know Varo read a random set of chats, roughly 10 to 50 a day, looking for wrong or odd answers | Decagon company training, Apr 3, 2026 |
| Automated watchers (Watchtowers) | Always-on monitors that scan every chat for set risks, such as anti-money-laundering topics, disputes, and agent quality | Data review, Nov 17, 2025 |
| Narrowing down bad chats | Start with low ratings or handoffs, then filter by workflow, topic, and error to find the cause | Decagon company training, Apr 3, 2026 |
| Dashboards | Resolution, satisfaction, and topic trends in Decagon and in Tableau | App Launch and Feedback Review, Mar 10, 2026 |
| Re-sorting old chats | Watchtowers can re-label past chats, which helps fill in history | Weekly team sync, data product, Jul 8, 2026 |

## Known gaps

* A check for customers who come back about the same issue within a few days was proposed as a way to catch wrong answers, but was not confirmed as built (Decagon company training, Apr 3, 2026).
* The agent sometimes offered a human handoff too often after an earlier handoff. The team chose to tune this after launch (Decagon company training, Apr 3, 2026).
