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

1. [INPUT] **User query**: User gives a core idea, a problem to solve or just give a specific library or API to use or literally anything
2. [PROCESS] **User query enrichment**: Perform a configurable amount of web searches and gather additional context relevant to user query.
   1. Do a web search on:
      1. Existing Product, service or feature
      2. Competitors
      3. Market trend
      4. Society trend
      5. Technology trend
3. [OPTIONAL INPUT] While web search is running, ask user to provide additional context regarding these aspects if he/she has not provided in the initial query 
4. [PROCESS] **Prioritizing the High-level Product Goal**: Given the additional context, the next step is to help the user prioritize a high-level product objective. External context is often incomplete, critical insights typically emerge through direct collaboration with stakeholders. Despite this uncertainty, the approach must remain strategic. You should clearly justify why each product goal is relevant and worth solving given the available context and give your opinion on which Product goal should be pursued. However, the user should have the final say in selecting which goal to pursue. Consider the following high-level product goals:
 	1. User Acquisition: Bring more users into the product
  	2. Activation: Reduce time-to-value by enabling users to reach the product’s core value as quickly as possible.
	3. Engagement: Drive deeper and more frequent interactions that reflect meaningful product usage
	4. Monetization Strategy: Capture value by translating user engagement into sustainable revenue streams.
	5. Product Quality: Deliver a consistently reliable, high-quality experience that meets user expectations
	6. Funnel smoothness: Minimize friction and drop-offs across user journey stages

5. [PROCESS] **User Empathy** You can start empathizing with user now. Come up with:
 	1. User persona
    2. User journey based on their persona
	3. Derive specific **User pain** points based on the journey
	4. Prioritize a user pain point to solve based on its
		1. Severity (how painful the problem is in terms of time or money)
  		2. Frequency (how often the problem surfaces)
		3. Reach (how many people the problem affects)
Re-define the Product Goal
Reframe the prioritized Pain Point
Define the Northstar Metric
A/B Testing strategy (how do we know if the feature is working)
Software System Design and Data 
Given the Re-defined Product Goal, come up with 3 features to build. Think creatively here. For each feature come up with the following:
Functional requirements
Non-functional requirements
Dashboard to monitor KPIs and enable decision-making regarding the feature 
