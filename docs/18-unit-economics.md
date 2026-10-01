# Unit economics: what a resolution is worth

The meetings never recorded a cost per chat or staff hours saved (see [Sources and evidence gaps](15-sources.md)). This page fills that gap with a model anyone can rerun with their own numbers. **Every input below is illustrative, not Varo data.** Only the resolution rates come from the project.

## The one formula that matters

```
Monthly value = chats moved off people x (cost of a person-handled chat - cost of an assistant-handled chat)
```

Everything else is detail. The two levers are how many chats the assistant truly resolves and how big the cost gap is between a person and the assistant.

## Worked example (illustrative inputs)

| Input | Illustrative value | Where the real number lives |
|---|---|---|
| Card chats per month | 100,000 | Contact reason tags in the data lake |
| Resolved without a person, before | 44% | Weekly team sync, data product, Jul 8, 2026 |
| Resolved without a person, after | 57% | Weekly team sync, data product, Jul 8, 2026 |
| Cost of a person-handled chat | $6.00 | Workforce cost / chats handled |
| Average handle time for a person | 8 minutes | Amazon Connect reporting |
| Productive hours per agent per month | 140 | Workforce planning |

| Result | Math | Illustrative answer |
|---|---|---|
| Chats moved off people each month | 100,000 x (57% - 44%) | 13,000 |
| Agent hours freed each month | 13,000 x 8 / 60 | About 1,730 hours |
| Agent capacity freed | 1,730 / 140 | About 12 agents |
| Gross monthly value, before vendor cost | 13,000 x $6.00 | $78,000 |

A 13 point gain on one contact reason is worth roughly a dozen agents of capacity at this scale. That capacity goes to the cases that need judgment, which is where it shows up in customer experience.

## How the pricing model changes the math

There are two common ways to pay for a support assistant.

| Pricing model | Who carries the risk early | What the buyer is really paying for |
|---|---|---|
| Flat platform fee | The buyer. The fee is the same whether the assistant resolves 43% or 57% | Capacity and the right to build |
| Price per resolved conversation | Shared. The vendor earns less while resolution is low | Outcomes, as long as everyone agrees what "resolved" means |

Sierra has been reported to price around $1.50 per resolved conversation ([ValueAdd VC, Sep 2026](https://valueaddvc.com/blog/sierra-ai-valuation-2026-15-8b-series-e-enterprise-ai-agents)). Unconfirmed by Varo.

Our own launch shows why this matters. Early on, with help articles only, the new assistant resolved 43% of chats against 55% on the old bot (Decagon company training, Apr 3, 2026). Under a flat fee, Varo paid full price for that dip. Under per-resolution pricing, the vendor would have shared it. In exchange, per-resolution pricing raises the stakes on the definition of a resolution, because every chat marked resolved is a charge. That definition is the subject of [What counts as resolved in banking](19-what-counts-as-resolved.md).

## Break-even check for per-resolution pricing

```
Per-resolution pricing pays off when: price per resolution < cost of a person-handled chat x share of resolutions that are truly correct
```

If 95% of chats marked resolved are truly correct, and a person-handled chat costs $6.00, any price below about $5.70 per resolution saves money. If only 80% are correct, the customers who come back cost twice, and the ceiling drops to about $4.80 before counting the cost of the repeat contact. Quality, not volume, sets the price a buyer can afford.

## The next value pool: disputes

Dispute intake is the next target, at about 40% lower cost to take in each dispute (Weekly team sync, data product, Jul 8, 2026). This is a goal, not a result. Disputes are worth more per conversation than card questions, because intake is slower, involves regulated timelines, and errors are expensive. They are also where the definition of "resolved" matters most.

## To make this page real

1. Replace the illustrative inputs with figures from workforce planning and Amazon Connect.
2. Measure the share of "resolved" chats that are truly correct, using the daily sample review.
3. Track repeat contacts within 7 days, which was proposed but not confirmed as built (Decagon company training, Apr 3, 2026).
