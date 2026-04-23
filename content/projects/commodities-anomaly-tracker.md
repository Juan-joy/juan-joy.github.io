---
title: "Commodities Anomaly Tracker"
date: 2026-02-11
description: "A live data tool that pulls commodity prices and flags statistical anomalies and basis divergences across crude, LNG, and palm oil markets."
status: "Completed"
role: "Solo Developer"
timeline: "2026"
tags: ["commodities", "trading", "data", "javascript", "statistical analysis", "finance"]
---

A little passion project sitting at the intersection of chemical engineering and markets. I built this because I wanted to know whether I could turn a market instinct into something that actually runs.Commodity prices misbehave constantly, for example a spread blows out, a product crack snaps, LNG decouples from oil for a week and nobody agrees why. I wanted to learn more about this space and see if i could build tool that would notice those moments for me instead of making me squint at charts. So I did.

[**View the tracker →**](https://juan-joy.github.io/commodity-anomaly-tracker/)

> This live version runs on simulated data since Github only runs static pages. The full build with live price feeds from Yahoo Finance is available on request, feel free to reach out via LinkedIn.

## What it does

The tracker watches three markets, crude, LNG, and palm oil. And it flags two things: anomalies and basis divergences.
An anomaly is just a price that's moved far enough from its rolling mean that it deserves a second look. I use a z-score threshold, which is a blunt tool, but a useful one, as it catches the moments that a trader would have noticed anyway, and it does it without my attention.
Basis divergences are the more interesting signal. They track the spread between related instruments, Brent vs WTI, nearby vs deferred months, that kinda thing, and flags when that relationship drifts outside its historical range. Spreads tend to behave more predictably than outright prices, so when they break, something structural is usually happening: a chokepoint, a storage build, a refinery turnaround, a war.
The dashboard sits on top of all of that. Take a glance at it, see which markets are behaving oddly, click in if something catches your eye.

## Technical Stack

- JavaScript - Core application logic, statistical calculations, data pipeline (Huge Shoutout to Zan Wai for helping me with this)
- HTML/CSS - Dashboard layout, data visualisation, responsive design
- Price Data - Simulated in the public build, live feeds via API in the full version


## Why I built this
Firstly, I wanted to deepen my understanding in this space, and what better way to do that than via a little project? Most people applying for commodity trading roles understand markets conceptually. I wanted to build something that showed I could operationalise that understanding, to turn a trading idea into working code.
Flagging a z-score breach on a Brent spread is one thing to talk about. Building a tool that does it automatically, every day, without me, is another. And it forced me to think carefully about what actually counts as a meaningful signal versus noise, a question that matters much more in live markets than it does in coursework.
The tracker isn't a trading system. It's a noticing system. And noticing, I think, is where trading actually starts.
