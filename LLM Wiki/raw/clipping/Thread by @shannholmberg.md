---
title: "Thread by @shannholmberg"
source: "https://x.com/home"
author:
  - "[[@shannholmberg]]"
published: 2026-04-14
created: 2026-04-15
description: "how to use autoreason for marketing karpathy's autoresearch works when you have a number to optimize. conversion rate, pass rate, something"
tags:
  - "clippings"
---
**Shann³** @shannholmberg [2026-04-14](https://x.com/shannholmberg/status/2043983746094026984)

how to use autoreason for marketing

karpathy's autoresearch works when you have a number to optimize. conversion rate, pass rate, something measurable. but most marketing decisions dont have that

whats the right positioning? is this landing page copy good? does this email hook or does it just exist?

autoreason solves that. say you need positioning for a product launch

1\. you write the initial positioning (or an agent does). this is candidate A

2\. a fresh critic agent reviews A and tears it apart. whats generic, what a competitor could say word for word

3\. a separate author agent reads that critique and writes candidate B from scratch. no access to A, only the critique

4\. a synthesizer reads both A and B and creates a third option AB that pulls from each

5\. all three go to a blind judge panel. three fresh agents score unchanged A, synthesis AB, and revision B via borda count. they dont know which is which

6\. winner becomes the new A. loop repeats

7\. when A survives two rounds without getting replaced, youre done. thats your output

every role is a fresh isolated agent. the critic has no channel to the author, the judges never see the critic's reasoning. nothing leaks between rounds so you dont get the usual yes-man feedback loop where one agent just agrees with itself

your value prop goes through adversarial review instead of one agent's first take. landing page copy gets tested against agents trying to beat it. brand voice docs get refined through structured debate instead of a single prompt. ad briefs get sharpened round by round, each pass stripping whatever is generic

this is different from asking an AI to "make this better" because autoreason builds in disagreement. agent B is competing with agent A, the judges are blind, what survives that is stronger than what comes out of a single conversation

now add a knowledge layer. feed the critic and judges real performance data from past campaigns. without that data the loop debates from general copywriting principles. with it the loop debates from your results

what goes into the knowledge layer:

\> past campaign performance. open rates, CTR, conversion by segment, what moved revenue

\> winning copy and losing copy. the subject lines that hit 38% open rate and the ones that sat at 12%

\> audience research. what your customers say in reviews, support tickets, reddit threads

\> competitor positioning. how they describe themselves, where your messaging overlaps, where youre distinct

\> brand voice rules. the specific words, tone, and patterns that sound like you vs sound like anyone

example: you run this on email subject lines. the critic can now say "this reads like the subject lines that averaged 12% open rate for us, not the ones that hit 38%" instead of arguing from gut feel. the whole loop gets anchored to your numbers

every campaign result goes back into the knowledge base. the next run has better evidence to work with. the loop gets better the more you use it because the data it argues over is accumulating

> 2026-04-13
> 
> how autoreason works
> 
> Karpathy's AutoResearch but for tasks where there's no test to pass, content, strategy, positioning, copy
> 
> paper + code by SHL0MS, co-written with Hermes Agent by NousResearch 🧵 x.com/82948227531848…
> 
> ![Image](https://pbs.twimg.com/media/HF2wYo8b0AA09qh?format=png&name=large) ![Image](https://pbs.twimg.com/media/HFxu5_vacAA6D3x?format=jpg&name=large)