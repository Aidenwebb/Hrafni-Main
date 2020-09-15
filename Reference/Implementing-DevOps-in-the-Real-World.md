# Implementing DevOps in the Real World
Study notes from Richard Seroter's course at https://app.pluralsight.com/library/courses/implementing-devops-real-world

## Overview
High performing IT Organisations:
  * 200x more frequent deployments
  * 24x faster recovery from failure
  * 3x lower change failure rate
  * 22% less time on unplanned work
  * 50% less time remediating security issues

Culture is revealed during retrospectives:
  * Not about assigning blame
  * Assemble timeline
  * Use facts to review what happened
  * Explain what worked, what didn't
  * Develop action plan and assign owners
  * Put record into discoverable place

## Who Cares About DevOps?

### Introduction and Overview

### The Business Imperative
> Every industry and company that is not bringing software to the core of their business will be disrupted.
>
> Jeffrey Immelt, CEO of GE

### The Challenge of Becoming Software-driven
  * Lack of trust between IT Teams, management and 3rd parties
  * Oppressive technical debt
  * Lack of automation
  * Competing silo priorities
  * Focus on efficiencies and local optimisation at the cost of flexibility and adaptability
  * Culture doesn't accept risk or change


### Characteristics of High Performing Organisations
> DevOps’s core insight is that reducing the distance between people, teams, and activities, combined with reducing the batch size of your work, allows you to deliver more value, more continuously, with greater quality.
> 
> Jeff Sussna

High performing IT organisations according to Puppet's State of DevOps report (2016):
  * 200x more frequent deployments
  * 24x faster recovery from failure. Cost of downtime is high, so fast recovery makes a huge difference.
  * 3x lower change failure rate. When making a lot of changes in increments, success is higher than completing a large batch of changes at once.
  * 22% less time on unplanned work. Less breakfix / emergency deployments. Often happens when work isn't completed right first time.
  * 50% less time remediating security issues. Often security is bolted on at the end of the project, but with a DevOps mindset, it can be easily built in throughout a project.


### Core DevOps Values and Characteristics
  * **Trust (but verify):** Trust that the team has the skills and will to do a good job. Set up tests, monitoring and alerts to catch problems.
  * **Empowerment:** Empower people to resolve problems and deliver service.
  * **Accountability:** Those who build the service, run the service. Encourages them to build it right the first time as now, when it goes wrong, they're on the hook for support. It's not just thrown over the fence to ops as their problem now.
  * **Continuous Improvement:** Always learning, always getting better. Not about finding perfection, but is about reflecting on the current state and being open to experiment to improve.
  * **Data-driven decisions:** Not simply anecdotal. When changing processes or investigating, use data rather than acting on a whim. Measure things so you have data to back up your choices
  * **Customer Empathy:** Doing what's best and going to improve the experience of the customer and improve things for them.

#### Characteristics of a DevOps Environment
  * **Optimised for throughput:** Change the focus away from optimising a system for accuracy to optimising it to throughput and for value for the customer. It's less about becoming efficient and more about improving the velocity at which value is delivered to a customer. Avoid work in progress being locked behind doors and bottlenecks and focus more on getting it to the customer.
  * **Clear view of the entire deployment pipeline:** When the definition of done is "My step is finished" then products stagnate and frustration is borne when product work has to be passed back to you. When the definition of done is "The product is available to the customer" then not only does everyone in the team deliver value to the customer, but they also work more efficiently in order to get that product in to the hands of the customer. Less thinking about the start and end of a project, and more thinking about the lifecycle of a product or service
  * **Customer-centric definition of "done":** Have you delivered value to the end user? Then you're finished. The team owns and feels responsible for the production of the product and is collecting metrics
  * **Small, frequent software releases:** Smaller debug surface, smaller chance of going wrong. Tests in place to catch errors.
  * **Defined feedback loops:** Powers continuous improvement. Lots of strong and discrete feedback loops. From Customers to Developers, Developers to Ops and everything in between. All groups are able to provide feedback that is consumed and reviewed.
  * **Automation-centric:** It's hard to do DevOps without automation. This is a good way to establish repeatable processes and build trust that you're able to complete tasks in a repeatable fashion
  * **Focused on outcomes, not activities:** What's valuable is the result. The outcomes are typically customer-centric. The input is less important than the value delivered from the outcome.

#### Changes you may see while adopting DevOps
  * **Philosophy Changes:** Do-Adapt model, rather than a Plan-Implement model. No longer assuming that you'll get a masterful product in the first iteration and instead creating working code and adapting it to fit the requirements. Aiming to have release-candidate level code at all times. No longer writing bad code and then integrating it in to releaseable code at the last minute.
  * **Team Changes:** Instead of Project teams where Devs never get feedback about the project once in production and are pulled off once done to focus on another project. Instead you have product teams who build, run and maintain a product.
  * **Tool Changes:** Products with API's that facilitate automation. Likely to use more open source 
  * **Satisfaction Changes:** Both customers and employees are typically happier. The Puppet report shows an increase in satisfaction across the board. From customers all the way through the chain to product owners, management and executives.


### Some Core Objections to DevOps
  * **"We're already doing DevOps. We have a QA and Release Team":** DevOps means a cultural shift in how you think about deliver software. It's not about separating out disciplines. Having a "Devops" team doesn't make you Devops. You're more likely to have a Feature team, Software team and Service team for a product.
  * **"This philosophy doesn't scale to companies of our size":** Not the case. Some of the largest companies in the world are adopting DevOps. 
  * **"We don't have the tech skills that startups do":** "Well we hire those people from you" - It's about investing in your own team. It can't be a grassroots exercise, it often requires some training and nurturing your staff to excel
  * **"Our executives don't think IT has value and is decreasing their IT investment":** This is often from a erosion of trust between IT and Management. You may need to incubate these values around the running of a smaller service and use them to rebuild trust
  * **"Our compliance needs are too complicated for this":** DevOps often increases security profile, you have a better audit trail through version control. Security is built in to the deployment pipeline such as code scans and pentesting.
  * **"My company buys commercial software. We don't build anything":** It's about choosing the right things to build. Many problems don't have existing commercial software to solve them, or if they do it often involves twisting software to work in a way it was never designed to and this can create problems.
  * **"It's just another fad that we can wait out:"** This is unlikely to be the case. DevOps looks set to become the new normal as we become more mobile and integrate with partners differently.

### How Enterprise DevOps Differs from Small DevOps
  * More stakeholders: May need more sign offs and sanctions from the board
  * Functional silo's in place: Some reorganisation may be needed.
  * Existing technical debt to manage: Some systems may not be automation friendly. Data may not be able to changed. You may need to build proxy layers around legacy systems
  * Specific compliance requirements: You don't necessaarily need to use Cloud. 
  * Outsourcing arrangements in place: Remote teams can still work well together.


### Related Books to Read
Added the following to YouTrack backlog.
  * The Phoenix Project - Already Read
  * DevOps Handbook - Currently Reading
  * Starting and Scaling DevOps in the Enterprise
  * Lean Enterprise
  * The Goal
  * Team of Teams
  * American Icon


## Week of DevOps - Mondays

### Holding Organisation and Team Standups

### Assigning an On-Call Engineer

### Planning the Next Software Sprint

### Triaging New Feature Requests

### Merging Code with the Master Branch

## Week of DevOps - Tuesdays

## Week of DevOps - Wednesdays

## Week of DevOps - Thursdays

## Week of DevOps - Fridays