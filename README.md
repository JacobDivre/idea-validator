# Idea Validator

An evidence-first Codex skill and workspace for testing business and product ideas before investing heavily in a build. It is designed to question assumptions, research real alternatives, surface evidence against an idea, and recommend a practical next test—not to cheerlead.

## Use it with Codex

1. Clone this repository and open its root folder in Codex. The repo-scoped skill is at `.agents/skills/idea-validator/SKILL.md`.
2. Start an idea review with a prompt such as:

   > Use `$idea-validator` to evaluate this idea: [describe it]. My goal is [solo business / personal project / venture-scale], and my constraints are [time, budget, skills, geography, audience]. Research current competitors, substitutes, demand signals, and a first-customer channel. Be skeptical and tell me what would disprove it.

3. Continue with the recommended next test. The skill can help plan interviews or experiments, but it does not contact people or launch campaigns for you.

## What it helps you decide

- Who has the problem, what they do today, and whether the problem appears costly or frequent.
- Which direct competitors and substitutes exist, what they charge, and what customers complain about.
- Whether public signals such as Google Trends, search results, reviews, and relevant content support or weaken the idea. These are clues, not proof of willingness to pay.
- Which product form to test first, how to find the first 10 qualified prospects, and how to test a distribution channel.
- Whether pricing, startup costs, ongoing operating costs, and founder workload fit your goal.
- Whether evidence justifies a manual test, prototype sketch, spec-driven development handoff, pivot, or stop decision.

## Workspace templates

- [Idea brief](docs/idea/idea-brief.md)
- [Market research and validation](docs/research/market-and-validation.md)
- [Business case and solo-founder feasibility](docs/business/business-case.md)
- [Decision log](docs/decisions/decision-log.md)
- [Prototype and SDD plan](docs/build/prototype-plan.md)

The skill leaves unavailable facts as unknown and distinguishes sourced research from reported customer evidence and hypotheses.

## Limitations

Public research can identify competitors and signs of demand, but it cannot establish that customers will pay. Treat customer behavior and concrete commitments as stronger evidence. The skill reduces uncertainty; it cannot guarantee a successful business.

## Repository layout

- `idea-validator/SKILL.md` — canonical reusable skill package.
- `.agents/skills/idea-validator/SKILL.md` — repo-scoped Codex copy; keep it identical to the canonical package file.
- `idea-validator.md` — pointer to the canonical skill file.

## License

This project is dedicated to the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). You may reuse, modify, and distribute it, including commercially, without attribution. CC0 does not cover third-party material or grant patent or trademark rights. See [LICENSE](LICENSE) and the [full legal code](https://creativecommons.org/publicdomain/zero/1.0/legalcode).

