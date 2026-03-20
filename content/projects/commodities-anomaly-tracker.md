\---

title: "Commodities Anomaly Tracker"
date: 2026-02-11
description: "A live data tool that pulls commodity prices and flags statistical anomalies and basis divergences across crude, LNG, and palm oil markets."
status: "Completed"
role: "Solo Developer"
timeline: "2026"
tags: \["commodities", "trading", "data", "javascript", "statistical analysis", "finance"]
---

A passion project sitting at the intersection of chemical engineering and markets. Built to sharpen my intuition for commodity price behaviour and demonstrate that I can turn a trading idea into a working tool.

[**View the tracker →**](https://juan-joy.github.io/commodities-tracker/)

> The live version runs on simulated data. The full build with live price feeds is available on request, feel free to reach out via LinkedIn.

## What It Does

The tracker pulls commodity price data across crude oil, LNG, and palm oil and applies statistical methods to surface two things traders care about: **anomalies** and **basis divergences**.

Anomalies are flagged when a price moves beyond a defined standard deviation threshold from its rolling mean — a simple but effective signal that something unusual is happening. Basis divergences track the spread between related instruments or delivery periods, highlighting when that relationship drifts outside its historical range.

The result is a clean dashboard that gives a fast read on where prices are behaving unusually, without needing to stare at raw data.

## Technical Stack

* **JavaScript** — Core application logic, statistical calculations, data pipeline
* **HTML/CSS** — Dashboard layout, data visualisation, responsive design
* **Price Data** — Simulated in the public build; live feeds via API in the full version

## Why I Built This

Most people applying to commodity trading roles understand markets conceptually. I wanted to build something that showed I could operationalise that understanding — translate a trading insight into working code. Flagging a z-score breach on a Brent spread is one thing to talk about; building a tool that does it automatically is another.

It also forced me to think carefully about what actually constitutes a meaningful signal versus noise, which is a question that matters a lot more in live markets than in coursework.

