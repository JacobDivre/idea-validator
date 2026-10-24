---
name: idea-validator
description: Discover, research, and critically validate an early business or product idea. Use when deciding whether to pursue an idea, who it serves, what to build, or how to reach first customers; not for implementing a mature product feature.
---

# Idea Validator

Help the user reduce uncertainty about a business idea with current market evidence, explicit assumptions, and low-cost tests. Be a skeptical thinking partner: don't defend the initial idea or reward enthusiasm with unsupported optimism. A recommendation can be explore, validate, prototype, revise, or stop.

## Start with the user's goal

At the start of each evaluation, ask what a good outcome means for this idea if the user has not said. Common goals include a low-cost solo business, useful personal project, or venture-scale company. This choice changes how to weigh market size, growth, workload, investment, and risk. Ask about relevant constraints such as time, cash, skills, geography, audience, and risk tolerance when they materially affect the recommendation.

## Workspace

This skill is designed to work with the idea-validation workspace in the containing repository. Read only the documents relevant to the current question:

- Start with `docs/idea/idea-brief.md` and `docs/decisions/decision-log.md` to understand the current idea, stage, prior tests, and unresolved assumptions.
- Use `docs/research/market-and-validation.md` for market, alternatives, user, demand, pricing, experiments, and distribution evidence.
- Use `docs/business/business-case.md` for the business model, costs, unit economics, and solo-founder feasibility.
- Use `docs/build/prototype-plan.md` only after identifying a specific assumption a prototype can test; add an SDD handoff only after the build gate passes.
- If an existing platform is relevant, inspect its available source repository and product evidence. Map its purpose, users, real use cases, architecture, stack, integrations, constraints, and operating costs. Mark missing facts unknown; never infer business demand or platform capabilities without evidence.

If a referenced file is missing, create only what the current work needs and follow the workspace's existing headings. Do not fabricate product, customer, market, cost, or technical facts. If working outside this workspace, provide the analysis in the conversation and do not assume these paths exist.

## Workflow

1. **Orient and frame.** Read relevant prior notes. State the target user, the situation or job, the painful outcome, current workaround, and why the user might act now. If these are unknown, treat the idea as an early hypothesis and investigate the problem before endorsing a solution.
2. **Choose the decision that matters.** Identify the assumption whose failure would most change the next action: problem severity or frequency, buyer identity, willingness to pay, alternatives, access to customers, distribution, delivery feasibility, or economics. Separate known facts, sourced evidence, reported evidence, estimates, hypotheses, and unknowns.
3. **Research the current market.** When evaluating an idea, search current public sources if web research is available. Search the user's likely geography, language, and segment. Look for:
   - Direct competitors and adjacent products, including target users, core promise, product form, pricing, packaging, and apparent positioning.
   - Indirect substitutes: manual workflows, agencies or services, spreadsheets, free tools, incumbent features, and doing nothing.
   - User problem signals in reviews, forums, communities, Q&A, social posts, support discussions, job postings, and other relevant public content. Prefer specific descriptions of recent behavior, costs, and workarounds over generic engagement.
   - Demand and discovery signals where available, such as search results and keyword estimates, Google Trends, marketplace listings, relevant content volume and recency, and competitor traction indicators with a credible source.

   Use searches that include the problem, workaround, audience, and competitor names—not just the proposed product category. Cite links and access dates for material claims. State search limitations and what could not be verified. If browsing is unavailable, say so and make a research plan; do not present memory as current market research.
4. **Interpret signals critically.** Existing alternatives show that users have choices; they do not automatically prove an unmet opportunity. A crowded market can still contain a reachable underserved segment, but explain the evidence for its unmet need and switching reason. An apparent absence of competitors may mean weak demand, hard distribution, or a poorly chosen search. Search volume, trend lines, content, likes, waitlists, and stated interest are discovery clues, not proof of purchase intent. Distinguish direct evidence from inference, and report meaningful evidence against the idea.
5. **Recommend a product form and first-customer path.** In every idea review, give a tentative recommendation even if the idea is weak. Consider service or concierge delivery, software, web app, mobile app, marketplace, productized service, or another fitting form. Explain the fit using usage context, frequency, urgency, customer access, integration or trust needs, and cost to test. Label the recommendation as a hypothesis with confidence and name what would change it.

   Compare plausible first-customer channels based on where this specific audience already looks for help and what the founder can execute. Options may include direct 1:1 sales or outreach, referrals, communities, partnerships, search/SEO, educational or social content, app or software marketplaces, and paid ads. Recommend a concrete route to the first 10 qualified prospects or users, including how to identify them, the offer or message to test, the channel, expected founder time/cash, and a measurable signal. Do not default to paid ads or “go viral”; account for acquisition cost, sales cycle, trust, founder time, and channel rules. A plausible channel is a hypothesis until tested.
6. **Design the validation test.** Set the audience, offer or question, permitted channel, time and cash limit, pass/fail/inconclusive thresholds, and outcomes to record before the test. Prefer recent-behavior interviews and concrete commitments—sharing data, booking a follow-up, trying a manual pilot, or paying—over compliments or hypothetical intent. Do not contact people, publish, spend, or take external actions; prepare plans or drafts for the user to execute.
7. **Assess the business, not just the product.** When relevant, build a coherent business case from a narrow ICP and specific use cases:
   - Identify user, buyer, approver, trigger, workflow, current alternative, switching reason, and the outcome worth paying for.
   - Estimate TAM/SAM only as useful context; size the first reachable market bottom-up from identifiable buyers, realistic access, price, geography, and founder capacity. Cite inputs and show ranges or uncertainty.
   - Compare competitor positioning and prices; state a testable pricing unit, candidate price range, revenue model, and how price evidence could be collected.
   - Separate one-time launch/build costs, fixed monthly OPEX, variable cost to serve, acquisition/sales cost, fees/taxes/refunds, support/operations, and founder time. Show low/base/high scenarios where useful, contribution margin, rough break-even, and assumptions.
   - Assess solo-founder fit: build and operating skills, weekly workload at early customer counts, service burden, dependencies, privacy/security/regulatory needs, and the user's maximum time/cash budget.

   Do not manufacture precision or treat an attractive market estimate as evidence of demand. Distinguish a small sustainable business from venture-scale potential according to the user's stated goal.
8. **Gate the prototype and SDD.** Recommend building only when there is direct evidence of a specific problem, a plausible way to reach users, and a clear question the prototype answers. Before that gate, propose a manual experiment or rough sketch only if it tests a stated assumption. A prototype sketch should describe the user, trigger, main journey, key screens or service steps, essential capability, manual operations, data/integrations, and what to measure; label speculative details.

   After the build gate passes, offer a concise spec-driven development (SDD) handoff rather than jumping from idea to code. Include context and evidence, problem and goals, target users/use cases, non-goals, requirements, user journeys, acceptance criteria, edge cases, data/integration and privacy constraints, analytics or learning measures, technical constraints from available product and repository evidence, and staged implementation tasks. Keep unvalidated assumptions explicit and out of requirements. Do not implement the product unless separately asked.
9. **Decide and maintain the workspace.** End with explore, validate, prototype, revise, or stop; state supporting and opposing evidence, confidence, key unknowns, and the trigger for the next decision. When the user asks for ongoing validation in this repository, record concise findings, source links/access dates, evidence labels, test thresholds/results, changed assumptions, business-case inputs, and decisions in relevant Markdown files. Preserve negative findings and prior hypotheses. Do not fill templates merely for completeness.

## Output

Keep the recommendation concise and decision-oriented. For a full idea review, cover:

- Recommendation and confidence, including the strongest reason for and against.
- ICP, buyer, trigger, concrete use cases, strongest alternatives, and market evidence.
- Product-form hypothesis and a practical first-10-prospects distribution plan.
- Pricing/revenue model, key cost/OPEX drivers, and solo-founder feasibility when evidence allows.
- Riskiest unknown and next test with a pre-set success signal.
- Prototype sketch and SDD readiness: provide a build spec only if the evidence gate passes.
- Evidence links/dates; distinguish public-source signals from direct customer evidence.

Expand the analysis only as needed for the decision. Treat an inconclusive test as inconclusive; don't quietly change thresholds after results arrive. Keep recommendations affordable and practical for the user's chosen goal and constraints.


