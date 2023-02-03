---
title: A Generic model to define and implement a practice
tags: [capability model, practice]
style: fill
color: info
description: Framework to helps to implement any practice.
---
![Capability Model](/assets/images/capability-model/capability-model-framework.png)

Assume that you have taken a charge of heading a new division to build a practice like SRE. At first place you can ask google. But, it is 2023, so you surrender the question to ChatGPT. ChatGPT guided with the following steps:

![ChatGPT](/assets/images/capability-model/chatGPT.png)

You thought this response was generic and would attempt to ask a better question.

![ChatGPT-SRE](/assets/images/capability-model/chatGPT-sre.png)

Goodness! It is really good. The challenge is very point is broad. I tried different capabilities like cloud, devops, and agile. the steps are more or less the same. I thought I can help to generalize this better. So this is the blog with a picture (which can speak 1000 words) that it can’t do😊. I will explain this with an example of implementing SRE Practice.

## Starting with foundational principles
Wikipedia defines principles as “a proposition or value that is a guide for behaviour or evaluation. In law, it is a rule that has to be or usually is to be followed.” This is so important that model our every action. 
For example, SRE can have the following principle. 
“We approach Reliability engineering as an extension of DevOps Principles in the delivery of Business Value by optimizing the value stream for speed and stability. We apply CALMS model.
![SRE Principles](/assets/images/capability-model/sre-principle.png)

[Example](https://sre.google/sre-book/part-II-principles/)

## Defining the capabilities of SRE Practice
Good or ChatGPT can be a good start in identifying the capabilities. As this is an iterative process involving experts in whiteboarding the capabilities at a high level. As the capabilities evolve you can cluster them into a capability domain.
![SRE Capability Cluster](/assets/images/capability-model/sre-capability-cluster.png)

Alert: Tools can bias you in defining the capabilities. These capabilities should be independent of the tools. Later these capabilities will help you to identify the right tool and getting stuck with a tool which doesn’t support a specific capability.

## Mapping Competency and Roles with the capability
Competencies are the skill required to achieve the capability. LinkedIn Job Description could be a good start. You may need to go deeper based on the domain you are working with. For instance, the competency required for Network SRE will differ from the Database SRE.
Technology drives certain competencies. Building a broader scope will allow us to cross-skill resources. For example, Everything as a Code can be achieved using IaC technologies like Terraform or Ansible scripts. 
Alert: Most organizations struggle has the skill of a resource does not match the required capability. A good Assessment Model for capability and competency can drive adoption.

## Capability Patterns, best patterns and reference guides
This process of defining patterns is a critical part that guides the practice of certain capabilities. Many organizations publish reference libraries for teams to apply and mature. To make the adoption faster, Artefacts are supported with tools specific snippets, examples, and templates.

![incident response patterns](/assets/images/capability-model/incident-response-pattern.png)

Source: A Framework for Incident Response, Assessment, and Learning  - IT Revolution

Example: 

•	[Service Best Practices](https://sre.google/sre-book/service-best-practices/)

•	[Postmortem Culture](https://sre.google/sre-book/postmortem-culture/)

•	[Postmortem Template](https://www.atlassian.com/incident-management/postmortem/templates)

•	[Response Pageduty](https://response.pagerduty.com/)



