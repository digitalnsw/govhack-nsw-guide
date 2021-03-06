---
layout: sidenav
breadcrumb: Background
name: Background
---

# Rules as code: Improving public access to the rules of government
### Written by Asghar Kazi

*This blog post talks about the possibilities if legislation and other rules of government were available as code. It has been written to not only convey what a transformative idea rules as code is, but will also cover some of the updates from the Rules as Code work that our team has been doing under the leadership of our Executive Director, Pia Andrews in the Department of Customer Service.*

## Context

A few months ago, a friend, who happens to be an international student in Sydney, contacted me to discuss a predicament he was in: he had been getting underpaid since the past two years despite repeated requests to his employer. I accompanied him to attend consultations at a local community legal centre that provides free legal advice. The lawyer at the legal centre asked us to provide him with a list of my friend’s working hours over the past two years and try to calculate how much amount he had been underpaid. We set about setting up an excel spreadsheet and looked at the relevant award of the industry in which he worked in. We started looking at rules specific to rostering, public holidays, breaks between shifts, consecutive shifts and translating these rules into formulas, in order to calculate the rate at which he should have been paid. 

What really baffled us was how difficult it was to translate the rules from the award into formulas on a spreadsheet. After spending more than thirty hours making the spreadsheet, we still had not unpacked all the conditions in the award. 

At about the same time, I had joined the Rules as Code team within the Digital Government Policy Innovation branch (and now within the Data Insights and Transformation branch) to work on a project titled “Rules as Code”. Rules as Code is, among other things, an approach to democratize access to government rules like regulation, legislation or operational rules that are often coded as business rules in siloed systems. These rules may affect any public system (think government use of rules for service delivery, regulating, auditing, calculating or integrating rules of other agencies) or private system (think private organisations whose systems depend on government rules). The Rules as Code project not only makes the rules (and any amendments to the rules) instantly available for anyone to build public facing services on them, it also unlocks value and creates avenues for entirely new RegTech business and public service models to be built on top of these rules. It is an idea that is gathering momentum within Australia, and just a few days ago, the Prime Minister of Australia publicly discussed the idea of legislation written in code.

I will link the situation that my friend was in, to the rules as code project, by a summary: Our current rules, laws and policies were built for an analog and siloed world and hence are cumbersome, hard to translate, comprehend and link to. In order to be a truly open digital government, it is time to re-draft them in code and legalese with policy drafters, legal experts and programmers in the same room and make the code open source. This means not just translating rules into code, but drafting new and existing rules differently from a digital perspective. The NSW Government has already embarked on this journey and I am proud to be a small part of it. 

## The journey so far
There are many “rules as code” projects that simply translate rules into code, but the key differences of our work is twofold:

1.	Better Rules: that we are trying to change how rules are drafted in the first place to be better. If you bring toether policy makers, drafters and developers, you can co-design the business logic, expected outcomes and truly test-driven rules, drafted as human and machine readable from the start.
2.	Government as a Platform: if the rules governments are responsible for were publicly available from government, people could set up their business systems to consume and interact with the rules rather than copying and pasting or having to hard code them in systems across the economy, dramatically improving consistency and speed of application.

So what have we worked on so far, as part of the Rules as Code project within the NSW Government? We’ve workshopped with policy owners to understand legislative context and history, arrived at singular definitions of concepts mentioned in rules, developed logical constructs and entities which can then be represented in code, and mapped out formulas to represent logical conditions within the legislation. More specifically, we have worked on the rules and policies mentioned below, noting that the rules we have coded so far are not authoritative in any shape or form, not endorsed or being presented as the law, and still in experimental stages: 

1.	Cost of Living: We examined various rebates related to cost of living. At the moment, Service NSW asks users a set of five questions and provides them with a list of what rebates the users “might” be eligible for. But by using Openfisca, we can actually create a dynamic series of questions (both internally and externally facing) which update based on additions to the list of rebates/policies related to cost of living. A proof of concept related to this was demonstrated at one of our showcases, earlier this year.

2.	Community Gaming Regulation: We’ve examined the Community Gaming Regulation 2019, abstracted logical concepts from it and coded the eligibility conditions for whether a charity/not-for-profit/business can run a community game for raising funds or promoting a trade (based on conditions such as the total value of prize money, individual prize money, etc.) This is still a work in progress with the policy owner (Better Regulation Division) and we recently had a Concept Modelling session with them.

3.	NABERS Energy Savings calculator: We’ve worked with the Office of Environment and Heritage on coding conditions for whether organisations are eligible for generating energy savings certificates (ESCs) by coding a small part of the Energy Savings Scheme Rules into OpenFisca.

## The rationale behind using OpenFisca: 
We’ve used OpenFisca (developed by the French Government for their rules as code using the python numpy package), which is an open source rules engine, to store our rules. By using OpenFisca, we have made our rules and policies open source in order for other agencies and third party organisations to refer to a single source of truth. This can be helpful in various situations. For example, if there is a change in the rate of a tax, then this can be updated by the policy owner within Openfisca, and would automatically reflect in the linked systems that connect to it (through the Openfisca API). In particular,what is really powerful about Openfisca is that it is not just a place to store all your rules, but it also has the functionality of running simulations and might be useful if you are modelling various scenarios related to testing the outcomes of various policies. For example, in the case of payroll tax, if the rules are modelled correctly and we have good quality data that has a 1:1 relationship with the coded rules, then various simulations can be analysed (by feeding csv files into the Openfisca SimulationBuilder). We have not done this yet while coding any of the rules, but it is definitely something that would really be worth exploring.

Most of this work has also involved the Rules as code team coding specific rules into OpenFisca after sitting with the policy owners through multiple requirement gathering sessions. But the really interesting bit would be when policy owners, drafters, legislative experts and programmers sit together in a room to co-draft and test any new policy and legislation that is not only human and machine consumable, but co-draft better rules for an increasingly digital world. These rules could then also be simultaneously tested against various scenarios to cover edge cases, which may be missed out when the process is done conventionally. The most exciting part about rules as code is yet to come.

## Get in touch with us: 
We want this process to be as collaborative as possible, and we’re still in an early experimental stage. If you think we’d benefit from talking to you, or if you have any suggestions, please get in touch at cs.transformation@customerservice.nsw.gov.au  

