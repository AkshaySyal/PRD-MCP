# IDEATION-PROMPTS
Instead of fixing plan mode, idea is to leverage deep research feature and prompts to get to idea quickly

1. **User query**: Give a core idea, a problem to solve or just give a specific library or API to use or literally anything
2. **User query enrichment**: Gather additional context (maybe provide links or give a certain number of web searches to perform)
   1. Do a web search on:
      1. Market trend (Existing similar Product or Service, Competitors)
      2. Societal trend
      3. Technology trend 
3. **Prioritizing the High-level Product Goal**: Prioritize a high-level product objective. You should clearly justify why each product goal is relevant and provide a recommendation on which goal to pursue. ASK MEfor the final decision on which product goal to prioritize:
 	1. User Acquisition: Bring more users into the product
  	2. Activation: Reduce time-to-value by enabling users to reach the product’s core value as quickly as possible.
	3. Engagement: Drive deeper and more frequent interactions that reflect meaningful product usage
	4. Monetization Strategy: Capture value by translating user engagement into sustainable revenue streams.
	5. Product Quality: Deliver a consistently reliable, high-quality experience that meets user expectations
	6. Funnel smoothness: Minimize friction and drop-offs across user journey stages in the existing product or service
4. **User Empathy** You can start empathizing with user now:
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
    5. Present ranked options to user.
5. **Re-define the Product Goal**
	1. Reframe the Prioritized Pain Point as the product goal.
 	2. Give me the exact source of evidence about the pain point.
	3. Establish a Northstar Metric
 	4. Make a 30s pitch communicating in a clear way what & why I am solving this problem and how am I going to measure if the solution is working. Remember: Bottom Line Up Front.
6. **UX Design**: Come up with 3 features to solve the Prioritized Pain Point. Till now you have been thinking logically. But here think creatively. Ask me to review the proposed features and ask whether to include, exclude, or refine them. I may also suggest additional features. For each feature think about:
	1. Interaction patterns
	2. Error states
	3. Accessibility considerations
7. **Testing:** Ask me about positive and negative Acceptance Test Cases to clearly define expected success and failure scenarios. As you implement features, continuously design and enforce test cases across functional and integration tests. Ensure that each feature is validated in isolation and in combination with existing components. Maintain a regression test suite and run it after every change to prevent breakages.
8. **System Design:** Finally deliver the following WRITEUPS in a concise, well-structured, numbered format. Ask me to review the proposed plans and ask whether to include, exclude, or refine:
	1. DATA SYSTEM DESIGN: For each approved feature come up with:
  		1. A/B Testing strategy (how do we know if the feature is working)
    	2. KPIs to monitor and enable decision-making regarding the feature
    	3. Dashboard specs (like what visualizations to use)
     	4. Also, populate databases with fake data. I don't want the dashboards to look empty.   
	2. SOFTWARE SYSTEM DESIGN: Incorporating each approved feature come up with the following:
  		1. Functional requirements
    	2. Non-functional requirements
    	3. Dependencies (APIs, models, infra)
    	4. Overall System Architecture overview
    3. RISK ANALYSIS: For each risk category, list one realistic risk and a corresponding mitigation:
       	1. Product
       	2. Technical
       	3. Data

When building a demo the first 6 steps of SDLC must be followed:
1. Planning [Agentic + User] (Current)
2. Requirements Analysis [Agentic + User] (Current)
3. System Design [Agentic + User] (I have limited knowledge)
4. Implementation (Coding) [Purely Agentic] (Need best practices) [Need to learn how to configure]
5. Testing [Agentic + User] (Need best practices) [Need to learn how to configure]
6. Deployment [Purely Agentic] (Need best practices) [Need to learn how to configure]
7. Maintenance (A/B testing) (I have limited knowledge)
