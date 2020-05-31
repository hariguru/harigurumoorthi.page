---
title: SRE 6 tips to regaining your error budgets
tags: [SRE, Error Budgets, SLO]
style: fill
color: info
description: Errors budget is an amazing quantitative measure to regain reliability in your system. This blogs describes highlights some of the techniques to reclaim the reliability and innovate
---

## Error Budgets
Error budgets can simply be defined as a quantitative measure to balance the feature velocity and the reliability of the system. This error budget can be compared with a maximum limit on our credit card purchase based on our income and capacity to repay without penalty. This will protect us from spending too much without knowing the risk. Error budget can be defined mathematically as

> ERROR BUDGET % = 1 – AVAILABILITY%

### Example of an Error Budget
Let us assume that you have a contractual obligation (Service Level Agreement) to provide service for 99.9% availability. Below is the math to calculate your Error Budget:

|||||
|--|--|--|--|
|**A**|ERROR BUDGET %|= 1 – 99.9%	|**= .1% OF UNAVAILABILITY**|
|**B**|NO., OF DAYS IN A MONTH|30 DAYS||
|**C**|TOTAL HOURS|	30 D x 24 H	|**720 HOURS**|
|**D**|UP TIME (HOURS)|(C) x 99.9%|**719.28 HOURS**|
|**E**|ERROR BUDGET (IN HOURS)|C – D|**.72 HOURS**|
|**F**|ERROR BUDGET (IN MIN)|E * 60 MIN|**43.2 MINUTES**|

## Exhausting Error Budgets
43.2 Minutes/month of Unavailability for a 99.9% availability is a tiny window for an issue to bubble up and operations team to fix it. Product owners should carefully define the availability that is manageable. The engineering team should continuously validate the features developed for its resilience.

![Error Budget](/assets/images/error-budget.png)
In the above example, the team has exhausted its error budget in 21 days. We can find more inferences from this measure:

* The Product Team is matured to survive 70% of its time (21 out of 30-day cycle) either pushing the features or bug fixes with the given error budget
* The Product team should prioritize 30% of its technical debt in its sprint schedule

## Techniques to regain your error budget
As we saw, the error budget is a good measure to build visibility and consensus between the product and operations team. Some of the techniques recommended by SRE practitioners that an organization can inculcate are:

### Freezing the feature releases
Stop more damage happening in production and focus the product team efforts to revive the reliability. SRE plays a vital role in analyzing the production challenges and helping teams to prioritize it. Conduct post-mortems to analyze the root cause and solutions to build more resilience. Product Owners can create reliability user stories with acceptance criteria to drive stability.

### Prioritize your Technical Debts to improve reliability
The interest we pay for not fixing a Technical Debt gets multiplied by X times when it goes to production. More we postpone fixing the debt; more it becomes challenging to remove the technical debt. The impact on the operations team grows exponentially, and automation also becomes a costly affair. Site reliability engineers can help to make the technical debt visible and help to prioritize it.

### Alter your release cadence
You can slow down and alter your release using canary and progressive deployment to reduce the number of users impacted by unstable releases. SRE can also look for a single point of failure in the deployment architecture. Modifying the release cadence provides a huge opportunity to test and learn in production with less impeachment.

### Revisit SLO with your Product Owner
If you see a trend in the error budget breaches, this may be a good sign that SLO is very high. You can use techniques like Toyota Improvement kata and redefine the next achievable target SLO.

### Improve monitoring and observability
Build capabilities that can identify the failures faster using proactive monitoring systems. The use of tools for Event Intelligence and AIOps drives a predictive approach in detecting the outages and availability challenges. The below metrics chart depict the relationship between product velocity and availability. For instance, the engineering team can measure the Time to Detect for troublesome features.

![Chart](/assets/images/metrics-chart.png)

## Automate your toils
Toils are a significant source of value leakage. Vivek Rau of Google defines toil as

> “Toil is the kind of work tied to running a production service that tends to be manual, repetitive, automatable, tactical, devoid of enduring value, and that scales linearly as a service grows.”

Find opportunities to automate the process of resolving the issues. SRE Workbook provides valuable guidance for eliminating toils.

## References
* [Risk and Error Budgets](https://www.youtube.com/watch?v=y2ILKr8kCJU)
* [Striving for Imperfection](https://www.usenix.org/node/189332)
* [Noise Reduction](https://blog.newrelic.com/product-news/noise-reduction/)
* [IBM Garage – Building SRE from Scratch](https://medium.com/ibm-garage/building-sre-from-scratch-485e23985bbd)
