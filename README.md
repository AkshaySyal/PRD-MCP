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
    5. Present ranked options to user.
7. [INPUT] Allow user to select the final pain point to pursue 
8. [PROCESS] **Re-define the Product Goal**
	1. Reframe the Prioritized Pain Point as the product goal. Give me the exact source of evidence about the pain point.
	2. Define the Northstar Metric
9. [PROCESS] **UX Design**: Come up with 3 features to solve the Prioritized Pain Point. Till now you have been thinking logically. But here think creatively. For each feature think about:
	1. Interaction patterns
	2. Error states
	3. Accessibility considerations
10. [OPTIONAL INPUT] Ask the user to review the proposed features and ask whether to include, exclude, or refine them. The user may also suggest additional features.
11. [PROCESS] Finally deliver the following WRITEUPS in a concise, well-structured, numbered format:
	1. DATA SYSTEM DESIGN: For each approved feature come up with:
  		1. A/B Testing strategy (how do we know if the feature is working)
    	2. KPIs to monitor and enable decision-making regarding the feature
    	3. Dashboard specs (like what visualizations to use)  
	2. SOFTWARE SYSTEM DESIGN: Incorporating each approved feature come up with the following:
  		1. Functional requirements
    	2. Non-functional requirements
    	3. Dependencies (APIs, models, infra)
    	4. Overall System Architecture overview
    3. RISK ANALYSIS: For each risk category, list one realistic risk and a corresponding mitigation:
       	1. Product
       	2. Technical
       	3. Data
12. [OPTIONAL INPUT] Ask the user to review the proposed plans and ask whether to include, exclude, or refine.

need to use skill-creator skill 
I need to find and configure skills for the things I don't know how to do. Over time, I need to iterate on them and define how to do them properly.
- UX Design is something that could be done for web and app by the LLM. But for certain applications like voice agents, I need to do it
- A/B testing skill
- Software System Design skill
- Risk Analysis

I think I wanna write test cases to ensure the app works and demo does not break. When I think about test cases, I can think of positive and negative Acceptance Test Cases. But I think the coding agent should think of test cases at all levels as it generates code.

The Skills course reveals that multiple sub-agents are created for specific tasks. And their specific instructions are written inside skills folder. This prevents overloading the context window of the main coding agent, it focuses on development, while the sub-agents perform their specific tasks according to their specific best practices. Sub-agents used: code-reviewer and test-generator


When building a demo the first 6 steps of SDLC must be followed:
1. Planning [Agentic + User] (Current)
2. Requirements Analysis [Agentic + User] (Current)
3. System Design [Agentic + User] (I have limited knowledge)
4. Implementation (Coding) [Purely Agentic] (Need best practices) [Need to learn how to configure]
5. Testing [Agentic + User] (Need best practices) [Need to learn how to configure]
6. Deployment [Purely Agentic] (Need best practices) [Need to learn how to configure]
7. Maintenance (Part of the pitch) (A/B testing) (I have limited knowledge)

Maybe I can get 4,5,6 generated or web fetched. And that could be used to setup the coding environment.
For now, need to rely on replit

I think I can use Replit entirely to build this end-to-end. Need to re-arrange the prompt at 11 and add test case point also.
Also, populate databases with fake data. I don't want the dashboards to look empty.
