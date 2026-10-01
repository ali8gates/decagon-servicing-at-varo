# What counts as resolved in banking

In most industries, a chat that ends without a person and without a complaint counts as resolved. In banking that is not enough. A customer can leave a chat happy while the bank has missed a regulatory obligation. This page proposes a standard for what "resolved" should mean in regulated servicing.

This is a proposed standard, written after the project. It was not the definition used in the meetings. The meetings do not record the exact definition behind the 44% to 57% card resolution figure, so confirm it before comparing the two.

## The problem in one example

A customer writes: "There's a charge on my card I don't recognize. Can you just tell me what it is?"

The assistant looks up the merchant, explains it, and the customer says thanks. The chat ends without a person. By the usual measure, it is resolved.

But the customer described a transaction they did not recognize. Under Regulation E, a consumer's report of a possible unauthorized electronic transfer can count as a notice of error, whether or not they use the word "dispute," and oral or written notice can start the bank's investigation clock. If the customer still believes the charge is wrong, and no dispute intake was started, the chat closed cleanly and the bank may have missed an obligation. The rating is high. The outcome is wrong.

## Five levels of resolved

Each level includes the ones above it.

| Level | Name | The test | How to measure it |
|---|---|---|---|
| 1 | Contained | The chat ended without a person | Handoff flag in the chat record |
| 2 | Answered | The customer confirmed the answer or rated it well | Post-chat survey |
| 3 | Correct | The answer matched Varo policy, and any account action matched the system of record | Daily sample review by people who know servicing policy |
| 4 | Durable | The customer did not come back about the same issue within 7 days | Repeat contact check across chat, phone, and email |
| 5 | Compliant | No regulatory duty was missed: disputes started when they should have been, complaints logged, required disclosures given | Automated watchers for dispute and complaint language, plus compliance sampling |

**Only level 5 is a true resolution in banking.** Level 1 is what most dashboards show. The gap between the two is the risk nobody is measuring.

## What triggers a level 5 check

These are the moments where a clean chat can still be a miss:

* **Unrecognized or unauthorized transactions.** Treat any description of one as possible dispute intake, even if the customer only asks a question.
* **Expressions of dissatisfaction.** A frustrated customer may be filing a complaint without saying so. Complaints have handling and reporting duties.
* **Fraud, anti-money-laundering, and discrimination topics.** These already go to a person (How Decagon works walkthrough, Feb 11, 2026). The check is that they reliably do.
* **Account closures and fee questions.** Required disclosures and fair treatment rules apply.

Varo already runs automated watchers for anti-money-laundering topics and disputes across every chat (Data review, Nov 17, 2025). The proposal is to count their findings against the resolution rate, not just report them separately.

## Why this matters for pricing

If a bank pays a vendor per resolved conversation, the contract should name the level. Paying at level 1 rewards the assistant for ending chats. Paying at level 4 or 5 rewards it for ending problems. The [unit economics page](18-unit-economics.md) shows how much the share of truly correct resolutions moves the price a buyer can afford.

## Proposed reporting

1. Report all five levels side by side, so the gap between level 1 and level 5 is visible.
2. Sample enough chats each week to estimate level 3 and level 5 with confidence. The current daily review of roughly 10 to 50 chats (Decagon company training, Apr 3, 2026) is a start.
3. Build the 7 day repeat contact check, which was proposed but not confirmed as built (Decagon company training, Apr 3, 2026).
4. Any level 5 miss gets a root cause review, the same way a production incident would.
