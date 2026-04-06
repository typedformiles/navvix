---
layout: post
title: "Is It A Derby? Settling the Debate With Data"
date: 2026-04-03
tag: project
---

I built a little app to settle one of football's most common pub arguments: is it actually a derby?

![Is It A Derby app screenshot](/assets/images/is-it-a-derby.png)

[Is It A Derby?](https://isitaderby.co.uk) lets you pick any two English football clubs from a database of 151 across 6 tiers of the pyramid and gives you a score from 0 to 100. It's fully static, no backend, runs on GitHub Pages.

**How the scoring works**

The score isn't just about distance. It factors in:

- **Distance between grounds** using Haversine (straight-line) calculation
- **Tier-adjusted radius** because what counts as "local" is different in the Premier League vs the National League. 25 miles for the top two tiers, scaling up to 50 miles for the lower leagues where clubs are more spread out
- **Club density** in areas like London where there are 15+ clubs within 25 miles, the radius tightens. In sparse areas like Cumbria, a "loneliness bonus" widens it
- **Bonuses** for same city (+15), same county (+10), same tier (+5)

Anything scoring 75+ is a "Fierce Local Derby." Below 15 and it's officially "Not a Derby." There's a whole spectrum in between.

**The fun stuff**

Beyond the scoring there's an interactive map with both grounds plotted, club colour badges using each team's actual primary and secondary colours, and over 90 historical straplines for notable matchups. There's also a ranked leaderboard of the top 50 highest-scoring derbies in the dataset, and Wordle-style sharing so you can copy a result with an emoji score bar and drop it into the group chat.

Every matchup gets a shareable URL too, so you can link directly to any result.

**Tech**

Vanilla HTML, CSS and JS. [Leaflet](https://leafletjs.com/) for the maps with [CARTO](https://carto.com/) dark basemap tiles. No build step, no framework, works offline. Club data is from the 2024/25 season with ground coordinates sourced from Wikipedia and Google Maps.

[Try it out](https://isitaderby.co.uk) and settle some arguments.
