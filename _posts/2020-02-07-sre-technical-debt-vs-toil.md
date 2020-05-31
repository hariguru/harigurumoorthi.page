---
title: Site Reliability Engineering - technical-debt-vs-toil
tags: [SRE, Technical Debt, Toil]
style: fill
color: info
description: Realizing Technical Debt is one of the key sources of Toil helps SRE Squads/teams to prioritize their automation efforts
---

## @ 2 a.m….
Sreejith, a smart and young SRE engineer was on-call last Sunday. Around 2 AM he got an alert: “Azure Virtual Machine Scaled set reaching its threshold”. It took some time to get out of his deep sleep. He boosted his mind with a dose of caffeine and started running a few LogAnalytics queries to hunt down the problem. It was the last evening release that occupied the heap memory and in-turn making the Virtual Machines busy. He ran a few clean-up workbooks but unable to bring the system to normal conditions. It was time to pull the Andon Cord! He created a Slack channel to wake up the dev and other dependent teams to resolve the issue. Developers provided a patch and by 6:30 AM the system came back to normal. Sreejith was tired and wanted to take a day off, but his manager called for a post-mortem meeting at 10:00 am so that this incident doesn’t happen in the future.

## Lessons from the Post-mortem
The post-mortem meeting went in a blameless way and teams were able to nail down the problem. The root cause was that the new algorithm deployed was not fully tested. Performance testing results were below the mark, but the team took a chance to fix the performance issue in future sprints. Sreejith was frustrated a bit but decided to hang out with his colleagues than going to bed in noon.

If you are an SRE or in a similar role, you will have a similar (even bitter) experience. In the SRE world, 2 am experience of Sreejith is a kind of Toil, but the root cause for the toil is the Technical Debt that the development team decided to pay later.

## What is a Toil – A SRE perspective?
As per Vivek @ Google, “Toil is the kind of work tied to running a production service that tends to be manual, repetitive, automatable, tactical, devoid of enduring value, and that scales linearly as a service grows.”


|Toil Characteristics |Example|
|-----------------------|-------|
|Manual	|Running manually executing an automated script|
|Repetitive	|Acknowledging every morning, an overnight alert without doing anything about it|
|Automatable	|Move logs from production server to cold storage|
|Tactical	|Deploying to Servers|
|No enduring value	|Creating SLI reports to management on a weekly basis|
|Linear scaling	|Increase in the number of tickets for the same issue every release|

## What is Technical Debt?
Technical Debt is a metaphor introduced by Ward Cunningham in 1992, stating that “a little debt speed development so long as it is paid back promptly.

> “Technical debt is a concept in software development that reflects the implied cost of additional rework caused by choosing an easy solution now, instead of using a better approach that would take longer.” – Wikipedia

## When does Technical Debt occur in Agile projects?
As business looks for deploying features rapidly, it expects the IT teams to handle the non-functional aspects like reliability, performance, security. As the non-functional requirements (NFR) are not visible in user stories, in the given sprint, IT teams may oversee the NFRs. If it is known it may not get listed in the backlog.  Slowly we lose track of these debts.

## Technical Debt is a source of Toil
Dag Liodden, in his [blog](https://hackernoon.com/there-are-3-main-types-of-technical-debt-heres-how-to-manage-them-4a3328a4c50c), discuss three type of Technical Debts.

* Deliberate tech debt
* Accidental/Outdated design tech debt
* Bit rot tech debt
The scenario we described earlier is a kind of deliberate technical debt which surfaced in production. It was easier to identify the technical debt as the proximity of the outage was closer to release. The other two types may take a longer time to identify unless tracked in the backlog.

Toils can be automated faster when the proximity of the release that introduced the technical debt is close.

## What can we do about it?
**Make Technical Debt visible to SRE and operations team**

* Track them and discuss during your review calls will help the SRE to be prepared. “Communicate Well”
* Trace toils to technical debt
 

**Build an effective feedback loop to the dev team**

* Helps to prioritize better
* Provides visibility to the Product Owner and management