---
title: Building High Performing Data Teams
tags: [Culture, HPT, Data Teams]
style: 
color: blue
description: >-
  This paper analyzes the factors that impacts high performance in teams, in a globally distributed and culturally diverse setup, and provide a model that can help data teams like Business Intelligence, Data Analytics and Science and, Data Engineering.
---

# ABSTRACT
This paper analyzes the factors that impacts high performance in teams, in a globally distributed and culturally diverse setup, and provide a model that can help data teams like Business Intelligence, Data Analytics and Science and, Data Engineering. This paper also attempts to give a holistic view of capabilities as a team should possess and competencies or skills of an individual should develop to drive high performance.  Literature review includes myriad of research works, models applied by top companies, and proven approaches from the practices and frameworks like Agile, DevOps, SRE, SAFe, TOGAF, BABOK. 

# INTRODUCTION

> "Getting good players is easy. Getting them to play together is the hard part.” – Casey Stengel

As per Wikipedia, A high-performing team (HPT) is a group of individuals with specific roles and complementary talents and skills, all aligned with and committed to a common purpose, who consistently show high levels of collaboration and innovation, produce superior results, and extinguish radical or extreme opinions that could be damaging. 
From the context of organizations, they invest on building high-performing teams to deliver business value, expecting them to be productive and perform well in achieving given goals. 

The concept of **productivity** and **performance** is a century old, researched domain and continuously evolving every time when technology disrupts the existing way of working. Mobile and Cloud disruption is now succeeded by Generative AI.  Organizations, based on its agility, redefine itself to adopt and enable teams and individuals to improve their performance for delivering business value. 
These types of adoptions, which are radical in nature, need huge investments and initiatives mainly for large companies. Most of these initiatives are run as transformation programs with multiple phases. To achieve high productivity, organizations use models in building and nurturing teams. Some known models [1] are:

* GRPI (Goal, Roles, Procedures, interpersonal relationships) Model
* Hackman Model
* T7 Model
* Lencioni Model
* Tuckman Model

Two common dimensions that arise out of these models are:
* **Practices** – capabilities that enable the people to achieve the vision. This includes framework, models, process, procedures, standards, and techniques.
* **People** – management of human talent, skill or competence, roles they play and how they collaborate. This includes Organizational structure, culture, relationships, and environment.

For consistency, this paper uses capability to represent the practices and competency to represent the people aspects in building high performing teams (HPT).

## CHALLENGES IN BUILIDING HIGH PERFORMING TEAMS
Organizations encounter bottlenecks in building HPT when they focus only on competencies or the capabilities. Both are intertwined and need continuous assessment and improvement. Case studies [2] have shown HPT if not defined well struggle with:
*	Hero culture,
*	Imposture Syndrome
*	Low Confidence
*	Burnouts,
*	Ineffective work practices, 
*	Ego, and cultural clash. 

# IDENTIFYING CAPABILITIES (PRACTICES) OF HPT
Capabilities are the building blocks that encapsulate a team’s ability to perform specific activities or deliver desired outcome. 
Which one should be defined first? People or Practice. Even though, this is an iterative approach, starting with the capabilities required to achieve the vision, we help to define the role and competence required. 
## IDENTIFYING CAPABILITIES BY DEFINING VALUE STREAMS
A value stream refers to the sequence of activities necessary to deliver a product, service, or experience to a customer, whether internal or external. It encompasses every touchpoint along the journey from idea generation to the delivery of value to customers. Here are some key points about value streams:

### Definition:
![Valuestream](/assets/images/hpdt/valuestream1.png "Value stream")

A value stream always begins and ends with a customer. It encompasses the entire lifecycle of delivering value.
Understanding value streams is crucial for making informed decisions. By mapping out these streams, organizations can allocate resources effectively and avoid wastage.
Without this knowledge, it’s challenging to identify what’s working well and where problems exist. For instance, lengthy delays during handoffs between teams can hurt productivity and quality.
Team can define multiple value streams based on the user journey. For instance, ODI Ways of Working defines, Front Door flow independently for new requirements, change requests, defects, and consultancy. Every flow involves certain capabilities and competencies. Below data analytics value stream flow is a simplified version of a new requirement flow.

![Data Developement Value stream](/assets/images/hpdt/data-vs.png "Data Analytics Value stream")

Each process step in the above diagram may contain sub processes and end with capabilities.

**Example:**
Discovery process involves certain set of practices like requirement gathering, planning, building roadmap, data discovery, customer value mapping. Mapping the capabilities and the features required will help to identify the tools and techniques to enable better performance.

![Data Value Stream Capabilities](/assets/images/hpdt/data-vs-capability.png "Data Value Stream Capabilities")

## IDENTIFYING CAPABILITIES TO MINIMIZE VALUE LEAKAGE
One of the critical steps in building HPT is to identify activities that do not directly contribute value to the end product or service from the end-user perspective. These activities slow down the teams and impacts their productivity.

![Data Value Stream Value Leakage](/assets/images/hpdt/data-vs-leakage.png "Data Value Stream Value Leakage Analysis")

Following are common value leakages (waste or Muda) that happens in Data teams:
| MUDA TYPE | DESCRIPTION |
| --- | --- |
|Transportation|While transportation itself is not inherently wasteful, excessive movement of data between systems, teams, or processes can be wasteful.|
|Inventory|Excess process of Data which is not used causes scalability / memory issues in Database.|
|Motion|Excessive motion refers to unnecessary movement of data or people. Duplication of Data across schema, processing time issues are typical problems data teams go through.|
|Waiting|Waiting occurs when data processing or decision-making is delayed. Waiting for Deployment, waiting for approval are good examples in this type.|
|Over-processing|Over-processing involves spending more effort or time on data tasks than necessary. Examples - Poor architecture, lack of automation.|

*Organizations build rich feedback loops using Monitoring and Alerting capabilities to visualize these type of value leakages. Value stream mapping exercise bubbles up these problems. *

## IDENTIFYING CAPABILITIES BASED ON EVOLUTION
Organizational dynamics change over time in the value, maturity, and predictability of capabilities within a value stream. Evolution describes the team’s collective learning journey, from being excited by novelty to becoming bored by ubiquity. Simon Wardley describes four phases of evolution [3]:

**Phases of Evolution:**
**Genesis**: capabilities in this phase possess significant potential but lack practical use today. They are highly experimental or even theoretical. Example - Headless BI – Capability that separates the metric definition from the visualization.

**Custom-build:** This phase includes bespoke capabilities, built for specific environment. These practices or capability is unstable or go through frequent changes. 

**Product:** This phase represents the increasingly common, the more defined, the better understood capabilities. Change becomes slower here with increased level of stability.

**Commodity:** This represents scale and volume operations of production, the highly standardized, the defined, the fixed, the undifferentiated, the fit for a specific known purpose.

Below Wardley map [3] is an example of a data team capabilities, its current and future evaluation stage in horizontal axis and visibility of the capability in the value chain from the eyes of customers.  Circles in red are potential future capabilities which trigger higher order opportunities and capabilities. For instance, migration of Qlik from on-premises to cloud Saas version will redefine some of the ASG model and enable DevOps practices.

![Data Wardley map](/assets/images/hpdt/wmap.png "Data Wardley map")

## TOOLS MINDSET IN IDENTIFYING CAPABILITIES
One anti-pattern that exist in building required capabilities is by picking the (favorite) tool that solves the specific problem. Challenge is the tools landscape  is huge and vendors compete with the features the tool can support. Choices are made based on Open source to commercial, licensing model, support model, and talent availability. Teams struggle with following problems with incorrect choice:
*Lack of Tools Chain or Integration between downstream and upstream tools
*API and CLI availability
*Maintainability and upgradability
*Elasticity or scalability
*Security

![Data Tools](/assets/images/hpdt/nata.png "Data Tools Landscape")

# IDENTIFYING COMPETENCIES (SKILLS) OF HPT
As we saw in the introduction section, much research works and models exist to identify and build the competencies required for the team.  Common attributes of high-performance team are:
*Trust and Respect
*Psychological Safety
*Clear Goals and Alignment
*Clarity in Roles and Responsibilities
*Culture of Continuous Learning
When transitioning to an Agile organization, we frequently shift from specialized teams to teams with diverse skills. Cultivating a broadly skilled workforce facilitates improved collaboration within cross-functional teams. Rather than functioning as isolated groups, these teams work together to solve problems, avoiding a sequential approach. This collaborative approach fosters highly effective teams, enabling innovation and the creation of superior solutions.

## BUILDING T-SHAPED PROFILES
The consequence of building an expert team is the development of Hero culture. Transitioning from a hero culture to a team culture within HPT is a pivotal shift. In a hero culture, individual brilliance and heroics take center stage. Singular contributors are celebrated for their exceptional achievements, often overshadowing collective efforts. However, in a team culture, the spotlight shifts to collaboration, shared responsibility, and mutual support.
In HPT, T-shaped skills play a crucial role in fostering collaboration, adaptability, and overall effectiveness. Broad Base (Horizontal Bar) represents a breadth of knowledge across various domains. Team members possess foundational skills that span beyond their specialized roles. 
Some of the broad skills includes:
* **Domain Knowledge –** Telecom Domain and regulations. Knowledge on Fibre, Ethernet and Copper, L2C and T2R Journeys
* **Agile and Lean Thinking –** Embrace change and solution just enough to solve the business problem, collaboration with internal and external stakeholders, problem solving.
* **Data Fluency –** Data management and governance, importance of data quality, data wrangling and cleaning, data visualization.
* **Requirement Management –** Translating business requirements to technical user stories, documentation of user flows.
Deep Expertise (Vertical Stem) signifies deep knowledge in a specific area. Each team member excels in their specialized field, whether it's discovery, design, testing, data analysis, or project management. This depth of knowledge enables them to tackle complex problems within their domain. It also fosters a sense of ownership and accountability.
Below diagram [4] from McKinsey provides three categories of skills. Mapping the deep expertise with the capabilities of identified will provide role clarity. 

![T Shape Profiling](/assets/images/hpdt/nata.png) "T Shape Profiling")



# MAPPING CAPABILITIES AND COMPETENCIES

![Capability Model](/assets/images/capability-model/capability-model-framework.png "Capability Model Framework")

Above diagram [5] provides a view of how organizations can build a community of practice combining the capabilities and the competencies required for a specific purpose. Each squad can identify campaigns to build the required knowledge to improve the productivity of the team. Continuously identifying opportunities to save time and improve quality reduce the efforts required to rework and testing cycles. 

# REFERENCES

[1] 	S. Jay, "Team effective models," Academy of Innovative HR, [Online]. Available: https://www.aihr.com/blog/team-effectiveness-models/.

[2] 	G. Bradt, "Why the Highest Performing teams always fail over time," Forbes, 2019. [Online]. Available: https://www.forbes.com/sites/georgebradt/2018/10/30/why-the-highest-performing-teams-always-fail-over-time/?sh=8f3867430dc6.

[3] 	N. Jones, "Mapping the Data Analytics Landscape," Jan 2022. [Online]. Available: https://medium.com/@nathanjones_77/mapping-the-data-analytics-landscape-chapter-1-8c5470fa0fdc.

[4] 	"Ops 4.0 Engaging your people," McKinsey, [Online]. Available: https://www.mckinsey.com/capabilities/operations/our-insights/operations-blog/ops-40-engaging-your-people.

[5] 	H. Krishnan, 2022. [Online]. Available: https://harigurumoorthi.page/articles/a-generic-model-to-define-and-implement-a-practice.

[6] 	E. Xheblati, "Data Executive Playbook," 2021. [Online]. Available: https://www.ergestx.com/data-executive-playbook/.

[7] 	M. Berner and A. Maedche, "The Impact of Process Visibility on Process Performance," 02 2016. [Online]. Available: https://www.researchgate.net/publication/284563165_The_Impact_of_Process_Visibility_on_Process_Performance.

[8] 	joapen, "Dynamics between Team Topologies and Wardley Maps," 2024. [Online]. Available: https://joapen.com/blog/2024/01/18/dynamics-between-team-topologies-and-wardley-maps/.

[9] 	"Creating High Performing Teams," Inflection Point, 23 10 2019. [Online]. Available: https://inflection-point.co.uk/creating-high-performing-teams-case-study/.

[10] 	J.-C. Rodriguez, "7 stunning lessons from how borders group failed," 2022. [Online]. Available: https://www.linkedin.com/pulse/7-stunning-lessons-from-how-borders-group-failed-rodriguez/.

[11] 	"Data Analytics Landscape," [Online]. Available: https://medium.com/@nathanjones_77/mapping-the-data-analytics-landscape-chapter-1-8c5470fa0fdc.

[12] 	T. Milner, "Wardley Mapping the Modern Data Stack," January 2022. [Online]. Available: https://dev.to/aws-builders/wardley-mapping-the-modern-data-stack-1h6g.

[13] 	G. Dobocan, 2020. [Online]. Available: https://medium.com/north-code/tech-fails-bbcs-100m-digital-media-blunder-ca397bb99ecd.

















