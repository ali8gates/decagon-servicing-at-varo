# The live production environment

## What is running today

| Area | Current state | Source |
|---|---|---|
| Channel | In-app chat for signed-in customers, 100% of traffic | Weekly team sync, data product, Jul 8, 2026 |
| Not yet covered | Phone support and customers who are not signed in | Decagon company training, Apr 3, 2026 |
| Content | Zendesk help articles synced automatically, plus custom answers | How Decagon works walkthrough, Feb 11, 2026 |
| Handoff to people | Chat summary and full history passed to the human agent; the agent side still runs through Amazon Connect | Data pipeline planning, Jan 14, 2026 |
| Privacy | Personal data masked in logs | Decagon/Varo weekly, Feb 3, 2026 |
| Data | Decagon chats flow into the same transcript table as before, so existing reports keep working | Weekly product review (Q3 planning), 2026 |
| Dashboards | Tableau views of resolution, satisfaction, and topics, built by Archika | App Launch and Feedback Review, Mar 10, 2026 |

## How a chat flows

```
Customer opens chat in the Varo app
        |
        v
Decagon reads the message and works out what the customer needs
        |
        +--> Answers from help content, or
        +--> Runs a workflow (for example, checking account details)
        |
        v
Answer checker reviews the answer against Varo's rules
        |
        +--> Resolved: customer can rate the chat
        +--> Needs a person: handed to a human agent with full context
        |
        v
Chat record masked for privacy and copied into Varo's data lake
```

## When chats go to a person

* The topic is outside what Decagon is allowed to handle, such as complaints about discrimination, possible fraud, or anti-money-laundering topics (How Decagon works walkthrough, Feb 11, 2026).
* The customer asks for a person.
* The queue is full. Decagon offers to keep helping, wait, or come back later (Decagon call, Jan 20, 2026).

## How the team watches it

See [Quality checks and monitoring](09-quality-and-monitoring.md).

## Not found in the meetings

* A written on-call or incident process for the live system.
* Formal numbers that would trigger pausing the rollout.
* Uptime or response time targets.

These are worth writing down as the system grows.
