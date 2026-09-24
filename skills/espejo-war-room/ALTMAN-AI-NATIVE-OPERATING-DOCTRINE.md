# Altman AI-Native Operating Doctrine

## Purpose
This doctrine distills the operational principles from the Sam Altman interview summary provided by the Commander and converts them into reusable decision rules for the Espejo AI OS.

Use it when evaluating AI-native products, company strategy, agent adoption, platform decisions, product focus, iteration speed, leadership behavior, and long-horizon bets.

## 1. AI-Native Rebuild Test
For every important business, ask:
**If we started this company today with current AI capabilities, would we build it the same way?**

If no, identify what should be redesigned.

Questions:
- Which workflows exist only because AI was previously unavailable?
- Which roles can be upgraded by agents?
- Which customer experiences should become conversational or agentic?
- What would the product look like if software actively participated instead of waiting for clicks?
- What should be rebuilt from scratch rather than incrementally optimized?

Rule: Do not merely bolt AI onto old workflows. Reimagine the workflow around AI where economics and customer experience justify it.

## 2. Agent Adoption Advantage
The interview frames agents as a shift from software-as-a-tool toward software-as-an-active-participant.

Espejo rule:
Every business should identify at least one workflow where an AI agent can own a measurable outcome rather than simply assist a human.

Examples: lead follow-up, support triage, campaign analysis, mobile QA, research, content repurposing, CRM hygiene, scheduling, onboarding, reporting.

Goal:
**Goal → agent loop → verified result**

## 3. Human Inertia Is a Market Constraint
AI capability can advance faster than users change behavior.

Implications:
1. Superior technology does not automatically create adoption.
2. Products must reduce behavior change and fit existing habits until they are compelling enough to create new ones.

Questions:
- What existing habit is the customer being asked to abandon?
- Can the AI capability fit into a workflow they already use?
- Is the product asking the customer to learn too much?
- What would create an “iPhone moment” for this workflow?

Growth rule:
Sell the outcome in familiar language. Do not require customers to understand agents, MCP, models, or technical architecture.

## 4. Iterative Deployment
Use:
**Build → Deploy → Observe → Break → Fix → Learn → Repeat**

Rules:
- Prefer small live pilots over long internal speculation.
- Track failures explicitly.
- Record postmortems for meaningful failures.
- Use real customer behavior as evidence.
- Do not claim readiness without live verification.

## 5. Success Pattern Library
Maintain a library of what actually worked.

For every successful campaign, product improvement, sales motion, automation, or agent workflow record:
- what was attempted
- audience
- channel
- offer
- implementation
- metric before
- metric after
- cost
- time to result
- why it likely worked
- conditions required to repeat it

Growth Command should reuse proven winning patterns before inventing new ones.

## 6. Power-Law Bets
Do not spread equal resources across every idea.

For each project portfolio identify:
- the one project with the highest upside
- strongest evidence supporting it
- key non-consensus assumption
- what must be true
- what milestone earns additional resources

Use staged conviction:
**small test → evidence → larger bet**

## 7. Non-Consensus Thinking
Questions:
- What do we believe that most competitors do not?
- Why might the market be wrong?
- What evidence supports our belief?
- What experiment could falsify it quickly?

Rule:
A non-consensus opinion without evidence is not strategy.

## 8. Hands-On AI Leadership
Leadership should stay close enough to the technology to understand what it can and cannot do.

Commander rules:
- use the product directly
- inspect agent outputs
- test critical workflows personally
- review actual customer journeys
- give precise feedback
- do not rely only on summaries

Question:
**Have we touched the real system, or are we deciding from status reports?**

## 9. Feedback Quality Is a Competitive Advantage
Use:
- Observed problem
- Expected behavior
- Actual behavior
- Business/customer impact
- Evidence
- Priority
- Suggested correction

Avoid vague feedback such as “make it better.”

## 10. Platform Over Feature Sprawl
Before creating another standalone product, ask whether it should instead become:
- a reusable platform capability
- a shared service
- a common agent
- a shared API
- a skill
- a module used across businesses

Examples:
- one lead enrichment engine
- one content repurposing engine
- one mobile QA harness
- one analytics layer
- one agent security gate

## 11. Kill Good Ideas for Great Ones
A good idea does not automatically deserve resources.

Ask:
- What existing project loses time, money, or compute if we pursue this?
- Is this better than our current top priority?
- What is the opportunity cost?
- What should be paused or killed to make room?

## 12. Cost-Performance Discipline
Use the cheapest model/tool that reliably completes the task.

Use high-capability models for:
- strategy
- hard coding
- architecture
- ambiguous reasoning
- high-stakes analysis

Use cheaper models or deterministic code for:
- classification
- formatting
- routing
- repetitive transforms
- API calls
- scheduled checks
- simple extraction

Measure:
**Cost per successful outcome**

## 13. Single-Interface Simplicity
Prefer:
- one obvious primary action
- clear language
- minimal setup
- low cognitive load
- progressive disclosure

Question:
**Can the customer understand what to do in five seconds?**

## 14. Human-Centric Agent Design
Agents should increase human agency, not silently take over consequential decisions.

Approval remains required for:
- spending
- legal commitments
- destructive changes
- unapproved public publishing
- mass outreach
- price changes
- sensitive data access
- reputational-risk actions

## 15. Accident / Failure Reporting
For each meaningful incident record:
- date/time
- agent/system
- intended action
- actual outcome
- root cause
- customer impact
- recovery
- permanent fix
- prevention test

Rule:
Every repeated failure without a recorded correction is a system-design failure.

## 16. Simulated Feedback When Customers Are Limited
Before meaningful user volume exists, use:
- QA benchmarks
- usability tests
- expert review
- conversion simulations
- agent mystery shopping
- competitor comparison
- clearly labeled synthetic scenarios

Do not treat simulated feedback as equivalent to real customer demand.

## 17. Altman Filter for War Room
When relevant, add:

### AI-NATIVE REBUILD
If we started today with current AI, what would we redesign?

### AGENT OWNERSHIP
What measurable outcome can an agent own?

### HUMAN INERTIA
What behavior change are we asking from the customer?

### ITERATION
What can we deploy quickly to get real evidence?

### PLATFORM
Should this be a reusable capability instead of a standalone project?

### POWER-LAW BET
What is the highest-upside opportunity?

### NON-CONSENSUS VIEW
What do we believe that others do not, and what evidence supports it?

### FOCUS
What good idea should we pause or kill to protect the best one?

### COST-PERFORMANCE
Are we using more AI compute than the task requires?

### HUMAN CONTROL
Where must approval and transparency remain?

## 18. Application to Current Espejo Businesses

### Seven Jungles
- redesign as an AI-native service platform, not a traditional agency
- give agents ownership of lead research, CRM hygiene, follow-up preparation, reporting, and QA
- sell outcomes, not technical jargon
- share agent infrastructure across verticals
- run pilots before scaling

### SYBAI
- simplify the customer journey
- use one obvious entry point
- build reusable free tools as acquisition infrastructure
- improve from customer behavior
- avoid feature sprawl

### Prosta Tracker
- simplify onboarding
- keep guidance human-centered and transparent
- make mobile QA mandatory
- use agents for assistance, summarization, reminders, and logging
- maintain strong safety boundaries

### Statement IQ
- make it an active financial-document workflow
- use agents to classify, summarize, route, and surface next actions
- track failures carefully
- use deterministic processing when reasoning is unnecessary

### American Gold Supply
- use AI for discovery, merchandising, QA, and support
- keep storefront behavior familiar
- use engineering-as-marketing tools for organic acquisition

### Golf De La Vega
- keep AI backstage for design iteration, content, QA, merchandising, and analysis
- preserve a premium human-facing brand
- store successful creative patterns as reusable brand memory

## 19. Core Espejo Operating Loop
**OBSERVE → THINK → ACT → VERIFY → LEARN → FOCUS → REPEAT**

Final doctrine:
Build AI-native, but design for real humans.
Deploy early enough to learn.
Keep leaders close to the technology.
Let agents own measurable outcomes.
Preserve human control over consequential decisions.
Prefer reusable platforms over repeated one-off systems.
Use the cheapest intelligence that reliably completes the job.
Record what works.
Record what breaks.
Kill good ideas when they distract from great ones.
And repeatedly ask:
**If we started this business today with current AI, what would we build differently?**
