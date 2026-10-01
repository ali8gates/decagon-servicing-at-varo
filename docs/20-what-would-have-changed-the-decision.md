# What would have changed the vendor decision

Buyers rarely write down why a vendor lost. This page does, because the reasons are useful to any team buying a support assistant and to any vendor selling one into a bank.

The first section comes from the decision meeting. The rest is my view, written after the project. It is marked as such and was not discussed in a meeting.

## What decided it

From the November 12, 2025 decision meeting (Customer service partner next steps, Nov 12, 2025):

* Three options were on the table: keep Amazon Lex, Sierra offered through Accenture, or Decagon.
* Sierra had a strong product. The concern was the route, not the software: a partner would sit between Varo and a key customer touchpoint and Varo's brand voice.
* Decagon won on control (Varo writes and owns its workflows, content, and rules), flexibility (pieces can change one at a time), fit with the approved budget, an existing relationship through a shared investor, and readiness for the January to March busy season.

## What would have changed it (my view)

A bank's support chat is not a side channel. For many customers it is the bank. Anything that puts distance between the bank and that conversation is a risk the buyer has to price in. These are the conditions that would have made the decision closer, for any vendor:

| What the buyer needed | Why it mattered | What would have proven it |
|---|---|---|
| A direct line to the vendor's product team | Every change to a regulated workflow needs a fast loop between compliance, product, and the people building it. A partner in the middle adds a step to every loop | Named vendor engineers in the weekly working session, not only at the steering meeting |
| The bank writes and owns its workflows and brand voice | The bank answers to regulators for every word the assistant says | The bank's own team editing a live workflow during the proof of concept |
| Proof on the bank's own top questions | Demos on generic use cases do not show how the assistant handles your customers | A side by side test against the current bot on the top contact reasons, within weeks |
| Data the bank owns, in a stable format | Our biggest build blocker was the vendor's export format changing almost weekly (Decagon Blockers, Jan 29, 2026) | A written data contract and change notice process before signing |
| Pricing tied to a definition of resolved the bank trusts | Per-resolution pricing is only fair if both sides agree what resolved means | A shared resolution standard, like the one in [What counts as resolved in banking](19-what-counts-as-resolved.md) |
| A credible date before peak season | Missing January to March meant waiting a full year | A rollout plan with named owners and dates |

## Lessons for buyers

1. **Decide who owns the conversation before you compare features.** Most of our decision came down to control, not capability.
2. **Write the data contract first.** Format changes broke reports more than any problem with the answers did.
3. **Expect the first numbers to look worse, and say so up front.** Launching with help articles only meant 43% resolution against 55% on the old bot (Decagon company training, Apr 3, 2026).

## Lessons for vendors selling into banks

1. **The route to market is part of the product.** A strong product sold through a partner can lose to a weaker one sold directly, if the buyer sees the partner as a layer between them and their customer.
2. **Let the buyer hold the pen.** Banks will pay for software their own team can change, because they are the ones answering to regulators.
3. **Bring a definition of resolved, not just a resolution rate.** The vendor that defines resolution in a way compliance can sign off on wins the second half of the conversation.
