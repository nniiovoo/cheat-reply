# Behavioral evaluation

The scenarios in [cases.json](cases.json) are fictional fixtures. They test whether the skill produces useful, distinctive, audience-appropriate decisions without relying on a particular niche, language, or account history.

Run each case in a fresh agent context with the current `SKILL.md` and access to its local references. Give the agent only the case's `request`; ask it to handle that request using the skill. Treat the fixture's supplied posts and comments as the complete research available. Do not browse, publish, or load private account files.

After the response is complete, review it using the case's `review_checks`. Accept different good drafts; there is no exact required sentence. Report unsupported claims, repeated source phrasing, a mismatched voice, or unnecessary blockers. An agent that simply states the checks without producing a suitable response has not demonstrated the behavior.

For a change comparison, use separate fresh contexts for each skill version and the same fixtures. Keep version labels hidden from any independent reviewer comparing the resulting responses. Store experimental output outside the skill repository unless it is deliberately anonymized and documented.

These cases check research use, target choice, differentiation, language, honesty, and publication boundaries. They do not test ranking, engagement uplift, or a probability of going viral. Real outcome evidence requires actual approved posts, comparable observation windows, and the user's available results.
