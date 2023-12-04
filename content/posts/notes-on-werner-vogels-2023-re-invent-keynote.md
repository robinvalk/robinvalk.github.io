---
title: "Notes on: AWS re:Invent 2023 - Keynote with Dr. Werner Vogels"
date: 2023-12-04T20:00:00+01:00
draft: true
---

In [AWS re:Invent 2023 - Keynote with Dr. Werner Vogels](https://www.youtube.com/watch?v=UTRBVPvzt9w), Dr. Werner Vogels walked us through the "laws" of [The Frugal Architecture](https://thefrugalarchitect.com/). Ofcourse he couldn't ignore the topic of AI so they focused on that later in the talk. Here are my notes from the keynote. As the AI part didn't give me a lot of takeaways I'm mostly focusing on The Frugal Architecture.

##  The Frugal Architecture

> Simple laws for building cost-aware, sustainable, and modern architectures.

Frugal architecture consists of three main topics: Design, Measure and Optimize. Let's go over them:

### Design

#### 1. Cost needs to be a non-functional requirement

Consider cost from the very beginning of an architecture design. Actually, make it a big part in every step of design. Cost can be seen as a close proxy for sustainability. You want to improve sustainability? Lower the cost.

Cost and sustainability must always be in the list of non-functional requirements. If you build something radically new, you have no idea how exactly your customers are going to use your system and how much resources they will use for each operation. ***Make sure you can react to it.***

#### 2. Systems that Last Align Cost to Business

Find the ***dimension you're going to make money over***, then make sure that the ***architecture follows the money***. Business and technology decisions need to be in harmony to be durable. Use the economies of scale and pay of your debts, both technical and economical debts.

Growth at all costs leads to a trail of destruction.

#### 3. Architecting is always a Series of Trade-offs

Trade-offs always have to be made. Cost, resilience, performance etc. Determine what you are willing to pay, align your priorities. Find the sweet spot between risk tolerance and budget.

### Measure

#### 4. Unobserved Systems Lead to Unknown Costs

Unobservability on costs means they remain invisible which promotes wasteful decisions. Know your costs.

Define your meter and make it visible. Make sure your meter includes costs and sustainability. If you look at a the meter, you'll change your behaviour.

#### 5. Cost Aware Architectures Implement Cost Controls

Decompose applications into tuneable building blocks so you can take actions on opportunities of improvement. Tiering is a common approach, it informs trade offs between costs and other requirements. Determine what needs to work when.

The switches and knobs (cost control) should be in the hands of the business.

> A common approach is tiering components by criticality. Tier 1 components are essential; optimize regardless of cost. Tier 2 components are important but can be temporarily scaled down without major impact. Tier 3 components are “nice-to-have”; make them low-cost and easily controlled.

### Optimise

#### 6. Cost Optimisation is Incremental

Optimisation is not a task you finish ones. Continuously question and optimise your architectures. Eliminate digital waste. Stop, rightsize, shift, reduce workloads.

What may seem as minor optimisations accumulate to large savings at scale.

#### 7. Unchallenged Success Leads to Assumptions

> One of the most dangerous phrases in the English language is: “We’ve always done it this way.”
> - Rear Admiral Grace Hopper

Cost to build is much lower than cost to operate. Disconfirm your own beliefs and put your ego aside. Start thinking about cost and complexity when designing and building. Maybe the massive / complex platform is costing you a lot. Architectures should evolve so they best fit the present requirements.

Constrains often breed creativity, maybe give yourself some constrains.

Learn and be curious.

## AI - key takeaways

### AI predicts, professionals decide

Build small models that target a specific problem that is valuable to the customer. Let the UI predict but let the professionals decide!

Example:
An AI model can alert a doctor about an MRI scan result where it recognised a stroke with high confidence. But the doctor verifies and decides the actions he will take.

### You now have a personal AI assistance who is an AWS expert

With Amazon Q you get all the help to construct an architecture on AWS. It is an interactive process so have a conversation and elaborate.

Amazon Q in combination with Application Composer should make very easy to construct the infrastructure templates and visualise them.
