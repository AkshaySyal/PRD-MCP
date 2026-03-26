# PRD-MCP
Fixing bad Plan mode of coding agents

UX / Design Requirements (Define user experience expectations)
Wireframes / mock descriptions [My final deliverable could be a figma doc. I would rather give a figma than a ppt or just words if the product does not work]
Interaction patterns
Error states
Accessibility considerations
Technical Considerations (Align with engineering early [in my case, it is the coding agent])
Architecture overview
Dependencies (APIs, models, infra)
Constraints
Tradeoffs
Risks & Mitigations (Show you’ve thought ahead)
Product risks
Technical risks
Data risks
Mitigation strategies

—————————————————————————————————————————

UPDATED PRD FLOW (thinking about Inputs, Process, Outputs structured according to Flow)

FLOW

1. [INPUT] User query: User gives a core idea, a problem to solve or just give a specific library or API to use or literally anything
2. [PROCESS] User query enrichment: Perform a configurable amount of web searches and gather additional context relevant to user query.
   1. Do a web search on:
      1. Existing Product, service or feature
      2. Competitors
      3. Market trend
      4. Society trend
      5. Technology trend
3. [OPTIONAL INPUT] While web search is running, ask user to provide additional context regarding these aspects if he/she has not provided in the initial query 
4. [PROCESS] User Empathy: Given additional context you can start **Empathizing** with the user. You need to think about these high level product goals:
 	1. User Lifecycle (sequence of stages a user goes through in your product)
    	1. Acquisition: Bringing users into the product
     	2. Activation: The moment a new user experiences the core value of the product for the first time
	   	3. Engagement: How actively users use your product
		4. Monetization: how the product converts user value into revenue
	2. User Experience
		1. Product Quality: how good, reliable, and satisfying the product experience is for users
		2. Funnel smoothness: how users move step-by-step through the product lifecycle <br>
	The goal is to prioritize a high-level product objective based on the enriched user query. External context alone is often incomplete; critical insights typically emerge through 	direct collaboration with stakeholders. Despite this uncertainty, the decision-making process must remain strategic. It is essential to clearly justify why the chosen product 		goal is relevant and worth solving given the available context.We can start empathizing with user now
Come up with User persona
Come up with User journey based on their persona
Derive specific User pain points based on the journey
Prioritize a user pain point to solve based on its
Severity (how painful the problem is in terms of time or money)
Frequency (how often the problem surfaces)
Reach (how many people the problem affects)
Re-define the Product Goal
Reframe the prioritized Pain Point
Define the Northstar Metric
A/B Testing strategy (how do we know if the feature is working)
Software System Design and Data 
Given the Re-defined Product Goal, come up with 3 features to build. Think creatively here. For each feature come up with the following:
Functional requirements
Non-functional requirements
Dashboard to monitor KPIs and enable decision-making regarding the feature 
