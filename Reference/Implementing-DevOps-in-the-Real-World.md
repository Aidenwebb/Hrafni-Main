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

### Holding Team Standups Handling Support Tickets
  * What is it? Org / Team Standup
  * Who is involved? Stakeholders, Team members, interested parties
  * Why does it belong in DevOps? Transparency, throughput, delivery focus

### Handling Support Tickets
  * What is it? Handle support tickets. End users raise issues about functionality, performance and defects. May be handled by a frontline support team, but routes to the team that owns the service.
  * Who is involved? On-Call engineers, front-line support
  * Why does it belong in DevOps? Responsiveness and accountability

Team closest to code handles tickets
  * Primary responsibility of on-call engineer that week
  * Using same ticketing system as support personnel. Avoid transfer waste
  * May become a group effort to resolve.
  * Sparks new ideas for new features to propose

Tips for Getting Started
  * Consolidate unique ticketing systems. Having separate ticketing systems means loss of information and transfer waste. It also means that whne it's resolved, you need to remember to close the ticket across multiple systems.
  * Don't assign on-call engineer additional work
  * Have test-bed ready to reproduce issues
  * Avoid handing over tickets to the next On-Call
  * Maintain good ticket hygiene


### Patching Infrastructure
  * What is it? Patch server clusters
  * Who is involved? Engineers on the application team, sometimes the On-Call Engineer
  * Why does it belong in DevOps? Consistency, Responsiveness, Security

Make Patching Routine, Uneventful
  * Upgrades required up and down stack
  * Infrastructure as Code. Treat infrastructure as another configuration, create it through automation without human interaction
  * Multiple possible approaches. Could patch with Config Management software. Could create new images/containers and replace existing ones. (Immutable Server)
  * Consistently applied to each environment

Tips for Getting Started
  * Do integration testing with infrastructure
  * Define a policy to never log in to servers. Avoid touching production servers manually
  * Introduce config management everywhere first
  * Aim for immutable infrastructure over time

### Pairing on Infrastructure-Centric Feature
  * What is it? Pair on Infrastructure Feature
  * Who is involved? Engineers on the application team
  * Why does it belong in DevOps? Cross Training, collaboration. Builds a better relationship between Infrastructure and Developer teams

Infrastructure is Code Too!
  * Hire generalists with specialities
  * All configuration details are in source control
  * Test rigorously in production-like environment

Tips for Getting Started
  * Make infrastructure work visible. Put stories on the backlog for requirements, automations etc.
  * Pair Ops engineers with software engineers. Build comradery and break down barries
  * Test infrastructure just like software

### Detecting and Handling a Service Interruption
  * What is it? Detect service interruption
  * Who is involved? Support staff, on-call engineer, potentially the whole team
  * Why does it belong in DevOps? Responsiveness, accountability

Disciplined Approach to Problem Solving
  * Upfront instrumentation pays off. Collect metrics and act on patterns
  * Use facts to figure out causation. Mean time to recovery is faster when you have good telemetery 
  * Communication is key. Collect a timeline of events, communicate that things are down. It's not fun, but it's much worse when customers are surprised by an outage and can't find information
  * Over-alerting causes fatigue. Alert only on actionable, high urgency items.

Tips for Getting Started
  * Identify core metrics that measure availability
  * Add tech for inside-out and outside-in tests. Add instrumentation to detect incidents that were previously user reported and not detected by tests
  * Make dashboards visible, proactive
  * Have a unified way to communicate status. This could be a chat channel internally, or a public status site. Don't have different stakeholders randomly calling team members.

### Sending Status Updates to Executive Stakeholders
  * What is it? Send status update to executives. Prove that things are working
  * Who is involved? Team Leaders
  * Why does it belong in DevOps? Transparency and Trust

Communicate and Iterate
  * DevOps is a cultural change, and requires transparency
  * Share core *business* metrics. Show how this is delivering value. Also show priorities, risks and technical information
  * Build momentum through demonstrated progress. This could be politically sensitive, could be upending a project management team or office who no longer get to deliver big releases.

Tips for Getting Started
  * Choose handful of core metrics to share. Focus on business statistics, release highlights, revenue, adoption statistics etc.
  * Maintain regular rhythm. Send it out at the same time each week/month. Actively push the information out, if it's ignored, that's their choice
  * Show good AND bad news to build trust. Don't just show green dashboards all day every day even if things are wrong. 
  * Keep refining based on feedback. Ask stakeholders what matters to them. Update metrics, format and audience

## Week of DevOps - Wednesdays

### Holding Team Standups
  * What is it? Org / Team Standup
  * Who is involved? Team Members, Interested Parties
  * Why it belongs in DevOps? Transparency, throughput, delivery focus

### Onboarding New Engineers
  * What is it? Onboard New Engineer. Could be a constant rotation within the team
  * Who is involved? Application team
  * Why it belongs in DevOps? Cross-training, customer focus

It's About Speed to Productivity
The faster a new employee is able to be productive, the faster a company sees value and the faster the new employee feels satisfied with their new role
  * Learn from source control, deployment, pipeline, wiki. Avoid having undocumented tribal knowledge within the team as this is a barrier to understanding and a barrier to productivity
  * Good opportunity to test deployment pipeline. See how a new participant works with the tools
  * Pairing accelerates readiness. New hires should pair with someone experienced and can contribute quickly.

Tips for Getting Started
  * New team members pair with existing ones. Not at random, consider who on the team are good coaches. Let them know ahead of time so they can plan their time
  * Encourage use of application itself
  * Add to the On-Call rotation quickly. Preferably within 6 weeks. A good crashcourse in to understanding the application.
  * Iterate onboarding docs based on feedback. Were there common or repeat questions that could be useful to add? Perhaps ask the new member to update documentation themselves as they have fresh eyes

### Attending a Monthly Operations Review
  * What is it? Attend monthly operations review
  * Who is involved? Application Team Leaders, Executives
  * Why it belongs in DevOps? Customer focus, continuous improvement

Accountability Breeds Focus
  * Remain focused on customer metrics. User adoption trends, account closures, abandoned carts etc
  * Leverage collective knowledge. Team is getting together to learn from eachother. Avoid local optimisations screwing up global concerns
  * Improves situational awareness for executives. Give an active view of the data so they can check in at any time without disrupting work.
  * Not a problem solving session. This is to communicate status, not solve problems
  
Tips for Getting Started
  * Ensure each app team defines success
  * Schedule a monthly review
  * Lead by example and mention challenges. Don't just show green and hide problems
  * Actively follow up on problem areas


### Conducting an Incident Retrospective / Postmortem
  * What is it? Conduct incicent retrospective / postmortem
  * Who is involved? On-Call Engineer, Stakeholders
  * Why it belongs in DevOps? Continuous Improvement, Transparency. Improve the service, you're not trying to find someone to blame

Culture is Revealed During Retrospectives
  * Not about assigning blame. Look for ways to redesign the system to prevent future accidents. 
  * Assemble a timeline of things that happened and when.
  * Use facts to review what happened. Avoid revisionist history (Oh we'd just done this we'd be fine). Focus on what happened and when and aim for constructive teamwork addressing faults in process
  * Explain what worked, what didn't. Brainstorm at the start of the session.
  * Develop action plan and assign owners. Don't just gather, throw around some ideas and leave, it's a waste of time. Instead, everything that didn't work well should be on an action plan at the end. Could be adding high availability, improving documentation or other such actions.
  * Put record into a discoverable place, as publically as possible. Show what happened, this is what happened, and this is what we're doing to fix this.

Tips for Getting Started
  * Set up a retrospective the day after the next incident
  * Choose an interface for collecting feedback where people can list what worked, what didn't, and creating action plans
  * Define crisp action items. Prevent errors from reoccurring. Create countermeasures and guard rails
  * Assign someone to keep and share minutes of the meeting


### Collaborating Across Teams
  * What is it? Collaborate Across Teams
  * Who is involved? Application Team Leads, Engineers
  * Why it belongs in DevOps? Remove bottlenecks, Improve Flow. Find things that are preventing the customer seeing the value you're developing and remove them

Collaboration In, and Across, Teams
  * No team should be entirely independent
  * Think locally, act globally. Purely local optimisation will impact and potentially damage the organisation as a whole. 
  * Create system for quick collaboration and decision making. Whiteboards, informal ways to solve the problem and keep going. 

Tips for Getting Started
  * Invest in chat room technology
  * Set up loose boundaries and guidance for commonalities
  * Foster cross-team communication through hackathons

## Week of DevOps - Thursdays

### Holding Team Standups
  * What is it? Org / Team Standup
  * Who is involved? Team Members, Interested Parties
  * Why it belongs in DevOps? Transparency, throughput, delivery focus

### Replacing a Team Process
  * What is it? Replace team process following Retrospective
  * Who is involved? Team Leaders, Team Members
  * Why it belongs in DevOps? Continuous Improvement

DevOps Is About Improving Flow
  * Hard to improve what you're not measuring. You can't say "This should be faster" if you don't know what "normal" looks like.
  * Act on broken processes, bottlenecks and links. Start with a bottleneck and fix it. The strength of a chain is dependent on its weakest leak.
  * Automation is often, but not always, the answer. Sometimes it's about training or communication.
  * Experiment and measure. Small batches and continuous improvement are important so you're able to try new things. 

Tips for Getting Started
  * Solicit feedback from the entire team. 
  * Listen to calls to stop at "good enough". You might never get to perfect, but over-optimisation at an area that is not the bottleneck is a waste.
  * Only buy products / services with APIs. This will allow you to develop middleware, integrations and automations.
  * Evangelise to other teams

### Creating Product Documentation
  * What is it? Write knowledge base articles, release notes
  * Who is involved? Application Team, Documentation Team, Others in Company
  * Why it belongs in DevOps? Knowledge sharing, throughput. People can't use things they don't know about. Help people stay well informed.

Faster Delivery Means More Frequent Explainations
  * As velocity increases, harder for users to track changes.
  * Content must be easy to create, edit and find. Most places don't have a document writing team. Most companies will need to collaboratively build documentation.
  * Change log and broadcast engine are important. Version control is important in documentation management too! 

Tips for Getting Started
  * Set up an open content system
  * Still have "owners" but many contributors
  * Define a light review process - pull requests work well!
  * Open up to those outside the team

### Upgrading the Deployment Pipeline
  * What is it? Upgrade deployment pipeline
  * Who is involved? Application team
  * Why it belongs in DevOps? Increased automation

Deployment Pipelines grow into a System of Record
  * Build a better audit trail over time. It's easy to audit the whole thing rather than a number of samples. Everything from patching code, to updating servers, to deployment history is in the pipeline history
  * First CI / CD attempt may be lightweight
  * Partner with groups like InfoSec and Compliance
  * Cross functional skills come in handy

Tips for Getting Started
  * Do value stream mapping with cross-functional team
  * Test changes repeatedly in non-production environments
  * Use or create API's to integrate with existing audit-visible systems
  * 
### Right-sizing the Team Roster
  * What is it? Right-size team rosters
  * Who is involved? Executives and Team Leaders
  * Why it belongs in DevOps? Responsiveness. React and change according to business needs.

Fluid Teams support Adaptable Strategies
  * Application teams aren't of fixed size. Funding a project and an operational team is a different mindset to funding a product team
  * Engineer count may swell during key periods, and contract after. This needs to be structured and planned, else adding people can slow down velocity.
  * Rotate operations, security expertise throughout. This allows key expertise and input from multiple teams and helps build trust
  * Offers maximum flexibility to respond to changing business needs. It's an engine for delivery services and value to end users and customers. It drives innovation and you need to be responsive and adaptive to the needs of the business.

Tips for Getting Started
  * Create culture of rotating opportunities. This needs to feel natural and positive, not a punishment
  * Use data to make decisions. Consider veloicity per engineer per team, introduce members in a structured manor
  * Avoid over-adjusting. Don't do this every week. Do it at most quarterly
  * Define tech standards that reduce transition time for engineers.

## Week of DevOps - Fridays
###
  * What is it?
  * Who is involved?
  * Why it belongs in DevOps?

Tips for Getting Started