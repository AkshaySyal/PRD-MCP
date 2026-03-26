# PRD-MCP
Fixing bad Plan mode of coding agents

[Key Behavior] (important constraint across ALL steps)
At every step, the system must:
1. Incorporate user-provided ideas
2. Avoid contradicting them unless explicitly necessary
3. Clearly indicate when it is:
	1. Using user-provided context
	2. Extending beyond it

UPDATED PRD FLOW (thinking about Inputs, Process, Outputs structured according to Flow)

1. [INPUT] **User query**: User gives a core idea, a problem to solve or just give a specific library or API to use or literally anything
2. [PROCESS] **User query enrichment**: Perform a configurable amount of web searches and gather additional context relevant to user query.
   1. Do a web search on:
      1. Market trend (Existing similar Product or Service, Competitors)
      2. Societal trend
      3. Technology trend
3. [OPTIONAL INPUT] While web search is running, ask user to provide additional context regarding these aspects if he/she has not provided in the initial query 
4. [PROCESS] **Prioritizing the High-level Product Goal**: Given the additional context, the next step is to identify and prioritize a high-level product objective. The user query may already indicate a preferred goal; this should be explicitly extracted and treated as a primary signal. External context can be used to validate, refine, or expand this understanding, but not override it. Since external context is often incomplete and deeper insights typically emerge through direct stakeholder collaboration, the approach must remain strategic. You should clearly justify why each product goal is relevant given both the user-provided input and the enriched context, and provide a recommendation on which goal to pursue. Ultimately, the user retains the final decision on which product goal to prioritize.
 	1. User Acquisition: Bring more users into the product
  	2. Activation: Reduce time-to-value by enabling users to reach the product’s core value as quickly as possible.
	3. Engagement: Drive deeper and more frequent interactions that reflect meaningful product usage
	4. Monetization Strategy: Capture value by translating user engagement into sustainable revenue streams.
	5. Product Quality: Deliver a consistently reliable, high-quality experience that meets user expectations
	6. Funnel smoothness: Minimize friction and drop-offs across user journey stages in the existing product or service
5. [INPUT] Ask user explicitly the final product goal to pursue
6. [PROCESS] **User Empathy** You can start empathizing with user now:
 	1. Generate User Segments & Personas: Identify 3 user segments based on the enriched query and product context. Define a concise persona for each segment (goals, behavior, constraints)
    2. Parallel User Journey Mapping: For each user segment (in parallel) map the end-to-end user journey. Extract specific, actionable pain points focusing on:
     	1. Friction
      	2. Confusion
       	3. Workarounds 
	3. Consolidate Pain Points
    	1. Combine pain points across segments into a unified list
     	2. Remove duplicates and normalize similar issues 	
	4. Prioritize Pain Points
		1. Severity (how painful the problem is in terms of time or money)
  		2. Frequency (how often the problem surfaces)
		3. Reach (how many people the problem affects)
    5. Present ranked options to user. Allow user to select the final pain point to pursue 
7. [PROCESS] **Re-define the Product Goal**
	1. Reframe the Prioritized Pain Point as the product goal
	2. Define the Northstar Metric
8. [PROCESS] **UX Design**: Come up with 3 features to solve the Prioritized Pain Point. Till now you have been thinking logically. But here think creatively. For each feature think about:
	1. Interaction patterns
	2. Error states
	3. Accessibility considerations
9. [OPTIONAL INPUT] Ask the user to review the proposed features and ask whether to include, exclude, or refine them. The user may also suggest additional features.
10. [PROCESS] DATA SYSTEM DESIGN: For each approved feature come up with:
  	1. A/B Testing strategy (how do we know if the feature is working)
    2. KPIs to monitor and enable decision-making regarding the feature
    3. Dashboard specs (like what visualizations to use)  
11. [PROCESS] SOFTWARE SYSTEM DESIGN: Incorporating each approved feature come up with the following:
  	1. Functional requirements
    2. Non-functional requirements
    3. Dependencies (APIs, models, infra)
    Give the overall System Architecture overview
12. [PROCESS] Finally deliver the following:
    1. End-to-end implementation of all features
    2. Dashboard screen (one page to monitor KPIs of all the features)
    3. Generate a concise (<100 words), well-structured risk analysis. For each category, list one realistic risk and a corresponding mitigation. Use bullet points. Cover: Product, Technical, and Data risks.
