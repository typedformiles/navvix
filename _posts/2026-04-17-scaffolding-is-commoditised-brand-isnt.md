---
layout: post
title: "Scaffolding Is Commoditised. Brand Isn't."
date: 2026-04-17
tag: opinion
---

I spent an evening this week redoing [my wife's personal training business website](https://oneaura.fit). Not a weekend. Not three weekends. An evening.

If you'd asked me to do the same task 12 months ago I would have blocked out a stretch of days, braced myself, and started the familiar ritual... spinning up a virtual server somewhere, wrestling with a dodgy content management system that probably hadn't been updated since 2019, fighting with Webflow's abstractions when I wanted to do anything slightly unusual, hitting a theme that looked great in the demo but fell apart the moment I added real content, and generally banging my head against the wall until something shipped that was "fine."

This time I just... described what I wanted. Back and forth a few times. Iterated on the design. Added the copy. Deployed it.

**The stack**

The site is built in [Astro](https://astro.build/) with Tailwind, hosted on GitHub Pages out of a GitHub repo. In effect, the repo is the server. There's no CMS, no hosting provider to log into, no database to worry about. Push to main, the site updates.

There are trade-offs, of course. The most obvious is that it's a static site... no dynamic content generation at request time, no logged-in user experience, nothing that depends on a backend. For a personal training business that's not a real limitation. What matters is that the site loads fast, ranks well in search, and tells the right story about the brand.

Actually, for SEO, static might be an advantage. I built [isitaderby.co.uk](https://isitaderby.co.uk) on the same pattern and it's now ranking organically on page one of Google for some surprisingly competitive queries. Google seems to like fast, semantic, low-JS pages. Static-first architecture plays directly into that.

**Where the real work went**

Here's the thing that became very clear as I rebuilt this site: while the build and scaffolding is getting commoditised, the need for good content and imagery is going in the opposite direction. It's increasing.

AI has a tendency to converge on specific design themes. People use image models to generate very generic-looking imagery. They default to stock photography because it's easy. And none of this cuts through in human-centric industries like fitness and personal training, where trust and authenticity are the entire value proposition. Nobody is booking a PT because the hero image is a "professional woman in athleisure pointing at a clipboard."

You also cannot shortcut brand. In our case, we spent time several years prior thinking through brand language, working with a designer to land on the right colour palette, the iconography, the tone of voice. All of that pre-existing brand equity is what made the site redesign work. Without it, even the slickest coding agent would just produce another generic fitness template.

Take a look at 90% of PT websites and it becomes clear very quickly how low the bar is for the industry. Same two or three templates. Same stock gym photography. Same copy structure. That's the baseline. Any brand that actually invests in its identity stands out immediately.

**What coding agents actually unlock**

The real opportunity coding agents give small businesses isn't "a faster path to a generic website." It's access. Access to a build capability that was previously locked behind expensive agencies or multi-day DIY slogs. For businesses with strong brand foundations, the scaffolding getting cheap means time and capital that used to go into implementation can now go into the things that actually differentiate... photography, videography, copy that sounds like a human, the bits AI is worst at.

I've been in and around this industry for 20 years, watching a lot of "this changes everything" moments come and go. Most don't. But the step-change in coding models over the past year feels different, precisely because it's not flashy. The task that used to take days now takes an evening.
