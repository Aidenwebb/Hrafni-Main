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
Inform people about milestones/blockers etc.
  * What is it? Org / Team Standup
  * Who is involved? Team members, interested parties
  * Why does this belong in DevOps? Transparency, throughput, delivery focus

Why a Daily Standup Matters:
  * Orient everyone
  * Draw attention to important information. Request for pairs, important issues, important customers to support etc
  * Come together to remove blockers. Figure out what the block is and get help rather than moving on to the next item
  * Facilitate continuous improvement

Tips for getting started
  * Set up a shared calendar with milestones
  * Keep brief, avoid status updates. Have someone keep track of time. Aim for 3-5 minutes total
  * Don't force everyone to speak
  * Set an example that asking for help is ok


### Assigning an On-Call Engineer
Someone needs to be responsible for end-user support throughout the week
  * What is it? Assign on-call engineer.
  * Who is involved? Rotating person on the application team
  * Why does it belong in DevOps? Develops empathy, focus on the customer

On-Call Engineer leads to better code and focus
  * Puts the focus on the customer and the service
  * Encourages code instrumentation, improvement. You end up building better logging, metrics and error reporting as you have to live with the architectural and coding decisions made.
  * Helps other team members stay focused. Stops context switching between dev and support
  * Record of experiences help the team

Tips for getting started
  * Sign up for a pager service. For a clear notification when things go wrong
  * Make it easy to find who is on-call for each team
  * Do dry-run exercises to flex and test the process. Encourage improvements, understand escalations, deployments etc
  * Add an "executive on-call" to the rotation. Helps Executives remove blockers, prioritise and empathise with both customers and teams


### Planning the Next Software Sprint
  * What is it? Plan the next sprint
  * Who is involved? Whole application team including the product owner
  * Why does it belong in DevOps? Focus on small batches, delivery pipeline

Key Part of DevOps is the Spring Approach
  * Product owner maintains a backlog and decides what work is in the sprint
  * Start meeting with a retrospective. Rewind and figure out how the last sprint went. Address issues and continually improve
  * Team decides amount of work in the sprint. Team will typically understand how much work they're capable of and their velocity and scope.
  * Sprint scope doesn't change. It's one way only. No scope creep, no new stories, typically no emergencies that cause everyone to drop work. Reduce sprint length. 1,2 or 4 weeks.
  * Team always ships at the end of a sprint. Keeps a sense of urgency and forces to wrap things up.
  * Sprint window should keep shrinking. It's about small batches and shrinking helps to highlight inefficiencies. 2 weeks testing might work in a 6 month sprint, but in a 3 week sprint, 2 weeks of testing is clearly ridiculous.

Tips for getting started
  * Designate a product owner. Not shared, dedicated and responsible solely for that product and is a facilitator with stakeholder. Product owner prioritises and understands the life of the products
  * Begin with one month sprints. Too long and it's easy to let stuff slide. Too short and you'll find it hard to get anything done.
  * Don't use planning session to design software. More requriement sessions and planning sessions before the sprint planning sessions. Sprint planning should be about ingesting the work and deciding on level of effort for each item in the sprint
  * If adding work from the sprint, subtract work from the sprint. Teams have a finite capacity, and adding new work without adding new resource erodes trust, increases stress and results in work not being completed.
  * Change process regularly to improve. Figure out new ways to measure velocity, understand item work etc.

### Triaging New Feature Requests
  * What is it? Triage new feature requests. Review requests and bugs raised by the customer
  * Who is involved? Product owner, stakeholders. 
  * Why does it belong in DevOps? Continual improvement, customer focus.

Do Realistic reviews of New Requests
  * Review all software requests regularly. Feedback to customers. Reject or Accept requests
  * Cross functional participation. Gain perspectives from multiple different teams. Things that are not important to one group, may be critical to another. A seemingly non important bug may be flagged by the support team as very important to the customer
  * Immediately adjust backlog priorities

Tips for Getting Started
  * Triage features AND bugs in this meeting. One methodology is bug fixes happen either in the current sprint, the next sprint, or are dropped until they reappear to avoid an enormous backlog of issues and bugs overburdening the team. It's important to make time for bugs in the sprint else they can become invisible and untracked work.
  * Support team and on-call engineers attend. Other teams can also attend. Voice of stakeholders is important
  * Reject the majority of requests. Not because they're not great ideas, but because there is a finite capacity and backlogging too many requests reduces the velocity at which an exceptional idea can make it to production.
  * Product owner retires old backlog items. One methodology is to keep under 100 items in the backlog at any one time. Backlog should be things that you can complete within the next 6 months.

### Merging Code with the Master Branch
  * What is it? Merge code with the master branch
  * Who is involved? All engineers
  * Why does it belong in DevOps? Small batches, limiting work in progress, keeping code production quality at all times

Continuous Integration Drives Confidence
Extended, multi-month integration periods can be exhausing, especially due to a lack of testing, and trying to glue code together
  * Test coverage is key to trusting automation. 
  * Fast feedback reduces wasted time later on. The purpose of automated testing is not to reduce the cost of testing, but to allow tests to be run on a more frequent basis to provide feedback to developers to reduce waste in new work.
  * Frequent tests mean a smaller debugging surface. Smaller releases mean less work to review to hunt down a bug.
  * Aim for green builds, but don't fear red. Red means your tests are working. If red, everyone should feel confident in what they need to do, check and review to get a green build

Tips for Getting Started
  * Source control repository is a must have. 
  * Get visual indicators of build status. Lamps or similar. Red lamps being broken build, Green being successful build. Pipelines on monitors etc.
  * Avoid long-lived feature branches. Consensus is typically that branches are a contributor to waste. The longer a branch is worked on, the harder it is to integrate back in to main when complete.
  * Make working code a forcing function
  



## Week of DevOps - Tuesdays

  * What is it? 
  * Who is involved?
  * Why does it belong in DevOps?

## Week of DevOps - Wednesdays

## Week of DevOps - Thursdays

## Week of DevOps - Fridays