---
name: Scaling DevOps in a Digital Enterprise 
tools: [DevOps,Lean,Enterprise Agile]
image: /assets/images/scalingdevops.jpg
description: Whitepaper - From the lens of Agile and Lean
---

# Scaling DevOps in a Digital Enterprise

##### DevOps has revolutionized the way organizations manage software delivery. As every business is becoming an IT business, Software Delivery and Operational Performance plays a vital role in deploying changes, defect fixes, or configuration faster by removing waste in the delivery process. The Outcomes of software delivery and operational performance are measured not just by the speed of delivery but also by the software's stability.

##### There are reported isolated islands of success, but the undeniable fact is that automation tools or cloud adoption to try to achieve enterprise transformation have not worked effectively. The challenge emerges when scaling the success of small teams to an enterprise-level adoption, like how Scrum, an Agile framework, struggled. Using the yardstick of a small team's DevOps practices for enterprise fails because each business unit's dynamics differ in their culture, structure, technology stack, and the competition it faces. This article analyzes the challenges in managing high-velocity changes in an enterprise from the lens of Lean and Agile principles.

## Surviving High Velocity of Change

> Whatever got you here may well prevent you from getting there. — Marshall Goldsmith

As digital technology is becoming the core of every industry, organizations need to thrive in adopting technology faster, and infuse it into the mainstream to gain a competitive edge. But what is more important at the enterprise level is using these technologies to observe, measure, and quickly respond to customer needs. As software becomes ever more integrated into every product and service, making a big shift in rethinking and reorganizing quickly becomes the key operational challenge for businesses of all kinds. We need a management model that does not merely account for, but embraces, continuous change (Seiden & Gothelf, 2017).  

## Adoption of Agile at scale for enterprise
Agile paved the way for development teams to embrace change but did not do enough for business and operations. Agile at scale was challenging for larger organizations with a legacy mindset. They picked only the rituals like the daily scrum but implemented the "Water-Scrum-Fall" model (West, 2011). 
Large-scale Agile frameworks like SAFe, LeSS, Spotify, Nexus, and Scrum-at-Scale evolved to streamline the adoption in larger organizations. Some of the common challenges (Carrol, 2019) associated with large-scale Agile frameworks are:

* Inconsistency in defining the concepts and terms of scaling Agile.
* Readiness and appetite for adopting large-scale Agile frameworks.
* Balancing the organizational structure and large-scale Agile frameworks.
* Top-down versus bottom-up implementation of large-scale Agile frameworks.
* Lack of evidence-based use of large-scale Agile frameworks.
* Maintaining developer autonomy.

However, there is very little empirical research examining these large-scale Agile frameworks and their impact on the organization's transformation process in response to change. 

### Managing cross-functional requirement changes
Cross- or non-functional requirements like security and infrastructure are traditionally handled by Operations and Infrastructure teams. These teams are seen as support services in an enterprise. Research shows that most of these teams are "outsourced as a function" and that their agility is mostly governed by the processes (State of DevOps Report, 2018). Outsourcing is viewed as a quick way to expand capabilities and bandwidth. Driving change takes a long time as there are huge hand-offs involved. Generally, Operations teams are built around stability and not for speed.

### Responding through DevOps
DevOps emerged a decade back, laying a foundation layer on top of Lean principles, and resolving the weaknesses of Agile frameworks. Most organizations started their DevOps journey by building audacious goals to automate their current painful processes, like build and deployment, using CI/CD tools. These tools provided a quick win in terms of seeing features and defects move faster, mostly for product owner review in staging and sometimes to production. Beyond these advantages, it became difficult to showcase the value of a DevOps transformation to the business. Organizations recruited talent in the tool stack and claimed to be unicorns of DevOps. That DevOps team of unicorns helped automate the processes but did not have the opportunity to understand the end-to-end value stream. Ultimately, organizations suffered from having created a siloed team between dev and ops. As a result, DevOps is viewed as a methodology for automation and not as a value-driven initiative for its customers. 

### DevOps Research on High-Performing Organizations
At the beginning of 2014, DevOps Research and Assessment (DORA), which is now part of Google, built an empirical model to identify capabilities adopted by high-performing organizations and patterns that impede the others. The "State of DevOps" research annual report shared the relationship between organizational performance, IT performance, and DevOps practices.
DevOps research has consistently shown that high-performing organizations are building the intelligence needed to know their customers better, experiment with ideas that add value, and preserve the ideas that add customer value in a faster and more efficient way. They are also able to embed these capabilities across teams and business units. 

## Scaling from the Lens of Lean
Understanding the challenges an organization faces and best practices of high performing organizations in addressing them helps define the capabilities an enterprise should consider during their DevOps journey. Below are two models used in Lean manufacturing and currently in Lean IT.

### Continuous Improvement Vs. Innovation
From process and operational improvement, Lean practices talk about Kaizen, meaning Change for Better, and Kaikaku, meaning Reform, Innovate. These two models have evolved to address the challenges organization faces and approaches to improve the performance.
![Continuous Improvement Vs Innovation](/assets/images/sde/cii.jpg) 

In Kaizen, most of the improvement comes from the team, with small changes gradually over time. This model reaches its limits where you need a Radical breakthrough, Kaikaku, that disrupts the whole model process and practices. In Toyota Production System, Kaikaku is not used. Kaizen is seen for change for better, which could be big or small.

### Applying Theory of Constraint
The Theory of Constraint introduced in 1986 by Eliyahu M. Goldratt explains the importance of identifying the most important limiting factor (i.e., constraint) that stands in the way of achieving a goal, and then systematically improving that constraint until it is no longer the limiting factor. 
Agile was introduced when organizations saw that the waterfall methodology was a constraint on increasing the time to market while maintaining high quality. Over the years, as the speed of development has improved, the stability of the system became the constraint. DevOps was introduced to build a collaborative model to further improve speed and stabilize the system. Cloud Platforms came as a breakthrough to optimize the constraints in infrastructure management. Now, the constraint is spread across the organization. Unless we consider the value stream of the entire organization, we cannot optimize end-to-end value flow.

![Theory of Constraints  in IT](/assets/images/sde/leanenterprise.jpg)

## Scaling DevOps in an Enterprise
Gene Kim, in his article [State of DevOps 2020 and beyond](https://itrevolution.com/state-of-devops-2020-and-beyond/) , highlights larger organizations need ability to pivot and adapt quickly when changes hit them hard. Organizations need to have sense of binary thought process to manage changes that are innovative and changes that are improvements to the existing product or services. The DevOps capabilities required for these thought process differ.

### Explore Vs. Exploit Domain
Enterprises need to consider the lifecycle of businesses and how organizations balance the exploration of new models for innovation and the exploitation of existing products or services (Jez Humble, 2015). Exploring new opportunities and exploiting existing ones are fundamentally different strategies requiring different structures, competencies, processes, and mindsets. The capabilities that are effective in the exploit domain leads to failure if applied to exploring new opportunities—and vice versa. The differences between these two domains are listed in the below table:

| Component | Explore | Exploit |
|---|---|---|
|*Strategy*|Radical or disruptive innovation, new business model innovation|Incremental innovation, optimizing the existing business model|
|*Structure*|Small cross-functional multi-skilled team|Multiple teams aligned to the overall mission|
|*Culture*|High tolerance for experimentation, risk-taking, acceptance of failure, focus on learning|Incremental improvement and optimization, focus on quality and customer satisfaction|
|*Risk management*|The most significant risk is the failure to achieve product/market fit|A more complex set of trade-offs specific to each product/service|
|*Goals*|Creating new markets, discovering new opportunities within existing markets|Maximizing yield from the captured market, outperforming competitors|
|*Measure of progress*|Achieving product/market fit|Outperforming forecasts, achieving planned milestones and targets|

*Source: Lean Enterprise, O'Reilly Media, Inc.,*

### Identifying Capabilities for Explore and Exploit Domains
When identifying capabilities to improve the DevOps practices, most of the organizations uses a static DevOps Maturity Model. This model is used to evaluate all of its business units or teams assuming that “Level 1” and “Level 2” look the same across all teams and organizations. Maturity models are quite often a “lock-step” or linear formula, prescribing a similar set of technologies, tooling, or capabilities for every set of teams and organizations to progress through. 
In contrast, capability models are multidimensional and dynamic, allowing different parts of the organization to take a customized approach to improvement, and focus on capabilities that will give them the most benefit based on their current context and their short and long-term goals. For example, DevOps Research now part of Google and DevOn Enterprise Capability Model derives the future capability state based on Outcome to drive Software delivery and operational performance than by the static model.

## Building Enterprise DevOps Competencies
It is often challenging to nail down the competencies of a resource from DevOps' lens, not because it is one of the most challenging roles in the current dynamic workforce, but because it is still evolving. Currently, it is hybrid with both technical and non-technical skills in equal measure. Professionals in a DevOps Organization must balance soft, process, functional, and relevant technical skills. When transforming to DevOps, collaboration, cooperation, and acceleration are at their core. We need a T-Shaped profile in cross-functional teams focusing on the continuous flow of value and feedback. T-Shape profiles are essential for the Enterprise compared to core technical or domain skill because they can perform tasks within their specialization and help their teammates out. 
## Summary
Organizations accept DevOps to accelerate its value delivery and build resilience for sustenance in the high-velocity change. Identifying the capabilities to accelerate, continuously training on these capabilities, applying these capabilities across the Enterprise, and measuring the overall outcomes that impact the organizational performance are critical across the value delivery. 

## References
* Carrol, K. C. (2019, April). [Implementing Large-Scale Agile Frameworks: Challenges and Recommendations. Retrieved from IEEE Software.](https://arxiv.org/ftp/arxiv/papers/1901/1901.08130.pdf)
Forsgren, N. (2019). Accelerate: State Of DevOps. Google.
Jez Humble, J. M. (2015). Lean Enterprise. O’Reilly Media, Inc.,.
Seiden, J., & Gothelf, J. (2017). Sense and Respond. Harvard Business Review Press.
[State of DevOps Report. (2018).](https://puppet.com/resources/report/2018-state-devops-report/)
[West, D. (2011). Water Scrum Fall.](http://www.storycology.com/uploads/1/1/4/9/11495720/water-scrum-fall.pdf)



