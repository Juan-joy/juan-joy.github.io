---
title: "What a Closed Strait Teaches You"
date: 2026-04-19
---

On February 28 this year, military action in the Middle East effectively closed the Strait of Hormuz. Roughly a fifth of the world's oil flows through that chokepoint, and when shipping stopped, prices did what prices do in a crisis, they went sideways and then vertical.
I did a little deep dive into this as i thought that what happened next is a good case study in why commodity traders care about spreads and not just outright prices. Here are my findings from my research, hope you enjoy the read.

## The obvious story, and the more interesting one

The obvious story is that Brent went from $61 at the start of the year to $118 by the end of March, briefly touching $128 in early April. That's a headline move. It's the kind of chart that ends up on every news site and every trading desk's morning note.
&#x20;

The more interesting story is what happened to the Brent-WTI spread.
&#x20;

Brent tracks seaborne crude exposed to global shipping. WTI sits in Cushing, Oklahoma, and reflects a landlocked US market with its own inventory buffer. In normal times, the spread between them hovers around $4-6 per barrel, enough to compensate for the cost of moving a barrel from the US Gulf Coast to Europe or Asia, not much more.
&#x20;
In March, that spread widened to an average of $11 and peaked at $25 on a single day. The EIA called it the widest in over five years.
&#x20;
The reason is pure physics, not sentiment. Brent got expensive because it sits on the wrong side of a closed strait, because tanker rates exploded, because anyone who needed a seaborne barrel was suddenly bidding against everyone else who needed one. WTI got cushioned because US inventories were elevated, because the SPR was released, because landlocked barrels don't care about tanker routes.
Two crude benchmarks. Same molecule (well, roughly). Wildly different outcomes. That's a basis divergence, and it's the kind of signal a spread-aware trader would have seen coming from the moment shipping lights started going out.

## Why spreads beat outright prices

&#x20;
When you trade outright crude, you're taking a view on a whole tangle of things at once: demand growth, OPEC discipline, geopolitical risk, dollar strength, refinery margins, storage economics. It's hard to be right about all of them simultaneously. Most traders who blow up don't do so because they misread one variable. They do so because they misread the interaction.
Spreads strip most of that out. A Brent-WTI spread trade doesn't care whether oil is going to $50 or $150. It cares whether the relationship between the two benchmarks is where it should be. That's a narrower, more defensible question, and it's one that statistics can actually help you answer.
The same logic applies across commodity markets:

Crude calendar spreads tell you about storage and short-term supply tightness.
Crack spreads (crude vs gasoline or distillate) tell you about refinery margins and product demand.
LNG-oil parity tells you about gas demand versus its historical substitution relationship.
Palm oil–soy oil spreads tell you about vegetable oil rotation and biodiesel economics.

Each one is a simpler question than "where is this commodity going?" And each one, critically, tends to mean-revert. Outright prices drift. Spreads oscillate.

## Where anomaly detection actually earns its keep

A little while ago, I built a tool that watches commodity prices and flags statistical anomalies, specifically basis divergences that have moved more than a threshold number of standard deviations from their rolling mean. This started as a passion project to expose myself more to the industry and build something real.
&#x20;
The appeal isn't that it predicts the future. It doesn't. What it does is redirect attention. On any given day, most commodity relationships are behaving normally. The few that aren't are where a trader's time is most valuable. A z-score screen is a crude filter - genuinely, a blunt statistical tool - but it's the right kind of blunt. It surfaces things that a human would have noticed anyway, except it does it at 7am across every instrument you care about, without tiring.
&#x20;
The Hormuz episode is exactly the kind of event this kind of screen catches. You don't need the tool to tell you that something is wrong, the news tells you that. What you need is the tool to tell you which relationships are still distorted three weeks later, once the headlines have faded but the underlying disruption hasn't cleared. That's when the money is made.

## What I would look at right now
The Hormuz disruption is still priced in, but unevenly. The Brent-WTI spread has started to tighten, LNG basis between Henry Hub and Asian import prices is sharply elevated, and distillate crack spreads in New York are at multi-year highs. Somewhere in that set of dislocations, something is mean-reverting faster than the market expects, and something else is not reverting at all because the structural damage is permanent.
Figuring out which is which is the trade. A tracker doesn't answer that question for you. But it makes sure you're looking at the right chart when you sit down to think about it.

If you made it till here, thanks for reading, and if you are interested in the commodities space as well, feel free to reach out via LinkedIn.


&#x20;


Interested in the tracker I mentioned? More here: https://juan-joy.github.io/commodity-anomaly-tracker/

