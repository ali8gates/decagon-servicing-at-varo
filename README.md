# Decagon at Varo: Rebuilding Servicing Chat, From Pilot to Full Production

I led Varo's move from its old scripted support chatbot (Amazon Lex) to Decagon, a support assistant that understands everyday language, alongside the customer experience team. This repository covers the work from the first vendor demo in October 2025, through the build and the gradual rollout, to full production in the in-app chat by July 2026, with a focus on what it changed for servicing: card questions, account requests, handoffs to people, and dispute intake.

It is written for readers across support operations, product, engineering, data, compliance, finance, and leadership. Each fact points back to the working session it came from.

## The story in five sentences

1. Varo's old chatbot could only follow fixed scripts, so many servicing requests ended up waiting for a person (varo <> Decagon, Oct 20, 2025).
2. After comparing vendors, we chose Decagon in November 2025 because Varo would keep control of its data and workflows, at a cost that fit an approved budget (Customer service partner next steps, Nov 12, 2025).
3. We built the connections, content, and safety rules between January and March 2026, then started with a small share of customers and grew it step by step (App Launch and Feedback Review, Mar 10, 2026).
4. Decagon reached 100% of chat traffic by July 2026, and the share of card questions resolved without a person rose from 44% in April to 57% in July (Weekly team sync, data product, Jul 8, 2026).
5. Net promoter score rose from about 40 to 50 before the change to over 80 afterward, based on my own reporting. The survey report is held internally.

## Start here

- [How I led this](docs/17-how-i-led-this.md): the hats I wore, how I worked with the customer experience team, and the outcomes.
- [What this changed for servicing](docs/16-servicing-impact.md): card questions, account requests, handoffs, and dispute intake, before and after.
- [What counts as resolved in banking](docs/19-what-counts-as-resolved.md): why a happy customer is not always a resolved case, and five levels of resolved.
- [Unit economics](docs/18-unit-economics.md): what a resolution is worth, and how per-resolution pricing shifts early risk.

## Wiki pages

1. [Executive summary](docs/01-executive-summary.md)
2. [Why we did this](docs/02-why-we-did-this.md)
3. [Timeline, from first demo to full production](docs/03-timeline.md)
4. [Proof of concept and vendor choice](docs/04-proof-of-concept.md)
5. [Build phase](docs/05-build-phase.md)
6. [Launch and gradual rollout](docs/06-launch-and-rollout.md)
7. [The live production environment](docs/07-production-environment.md)
8. [Results, including the promoter score](docs/08-results-and-promoter-score.md)
9. [Quality checks and monitoring](docs/09-quality-and-monitoring.md)
10. [Risks, issues, and lessons learned](docs/10-risks-and-lessons.md)
11. [What comes next](docs/11-roadmap.md)
12. [People and roles](docs/12-people-and-roles.md)
13. [Plain language glossary](docs/13-glossary.md)
14. [Detailed analysis](docs/14-analysis.md)
15. [Sources and evidence gaps](docs/15-sources.md)
16. [What this changed for servicing](docs/16-servicing-impact.md)
17. [How I led this](docs/17-how-i-led-this.md)
18. [Unit economics: what a resolution is worth](docs/18-unit-economics.md)
19. [What counts as resolved in banking](docs/19-what-counts-as-resolved.md)
20. [What would have changed the vendor decision](docs/20-what-would-have-changed-the-decision.md)
21. [Architecture at a glance](docs/21-architecture.md)

## How to use this repository

* Read the executive summary first. It is one page.
* Use the analysis page when you need the "so what" for leadership.
* Use the sources page before quoting a number. It shows how strong the evidence is for each one.
* The `data` folder holds the key numbers in a spreadsheet-friendly format.

## Status

Last updated October 1, 2026. Owner: Ali Gates, Director of AI and Machine Learning, Varo.
