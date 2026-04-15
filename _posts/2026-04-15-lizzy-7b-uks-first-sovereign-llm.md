---
layout: post
title: "Lizzy 7B: The UK Just Got Its First State-of-the-Art Sovereign LLM"
date: 2026-04-15
tag: opinion
---

Today at the Flower Labs AI Summit, Nicholas Lane unveiled Lizzy 7B... and it's a big deal. This is the UK's first state-of-the-art sovereign large language model, built entirely in the UK, trained on UK-relevant data, and open weights from day one.

![Nicholas Lane presenting Lizzy 7B at the Flower AI Summit 2026](/assets/images/lizzy_launch.jpg)

It's amazing to see the UK at the forefront of LLM innovation like this. London in particular has become a major hub for AI development, and this feels like a moment we should be proud of. I was there in the room when Nicholas demoed the model, and it's truly impressive.

The model is live on [Hugging Face](https://huggingface.co/flwrlabs/Lizzy-7B) right now under an Apache 2.0 license. No waitlists, no gated access. Just go use it.

**What makes it interesting**

Lizzy is a 7B parameter model, which puts it in the "actually runnable on reasonable hardware" category. But the benchmarks punch well above that weight class. It scores 77.9 on MATH (compared to 31.3 for EuroLLM 9B and 22.4 for Apertus 8B), 91.8 on GSM8K, and 70.2 on HumanEvalPlus. For a 7B model going up against 8B and 9B European competitors... those are striking numbers.

And then there's the Britishness benchmarks. Yes, that's a real thing. Lizzy scores 89.9 on Britishness Domains, 80.1 on Britishness CoT, and 71.0 on Britishness MCQ. It knows its way around UK law, compliance, and cultural context in a way that generic models simply don't.

![Lizzy 7B benchmark comparison against EuroLLM 9B and Apertus 8B](/assets/images/lizzy_performance.jpg)

**The SuperGrid angle**

What's quietly fascinating is how Flower Labs built this. Their SuperGrid platform enables decentralized training across distributed compute, networking different GPU clusters without centralizing all the data. IoT data stays in place. Proprietary datasets don't need to migrate to a data center. They effectively create virtual data centers by partnering with organizations that have idle GPUs.

This isn't just a nice-to-have architectural choice. For regulated industries (pharma, finance, public sector), keeping data where it lives while still training frontier models is a genuine unlock.

Flower has been at the cutting edge of federated learning, federated training, and model tuning for a long time now. And honestly, while a lot of the initial applications have been very interesting from a research perspective, commercial scalability has been a challenge. What excites me about SuperGrid and Lizzy is that it feels like the team is putting those years of deep experience to work in an area with significantly more commercial viability and utility. The market for sovereign, compliance-ready enterprise AI is broad and growing fast. It's really great to see Flower finding that fit. Kudos to the team.

**Enterprise ready, not enterprise gated**

Flower Labs is tagging this as "preview" but they're clearly confident. They're offering 24/7 support for direct enterprise integration, and early adopter organizations in the UK are already testing it. Key use cases center on internal AI infrastructure optimization, proprietary data integration, and compliance alignment for UK legal requirements.

The model supports up to 65k token context, runs on vLLM and standard inference stacks, and has a one-click deploy option via Hugging Face. The technical barrier to getting started is low.

**What's next**

Lane positioned Lizzy as "just the beginning." Expansion to Germany and other European nation states is planned, and the SuperGrid technology has global applicability. The open source community is encouraged to build on top of it.

For anyone working in UK enterprise AI, compliance-sensitive industries, or sovereign AI infrastructure... this one's worth paying attention to.

- [Flower Labs model page](https://flower.ai/models/lizzy/)
- [Hugging Face model card](https://huggingface.co/flwrlabs/Lizzy-7B)
