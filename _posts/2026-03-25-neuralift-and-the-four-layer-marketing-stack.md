---
layout: post
title: "Neuralift and the Four Layer Marketing Stack"
date: 2026-03-25
tag: opinion
---

I've been doing some noodling on how best to represent Neuralift's position in the marketing and data stack and settled on a four tier model with us occupying two layers in the middle. That might seem self-serving for Neuralift to take 50% of the stack, but bear with me...

![Neuralift Four Layer Stack](/assets/images/neuralift-stack.png)

**Layer 1: 1st Party Data Sources**

Wind the clock back 18 months or so and ML would probably have been a layer in its own right, but this has gradually collapsed into layer 1 - the data foundations. ML and manual data science are valuable but this is table stakes today and is fundamentally part of your data warehouse / lake approach now. Your AWS, Google Cloud, Snowflake, Databricks, etc.

**Layer 2: Deep Learning and Segment Discovery**

Deep learning and discovery have emerged as the new frontier on top of these 1st party data foundations, but they are fundamentally HARD things to do. As my CEO Jon recently wrote in a [LinkedIn post](https://www.linkedin.com/posts/jonathanmendez_a-shift-i-think-matters-a-lot-right-now-share-7442195635874963456-a-q4):

> "Advantage now is not measurement. It is using customer data to discover hidden patterns, untapped opportunities, and strategic moves that are hard to see through reporting alone"

But back to this being hard. Training, iterating and fine-tuning a model to support the specific use case on top of the 1P is not a menial task. Adapting your data to be AI ready - hyper-parameterising but let's keep it simpler; feature engineering, lots of booleans, banding constants, etc - is a huge undertaking, and that's before you've even tried to get hold of enough GPU clusters to run the job. Most companies are not Netflix or Amazon. Neuralift at layer 2 represents a turnkey pipeline for both the model and the GPU compute. It makes no sense for 99% of clients to go off and do this themselves due to cost, time and complexity.

**Layer 3: Context Building and Actionable Intelligence**

The layer above this is all about reasoning, explanation and humanising of the neural network outputs. How do you get that valuable information that is found as part of deep learning and make it useable and actionable by business teams instead of it being trapped inside a data lake? 

At this level there's a temptation to think you can just point an LLM at the tables being created by the prior layer of the stack, but it's much more nuanced than that. Yes using LLMs is important here in converting 1s and 0s into human readable information, but bneyond that you also need to have an opinion. This is the one things that LLMs fail on consistently, but that a good martech data tool needs to have in 2026. In this context opinion means an app that has industry-tuned reasoning models, that understands the domain and your aims, and ultimately makes sure that outputs are KPI-aligned to root the whole exercise in value creation. Oh, and a nice UI! Never underestimate the value of a good UI :)

**Layer 4: Activation, Execution and Agentic Systems**

And finally the activation stack, which is changing. It used to be that you would take a segment or segmentation and the only endgame was to push it to an API like Meta, your ESP, etc. Now there's a whole necessity to make sure that the data tools and applications you're working with can export all of the new data to agentic systems.

![Tony Kipkemboi tweet on enterprise SaaS and agent-first tooling](/assets/images/tony-kipkemboi-tweet.png)

[Tony Kipkemboi's recent tweet](https://x.com/tonykipkemboi/status/2035051776110375405) nails this. Enterprise customers care most about being able to give their agentic layer access to their data in the most efficient and comprehensive way, and less so about your harness. Build better MCPs, CLIs, APIs. New startups will start popping up that are agent-first and your customers will eventually switch if you don't innovate.

**Feeding the machine**

The way the world's most powerful performance oriented systems work today is a combination of great data foundations, deep learning / neural networks on top of them, feeding into reinforcement learning and recursive loops. This is how the likes of Google Pmax, Meta Advantage+, Amazon Performance+ and even the new breed of agentic solutions are fed. So feed your own systems what they want - better clusters, with better reasoning and every single scrap of maths that went into the decisioning.
