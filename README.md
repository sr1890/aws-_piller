# Operational excellence:

At Amazon, we define operational excellence as a commitment to build software correctly while consistently delivering a great customer experience. It contains best practices for organizing your team, designing your workload, operating it at scale, and evolving it over time.
Operational excellence helps your team to focus more of their time on building new features that benefit customers, and less time on maintenance and firefighting.

The following are the design principles for operational excellence in the cloud:
        o	Perform operations as code:
        o	Make frequent, small, reversible changes: 
        o	Refine operations procedures frequently:
        o	Anticipate failure: 
        o	Learn from all operational failures: 
        o	Use managed services: 
        o	Implement observability for actionable insights: 

There are four best practice areas for operational excellence in the cloud:
1)	Organization: 
a.	Your teams must have a shared understanding of your entire workload, their role in it, and shared business goals to set the priorities that will achieve business success.
b.	Evaluate internal and external customer needs involving key stakeholders, including business, development, and operations teams, to determine where to focus efforts.
c.	Evaluate threats to the business (for example, business risk and liabilities, and information security threats) and maintain this information in a risk registry.
d.	Verify that there are identified owners for each application, workload, platform, and infrastructure component.
e.	Encourage experimentation to accelerate learning and keep team members interested and engaged. 
f.	If there are external regulatory or compliance requirements that apply to your organization, you should use the resources provided by AWS Cloud Compliance
	a) Organization priorities:
i.	Evaluate external customer needs
ii.	Evaluate internal customer needs
iii.	Evaluate governance requirements
iv.	Evaluate compliance requirements
v.	Evaluate threat landscape
vi.	Evaluate tradeoffs
vii.	Manage benefits and risks
		
	b) Operating model:
a)	Operating model 2 by 2 representations:
a.	Fully separated operating model --> Applications and Platform On the horizontal axis, we have Engineering and Operations.
b.	Separated Application Engineering and Operations (AEO) and Infrastructure Engineering and Operations (IEO) with centralized governance.
c.	Separated AEO and IEO with centralized governance and a service provider.
d.	Separated AEO and IEO with centralized governance and an internal service provider consulting partner.
e.	Separated AEO and IEO with decentralized governance.

b)	Relationships and ownership:
a.	Resources have identified owners
b.	Processes and procedures have identified owners
c.	Operations activities have identified owners responsible for their performance
d.	Team members know what they are responsible for
e.	Mechanisms exist to identify responsibility and ownership
f.	Mechanisms exist to request additions, changes, and exceptions
g.	Responsibilities between teams are predefined or negotiated
	
	c) Organizational culture: 
Provide support for your team members so that they can be more effective in taking action and supporting your business outcome.
a.	Executive Sponsorship
b.	Team members are empowered to take action when outcomes are at risk
c.	Escalation is encouraged.
d.	Communications are timely, clear, and actionable.
e.	Experimentation is encouraged.
f.	Team members are encouraged to maintain and grow their skill sets
g.	Resource teams appropriately
h.	Diverse opinions are encouraged and sought within and across teams




	
2)	Prepare:
	To prepare for operational excellence, you have to understand your workloads and their expected behaviours. You will then be able to design them to provide insight to their status and build the procedures to support them.
Design your workload so that it provides the information necessary for you to understand its internal state (for example, metrics, logs, events, and traces) across all components in support of observability and investigating issues.
Adopt approaches that improve the ﬂow of changes into production and that achieves refactoring, fast feedback on quality, and bug fixing. 
a)	Implement observability:

Implement observability in your workload so that you can understand its state and make data-driven decisions based on business requirements.

i)	Identify key performance indicators:
(i)	Start with business outcomes:
(ii)	Correlate technical metrics with business objectives:
(iii)	Use Amazon CloudWatch:
(iv)	Regularly review and update KPIs: 

ii)	Implement application telemetry:
(i)	Metrics, logs, and traces form the three primary pillars of observability
(ii)	Identify what data to collect:
(iii)	Deploy the CloudWatch agent:
(iv)	Define and monitor business KPIs:
(v)	Instrument your application with AWS X-Ray:
(vi)	Standardize data collection across your application:
iii)	Implement user experience telemetry:
		Gaining deep insights into customer experiences and interactions with your application is crucial. Real user monitoring (RUM) and synthetic transactions serve as powerful tools for this purpose.
Use CloudWatch RUM
iv)	Implement dependency telemetry
		Dependency telemetry is essential for monitoring the health and performance of the external services and components your workload relies on DNS, databases, or third-party APIs
v)	Implement distributed tracing
		
b)	Design for operations:
i)	Use version control
(1)	codecommit
ii)	Test and validate changes
(1)	Codeguru, Codebuild , codepipiline
iii)	Use configuration management systems
(1)	AWS Config 
		
c)	Mitigate deployment risks:
	Adopt approaches that provide fast feedback on quality and provide rapid recovery from changes that do not have desired outcomes. 
i)	Plan for unsuccessful changes
ii)	Document the policies that require teams:
iii)	Analyze the level of impact of all changes related to each component:
iv)	Integrate tools and workflows to enforce your policies programmatically:
	Make data about changes visible to other workload owners to improve the speed of diagnosis:
v)	Test deployments
Test release procedures in pre-production by using the same deployment configuration, security controls, steps, and procedures as in production.
		Use drift detection:
		Use change sets:
	 	Employ safe deployment strategies.
	 	Automate testing and rollback
3)	Operate:
Observability allows you to focus on meaningful data and understand your workload's interactions and output. By concentrating on essential insights and eliminating unnecessary data, you maintain a straightforward approach to understanding workload performance. It's essential not only to collect data but also to interpret it correctly.
With observability, you're better equipped to foresee and address potential challenges, ensuring that your workload operates smoothly and meets business needs.
		
	a) Utilizing workload observability:
			Analyze workload metrics
			Analyze workload logs
			Analyze workload traces
			Create actionable alerts
			Create dashboards
			
	b) Understanding operational health:
	c) Responding to events:

4)	Evolve

•	Learn, share, and continuously improve to sustain operational excellence. Dedicate work cycles to making nearly continuous incremental improvements.
•	Perform post-incident analysis of all customer impacting events.
•	Regularly evaluate and prioritize opportunities for improvement 
•	Include feedback loops within your procedures to rapidly identify areas for improvement and capture learnings from running operations.
•	Share lessons learned across teams to share the benefits of those lessons. 
