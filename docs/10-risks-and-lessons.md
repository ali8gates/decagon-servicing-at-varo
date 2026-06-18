# Risks, issues, and lessons learned

## Issues we hit

| Issue | Effect | What we did | Source |
|---|---|---|---|
| Vendor data format changing often | Reports and dashboards broke | Advance notice process; keep a raw copy first | Decagon Blockers, Jan 29, 2026, Weekly team sync, data product, Jul 8, 2026 |
| Secure account connections running about 10 days late | Delayed account closing and card features | Engineering pushed the security work forward | Decagon company training, Apr 3, 2026 |
| Early resolution below Lex | 43% vs. 55% | Expected; closed by adding account actions | Decagon company training, Apr 3, 2026 |
| App Store approval timing | Launch date uncertain | Built the review loop to start the moment it was approved | App Launch and Feedback Review, Mar 10, 2026 |
| Too many handoff offers | Some customers pushed to a person unnecessarily | Deferred tuning until after launch | Decagon company training, Apr 3, 2026 |

## Lessons for the next rollout

1. **Start small and grow in steps.** Reviewing the first 100 chats caught problems before most customers saw them.
2. **Protect the data early.** Keep an untouched copy of vendor data so format changes do not break reports.
3. **Keep test sets small and meaningful.** Big automated test suites create noise.
4. **Expect the first numbers to look worse.** Launching with help articles only meant a lower early score. Tell stakeholders that up front.
5. **Analytics is a dependency, not an afterthought.** The data team became critical for proving each rollout worked (Weekly team sync, data product, Jul 8, 2026).
6. **Keep vendor control.** Owning the workflows let Varo move quickly without waiting on a partner.
