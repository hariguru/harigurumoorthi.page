---
title: Adopting DevOps for Legacy systems
tags: [DevOps]
style: 
color: 
description: >-
  From the business perspective – “Legacy system is one that is still adding some value to end users and is generating revenue directly or indirectly but of course tough to maintain and change.” Struggle for business is to bring innovative ideas quickly to market, to get a competitive edge and stay ahead.
---

From the business perspective – “Legacy system is one that is still adding some value to end users and is generating revenue directly or indirectly but of course tough to maintain and change.” Struggle for business is to bring innovative ideas quickly to market, to get a competitive edge and stay ahead.

This blog jots the steps from the consulting experience in adopting DevOps for a Legacy System.

## Step 1: Get the answer to “Why to adopt DevOps and the vision aligned – Top to Bottom

“To survive in the world of digital disruption, we will move all the projects towards Agile and DevOps” – I was reading a shout out from a new C-Suite executive. I was curious to observe DevOps adoption from this mid-size company started in late 2000. I tagged myself to the company’s social media and a few great people who were working towards this new direction. Sadly the initiative lost its momentum within a year. The main reason most of them shared was that the new process and tools made their life tough. People left the company due to high work pressure.

Maintaining a code of someone without rigorous testing and documentation is tough – Let us be frank here. DevOps starts with Culture. Understanding the teams’ struggle to keep the system stable for a change (the flow) is the biggest step before even embarking on the DevOps journey. If the team is able to visualize the vision of the end state without the struggle then the initiative will be of great success.

### Tools and Techniques

[5 Whys](https://www.mindtools.com/pages/article/newTMC_5W.htm)

[Simon Sinek Golden Circle](https://www.toolshero.com/leadership/golden-circle-simon-sinek/)

## Step 2: Build guiding principles and let the team choose what would work best for them
DevOps brings lots of best practices like Continuous Planning,  Continuous Integration, Continuous Testing, Continuous Delivery, Continuous Deployment, Continuous Monitoring, Continuous X, etc. Building an Enterprise DevOps Maturity Model across these areas and measuring the legacy system with the same yardstick won’t work, for a simple reason – not all the practices would be necessary and practical to apply.

A better approach would be to provide guidelines for each DevOps Practice with supporting tools and tricks. This would help the teams to evaluate and choose what suits the system

### Tools and Techniques

[Theory of Constraints](https://www.leanproduction.com/theory-of-constraints.html)

## Step 3: Define Measure to track the progress
For every chosen practice, identify 1 or 2 measures. Benchmark the current state and automate to collect the required data for the measure. For instance,  if the Legacy support team decides to modernize the legacy system by refactoring, or re-platforming its code, then it can choose to use continuous integration and testing.  Identify metrics that would validate the refactoring or re-platforming progress.

### Reference

[The Problem of Code Smell and Secrets of Refactoring](https://www.sealights.io/software-development-metrics/the-problem-of-code-smell-and-secrets-to-effective-refactoring/)

[Metrics based refactoring](https://www.researchgate.net/publication/3893282_Metrics_Based_Refactoring)

## Step 4: Automate High Value, error-prone, complex task first
I have seen teams maintain Continuous service improvement register to track automation opportunities. Rate those tasks by the Value it provides to the business, errors team will avoid and complexity of the task. Use techniques like Value Stream Mapping and tools that will reflect the overall throughput to identify the highest priority. Dedicate a resource similar to the role of an SRE who spends 50% of his or her time in automation.

### Reference

[Video: Value Stream Mapping for DevOps](https://www.youtube.com/watch?v=Z5zLhjH_VWU)

[Site Reliability Engineering](https://landing.google.com/sre/)

## Step 5: Celebrate and revisit to Step 2
Every milestone achieved is a reason to celebrate. Recognize the efforts and celebrate little wins. This is a continuous process. Start with the biggest pain area and move forward.

### Tools and techniques

[DevOps Culture and Mindset: Improvement Kata](https://www.coursera.org/lecture/devops-culture-and-mindset/devops-principles-improvement-kata-3VDu0)