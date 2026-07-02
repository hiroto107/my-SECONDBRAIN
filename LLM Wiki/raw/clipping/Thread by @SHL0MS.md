---
title: "Thread by @SHL0MS"
source: "https://x.com/SHL0MS/status/2043415274196435325/photo/1"
author:
  - "[[@SHL0MS]]"
published: 2026-04-13
created: 2026-04-15
description: "introducing Autoreason, a reasoning method inspired by @karpathy's AutoResearch which extends the strategy for subjective domains the paper"
tags:
  - "clippings"
---
**𒐪** @SHL0MS [2026-04-12](https://x.com/SHL0MS/status/2043415274196435325)

introducing Autoreason, a reasoning method inspired by @karpathy's AutoResearch which extends the strategy for subjective domains

the paper was co-written with Hermes Agent by @NousResearch, using a research-paper-writing skill developed while writing it

paper + results below

![Image](https://pbs.twimg.com/media/HFugOIWbIAAkICr?format=png&name=large)

---

**𒐪** @SHL0MS [2026-04-12](https://x.com/SHL0MS/status/2043415280953524404)

we show that iterative self-refinement with LLMs, no matter the prompt, usually makes things worse. the model hallucinates flaws to satisfy critique prompts, each pass expands scope unchecked, and models almost never decline to make changes even when they should

Autoreason fixes

![Image](https://pbs.twimg.com/media/HFui1jUaAAAHgdp?format=jpg&name=large)

---

**𒐪** @SHL0MS [2026-04-12](https://x.com/SHL0MS/status/2043415285592436819)

here's what a full autoreason trajectory looks like over 26 passes. the incumbent gets displaced, recovers, gets displaced again — convergence happens when the output is genuinely stable, not when the model runs out of things to say

with k=2, the AB synthesis from pass 13 wins

![Image](https://pbs.twimg.com/media/HFunFXfWIAEai3E?format=jpg&name=large)

---

**𒐪** @SHL0MS [2026-04-12](https://x.com/SHL0MS/status/2043415289916727379)

convergence speed varies by task complexity, but the method reliably terminates. policy tasks converge in ~10 passes. multi-stakeholder operational processes take up to 28. Monte Carlo runs on the same task show different paths but consistent final quality

![Image](https://pbs.twimg.com/media/HFuoTGVakAAw6c2?format=jpg&name=large)

---

**𒐪** @SHL0MS [2026-04-12](https://x.com/SHL0MS/status/2043415294098526251)

with Haiku 3.5 (~10x cheaper than Sonnet 4), Autoreason scored a perfect 42/42 Borda across three tasks; every judge preferred it every time. every standard refinement baseline degraded the same model's outputs below its unrefined single-pass

critique-and-revise averaged 16.3

![Image](https://pbs.twimg.com/media/HFukgmbawAAdF50?format=jpg&name=large)