---
layout: post
title: "Designing Publisher Business Models for Humans and AI"
date: 2026-03-13
---

There's a question every publisher needs to answer in 2026, and most are not yet asking it clearly enough. It is not "how do we survive AI?" as this framing is very passive and ultimately too vague to actually act on.

The right question is this: who (_maybe even what_) is visiting my content, and am I running the right business model for each of them?

Right now two fundamentally different visitors are arriving at your content each day. They look nothing alike and they want very different things. The result is that they have different economics, and critically... they require completely different infrastructure to monetise their visits.

One of them is a human. The other one is a machine.

This article aims to dig in on each of the technologies, standards and monetisation stacks that could underpin each.

* * *

## Human Visits aren't Dead, but they are Changing.

I want to be clear about one thing up front; human traffic isn't totally disappearing overnight, but it is being mediated very differently especially as relates to web and written content.

The users who once typed a query into Google, scanned a bunch of links, and then clicked through to your article are increasingly getting answers without clicking. AI Overviews, ChatGPT search , Perplexity... these are the new front door, and they are increasingly staying closed to your actual URL ever being delivered to a user.

It's well documented that search referral traffic is down more than 50% for some publishers. This is a the biggest shift in how humans discover and consume information we've seen since the arrival of the internet itself.

But here is what matters and doesn't get discussed enough... the human visitor who **_does_** arrive is now typically more intentional, more engaged, and clearly often arriving via a different pathway. Direct, social, newsletters are more important than ever, and increasingly those visitors arriving via an AI assistant that decided your content is worthy of surfacing. The casual or transactional visit is declining for web publishers and the high-value visit is becoming a larger share of a smaller pool. This places less focus on ads ad more on CRM.

Human traffic as is no longer just a volume game.

* * *

## The Machine Visit is New and Nobody's Priced it yet.

At the same time a second type of visitor has arrived at pretty incredible scale, and this one didn't exist when you sat in the boardroom and designed your current business model.

AI systems... crawlers building training sets, RAG fetching real-time content, agents executing tasks on behalf of users... these are suddenly visiting (or _trying_ to visit) your content at incredible scale. They want to read your journalism, your weather data, your product reviews and your research. Their whole raison d'etre is extracting information, synthesising it, and then surfacing it inside AI interfaces to complete an often time-sensitive task. Usually without real attribution, I might add, and almost always without a click.

This visitor generates zero ad revenue under the legacy monetisation models. It doesn't trigger a page view and it absolutely doesn't see your banner or in-stream video ads. It does not subscribe. As it stands it just takes!

The economics here are genuinely broken. Not because the value isn't there, but because the commercial infrastructure to capture that value does not yet fully exist or hasn't been properly adopted yet. The machine is reading your content but the machine is not paying for it.

This is all about to change though and publishers need to prepare!

* * *

## Two Stacks Are Emerging- you Need Both.

The industry is in the early stages of building parallel monetisation infrastructures to adapt to these normalities. Each one is aimed at these two different visitor types, and understanding the difference between them is probably the most important strategic insight available to a media exec right now.

### Stack One: Human

This is the evolution of what we already know. Advertising, audience data, contextual targeting, subscriptions... but all rebuilt for a world where AI agents are increasingly involved in the process not just the audience.

On the ads front, two standards efforts are emerging here and it is worth understanding the difference between them.

**AdCP (Ad Context Protocol)** was launched in late 2025 by a consortium including Scope3, Yahoo, PubMatic and others. Built on top of Anthropic MCP it's agent-native by design and the idea is that a buyer's AI agent can describe a target audience in natural language, discover relevant inventory, compare pricing, and activate a campaign across platforms without custom integrations for each. Kind of like a new semantic layer for how advertising intent gets expressed and executed in an agentic world.

[https://adcontextprotocol.org/](https://adcontextprotocol.org/)

**ARTF (Agentic RTB Framework)** is the IAB Tech Lab's answer and rather than building something new from scratch ARTF extends the standards the industry already runs on... OpenRTB, OpenDirect, etc... using containers to make RTB faster and agent-compatible. IAB Tech Lab CEO Anthony Katsur has been publicly sceptical of AdCP, arguing the industry does not need to reinvent the wheel, and ARTF is his counter-proposal: upgrade the existing plumbing rather than replace it.

[https://iabtechlab.com/standards/agentic-rtb/](https://iabtechlab.com/standards/agentic-rtb/)

**UCP (User Context Protocol)**, donated to IAB Tech Lab by LiveRamp in late 2025 and now called Agentic Audiences" this tries to sit underneath both. It defines how agents exchange identity signals, contextual signals, and performance data in a privacy-safe, interoperable way. Think of it as the audience intelligence layer that can feeds whichever transaction framework wins out to enrich the user signals.

[https://iabtechlab.com/standards/agentic-audiences/](https://iabtechlab.com/standards/agentic-audiences/)

Whether AdCP or ARTF prevails or whether they coexist at different layers, which PubMatic and others argue is the likely outcome, the signal quality requirements for publishers are rising sharply either way. Richer, more structured first-party data will command premium rates. Thin behavioural signals and third-party enrichment will be squeezed.

But here is the thing the ads standards discussion mostly obscure... The most durable moat for a publisher in the new human stack has nothing to do with ads at all.

It is simply the direct customer relationship.

Subscriptions. Newsletters. Registered users. Known audiences with declared preferences and genuine loyalty. This is not a new idea it is actually a really old one. Publishers who built direct relationships with their readers before the programmatic era had something that the open web subsequently eroded: a CRM. Names, emails, preferences, history. A database of people who chose you.

That asset is now more valuable than it has been in twenty years. Because in an agentic advertising environment, the signal that commands the highest price is consent-based, first-party, and tied to a real person who has a demonstrated relationship with your brand. That is not a cookie. That is a subscriber.

So the media brands who will thrive as relates to the human stack are not necessarily the ones who implement AdCP fastest. They are the ones who spent the last few years rebuilding the direct relationship... the newsletter, the membership, the app, the registered login... and now have a genuine CRM to bring to the table.

Quality of audience over quantity of impressions. It sounds obvious but honestly most publishers still haven't done it!

### Stack Two: Machine-to-Machine

Now this stack is entirely new infrastructure, and it is having to be built from scratch because nothing that exists today handles it adequately. We can't take what we built for the programmatic era and just replatform it.

When an LLM's RAG pipeline tries to fetch your article to answer a user's question, there is no ad impression. There is likely no cookie, and there's no human to show a banner or video to. The entire architecture of digital advertising is irrelevant to this new type of content transaction.

What's needed here instead is a form of licensing and / or a micropayment layer that operates at the content level, in real time, and works machine to machine.

Several pieces of this infrastructure are now in motion simultaneously:

**CoMP (Content Monetisation Protocol)**, released this week by IAB Tech Lab for public comment this week, establishes a standardised framework for publishers to signal commercial terms to AI systems before content is accessed. It does not replace CDN-level blocking... it assumes you already have that. But it creates a structured path from restriction to licensed access.

[https://iabtechlab.com/standards/comp-content-monetization-protocols-initiative/](https://iabtechlab.com/standards/comp-content-monetization-protocols-initiative/)

**x402** - this is a HTTP micropayment standard championed by Coinbase and increasingly supported by Stripe and Cloudflare which provides a payment execution layer. When an AI agent hits a 402 response, it is being told: access requires payment. Remarkably HTTP 402 errors have been there forever, we just never saw them in the way we do 404s and 403s every day!

The x402 standard defines how a payment is negotiated and settled to access the HTTP resource and is typically in stablecoins resolved in milliseconds. Stripe launched x402 payments on Base in February 2026. and Cloudflare's support removes the bootstrapping problem at the CDN level.

x402 is something that I personally find fascinating as you can imagine a world where a user's token balance in Claude or OpenAI gets converted into USDC/T and is paid to a publisher in exchange for the content needed. All automated and handled by an agent with a wallet, no credit card needed. All of the major LLMs already have advanced metering through systems like Metronome (now part of Stripe), so the main open question here is how to define the exchange rate between LLM tokens and content value.

Micropayments for content have been tried many times before but bought way too much friction to actually work. The tech might just be catching up to the idea!

[https://x402.org](https://x402.org)

**Moszaic**, founded by James Curran (previously of STAQ), is building out the pricing intelligence layer. Helping publishers understand what their content is actually worth to an AI system, segment by segment, before they set floors. This is the same logic as ad yield management, applied to content licensing.

[https://moszaic.ai](https://moszaic.ai)

**TollBit and similar marketplaces** are starting to sit above these protocols as intermediaries, brokering access between publishers and AI systems, setting rate floors, and handling the commercial relationship at a layer above raw protocol implementation.

[https://tollbit.com](https://tollbit.com)

Taken together these are not competing, they are different layers of the same machine to machine stack. Permissions, pricing intelligence, brokerage, payment execution, settlement... I guess the equivalent in programmatic terms would be having an SSP, a DMP, an ad server, and a payment rail?

* * *

## The Lesson From Programmatic

In the early days of programmatic publishers faced a choice. They could hold their inventory back, invest in understanding its value, and negotiate from a position of quality - constrained confidence. Or they could open the firehose and accept whatever the market would pay.

Most publishers chose the firehose and sadly the results were catastrophic and largely irreversible. CPMs fell, margin got extracted by intermediaries, the audience data that publishers generated (perhaps the most valuable part of the whole system) got captured by platforms and data brokers, and not by the publishers themselves.

That mistake is available to be made again, right now, but with content licensing...

AI companies are currently paying for bulk content licensing deals with large publishers. The New York Times settlement with OpenAI, and Reddit, being the most prominant examples. But the terms of those deals have been set before any pricing norms actually exist for this new model. They're being made before publishers have the tools to understand their content's actual contribution value to AI systems, and before the aforementioned micropayment infrastructure that would enable seamless per-fetch pricing has been widely adopted.

Maybe pubs signing bulk deals today without understanding the per-fetch economics might end up being synonymous with making the same mistake as those who opened their inventory to programmatic in 2012 without yield management?

Moszaic's James Curran put it plainly in a recent conversation with me: "LLMs are going to pay zero until publishers can defend their rate floors"... the infrastructure to build and defend those floors is what is being constructed by him and others right now and we should all pay attention.

* * *

## What This all Means in Practice

So for a media executive thinking about where to focus in the next 12 months, the bifurcation suggests a clear set of priorities...

**On the human stack:** invest in first-party data quality and structure. The signal requirements for AdCP and UCP-compliant programmatic are higher than today's standard. Media owners with rich, well-organised and hopefully differentiated audience and content data will be able to command premium rates. Those relying on third-party enrichment or thin behavioural signals are going to be squeezed further. You have to double down on your 1P estate here. Investigate the cutting edge of segmentation and value extraction from your data today so that you have the strongest possible foundations around your human audience to deliver deep context to these agentic protocols.

**On the machine stack:** start exploring and building the infrastructure now, before pricing norms harden. This might mean implementing CDN-level access controls, engaging with CoMP's public comment process, starting to understand x402 and what it might mean for your content architecture if users are able to authorise a micropayment to get the content they need for the LLM workflow they are in the middle of, and finally getting serious about content valuation.

**On pricing:** It's likely tempting to sign a long-term bulk licensing deal but be conscious of tjhe fact  that without understanding where per-fetch economics might take us this could undersell in the mid to long term. Bulk deals are revenue today and traditional publishers are under pressure but it may be a floor that is hard to escape later.

**On both:** recognise that these two monetisation models may require different teams, and different data infrastructure, and probably different commercial relationships. The person who manages your ad server setup isn't necessarily the same person who should will define the rate floors for serving millions of markdown files a day to a bunch of machines.

Two distinct types of visitors - Two business models.
