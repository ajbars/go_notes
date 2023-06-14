Microsoft Devops Challenge Lessons

1. OODA loop: observe, orient, decide, act. This was invented to keep fighter pilots from being shot out of the sky

Observe business, market, needs, current user behaviour and telemetry data
Orient with the enumeration of options for what you can deliver, perhaps with experiments
Decide what to pursue
Act by delivering working software to users

Become data informed - use data to inform what to do in next cycle
1/3 of deployments bring negative results, 1/3 neutral and 1/3 good. Double down on good, fail fast on the ones that don't advance the business. 'Pivot or persevere' approach.

Shorten your cycle time
You shorten your cycle time by working in smaller batches
Using more automation
Hardening your release pipeline
Improving your telemetry
Deploying more frequently

More frequent deployment = more experimenting. This acceleration in validated learning is the value of the improvement. 

The goal is to shorten the cycle. Start with the release pipeline. How long does it take to deploy a line of code? That is a brake on your velocity.
Continuous integration drives the ongoing merging and testing of code, leading to an early finding of defects + less time fighting merge issues and rapid feedback for devs.
Continuous Delivery of software solutions to prod and test environments helps quickly fix bugs and respond to changing business requirements
Integrate Version Control with software development tools for monitoring deployments
A Devops Definition of Done is a working software collecting telemetry againts the intended business goals
Monitoring and logging of running applications. Helps create a hypothesis and quickly validate/disprove strategies

DevOps may hurt at first. If it hurts, do it more often
Cross-train to develop synergy


Explore shared goals
Goals should include numbers
Reduce the time spent on fixing bugs by 60%
Reduce the time spent on unplanned work by 70%
Reduce the out-of-hours work required by staff to no more than 10% working time
Define timelines for goals
Have an ongoing series of short-time goals
Every few weeks improvements should be clear and measurable
Short plans allow: 
easier changing of plans/priorities
reduced delay between work and feedback
easier to keep organizational support

How to apply DevOps practises to minimize initial resistance

Greenfield and brownfield projects
Greenfield is previously undeveloped project. Brownfield relates to the one that was used before. Common misconception is that DevOps can only serve and succeed in greenfield projects.
In brownfield there is usually a large gap between client expectations and reality.
The team has already lived the challenges and drawbacks of what they are currently doing.

Greenfield give more possibilities, avoid politics, avoid buiseness practices that don't align with your plans
Brownfield ones have baggage, have existing teams, have significant technical debt
Brownfield spend a lot of effort maintaining and not developing code
Management see the potential benefits better, have sense of urgency

Systems of record versus systems of engagement

SOR provide the truth about data elements. They've evolved slowly and carefully. Bank systems. Emphasize accuracy and security.
SOE are more exploratory. Use experimentation to solve new problems. Are modified regularly. Quick is priority over correct.
There is a perception that DevOps suits SOE better, however that is not correct. Sometimes the necessity of doing things correct is an excuse for not implementing DevOps practises. 
It's easier to start with SOE when first starting DevOps transformation.
But the most significant outcomes often come from transforming SOR.

Identify groups to minimize initial resistance

Canary users
voluntarily test bleeding edge features once they are available
Early adopters 
voluntarily preview releases, more refined than previous group
Users,
who consume the product after it was tested by two previous groups
Find staff members keen to see new features as soon as they are available and are highly tolerant of issues
EA are similar to the Canaries. Often have work requirements that make them less tolerant of issues and interruptions to work
Development and IT operation staff can be less conservative than users

Ideal target improvements

It's also important to roll out changes incrementally. Any successful large IT system was initially a successful small system.
Large systems rolled out at once have abysmal success record. Most fail no matter support from the management.
Find the improvement that:
Can be used to gain early wins
Is small enough to be achievable in a reasonable timeframe
Has significant and evident benefits to the organization
The aim is to build a snowball effect where any success adds to the previous ones. It will maximize a buy-in from all involved.

Project metrics and KPIs

The common ones are:

Faster outcomes:
Deployment frequency - increased
Deployment speed - reduce the time that deployments take
Deployment size - how many features, stories and bug fixes are being deployed each time
Lead time - how long from the creation till the completion

Efficiency:
Server to admin ratio: are the projects reducing the number of required admins for a given number of servers?
Staff member to customer ratio: is it possible for fewer staff members to serve given number of customers?
Application usage: how busy is the application?
Application performance: Is improving or dropping? Metrics-based

Quality and security:
Deployment failure rates - how often do deployments or apps fail?
Application failure rates - how often do app failure occur, config failures, performance timeouts etc
Mean time to recover - how long it takes to recover from the fail?
Bug report rates - is the amount customers see increasing or decreasing
Test pass rates - how well is automated testing working?
Defect escape rate - what percentage of defects are being found in production?
Availability - what percentage of time the app is truly available for customers?
Service level agreement achievement - are you meeting SLAs?
Mean time to detection - if there is a failure, how long it takes to be detected?

Culture:
Employee morale: are employers happy with the transformation and where the organization is heading? By anonimous surveys
Retention rates: is the organization losing staff?

