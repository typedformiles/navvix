---
layout: post
title: "Databricks State of AI Agents: Thoughts and Commentary"
date: 2026-04-02
tag: opinion
---

I read Databricks' latest report on [The State of AI Agents](https://www.databricks.com/resources/ebook/state-of-ai-agents) with great interest last week. Databricks is in a great position to comment here thanks to the Neon acquisition, the scale of their AI/agent gateway and their position to own so much telemetry around who is doing what with AI. The report is built from aggregated, anonymised data across 20,000+ organisations including over 60% of the Fortune 500.

**The TLDR:**

- Multi-agent systems grew 327% in just four months, with supervisor agents (orchestrating multiple specialised agents) now the #1 use case
- AI agents now create 80% of databases and 97% of database branches, up from 0.1% two years ago
- 78% of companies are using two or more LLM model families
- 40% of top AI use cases focus on customer experience and engagement
- Companies using AI governance get 12x more projects into production
- Companies using evaluation tools get nearly 6x more into production

**On the 95% failure rate**

The report references a stat from MIT NANDA that 95% of generative AI pilots fail to get into production. I think this is wildly out of date already. We've seen such acceleration in the last 6 months that I'd argue that stat could be halved today. As evidence for this, the Databricks report itself claims to have observed that 97% of database branches and 80% of newly created databases are now done by AI agents. This is versus 0.1% a couple of years ago, so a truly profound growth rate. Things are moving fast.

**Governance as an accelerator, not a blocker**

The follow-on stat here is that according to Databricks, companies who are using a form of AI governance are 12x more likely to get their projects into production than those who don't. This is a great advert for getting AI properly organised across your org today, and not just cooking up MVPs on your own.

We see this ourselves at Neuralift; "doing AI" is more than just an idea, it's a business motion. The best results come from having access to the most data, which means working with all the right stakeholders and embedding governance into the process from day one. The companies that treat governance as a tax on innovation are the ones whose pilots never make it out of the lab.

**Multi-model is the new default**

78% of companies are now using multiple model families. Clearly there are two forces at play here. First, the use of models is more normalised and businesses are more au fait with their deployment, so the barrier to using multiple is much lower than before. Second, companies are learning that betting on one model alone brings risks with it and are insulating themselves.

This has implications for how you think about your martech stack too... Can you bring your own keys and deploy LLMs via your own gateway? This is going to be increasingly important. If your martech vendor locks you into a single model provider, you're taking on risk that the report suggests most enterprises are already moving away from.

**Built on Databricks**

We're proud at Neuralift to be a Built On Databricks partner, and to have a large percentage of our technical setup running on Databricks technologies from Neon to Delta to Unity Catalog. The infrastructure layer matters enormously when you're running deep learning at scale, and this report reinforces why.

[Read the full report here](https://www.databricks.com/resources/ebook/state-of-ai-agents) - it's really filled with good data and enterprise perspective on the acceleration of AI agents.
