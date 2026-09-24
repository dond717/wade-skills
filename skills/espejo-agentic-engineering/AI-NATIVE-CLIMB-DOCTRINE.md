# Espejo AI-Native Climb Doctrine

## Purpose

This doctrine adapts the framework from the source **“5 Steps to AI Native Playbook” by MEZ** into the Espejo AI OS.

Source framework:
- Base Camp: Foundation Before AI
- Step 1: Context
- Step 2: Execution
- Step 3: Delegation
- Step 4: Autonomy
- Step 5: Compound

The source argues that AI-native maturity should be judged by how much useful business work can run without constant manual intervention, not by tool count or headcount. This doctrine preserves that core ladder while adding Espejo-specific verification, security, cost, and approval gates.

This is an adaptation for the Espejo AI OS, not a verbatim reproduction of the source.

---

# THE ESPEJO AI-NATIVE CLIMB

## LEVEL 0 — FOUNDATION

Source concept:
Audit → Document → Delete → Simplify

Espejo interpretation:
Before AI touches a workflow, understand the actual process and remove unnecessary complexity.

Required:
- list tools, subscriptions, systems, and recurring jobs
- document the real workflow
- remove work that should not exist
- simplify the remaining process
- identify the system of record
- define ownership and handoffs
- define measurable success

Graduate only when:
- the process is documented well enough for another operator to follow
- unnecessary steps have been removed
- the workflow has a clear start, finish, and owner

Status:
**AI-NATIVE LEVEL 0 — FOUNDATION**

---

## LEVEL 1 — CONTEXT

Source concept:
Build the Brain. AI should answer from the business's real knowledge, not generic information.

Espejo interpretation:
Give the agent durable, relevant, structured context.

Context may include:
- SOPs
- offers
- pricing
- policies
- customer profiles
- brand voice
- examples
- project state
- business rules
- approved tools
- known constraints
- metrics

Important adaptation:
The source recommends Notion as the Brain. Espejo does not require Notion. The requirement is a durable, structured, searchable source of truth available to the agent.

Graduate only when:
- the agent can answer business-specific questions from real context
- the agent distinguishes known facts from missing information
- context is current enough for the workflow
- the agent does not rely on generic guesses where internal knowledge is required

Status:
**AI-NATIVE LEVEL 1 — CONTEXT**

---

## LEVEL 2 — EXECUTION

Source concept:
Give AI hands. AI stops only advising and begins working inside real tools.

Espejo interpretation:
The agent can complete a real task through tools, APIs, code, browser actions, or connected systems.

Required:
- tool access
- clearly defined completion state
- checkpoint or review status
- logs/evidence
- bounded permissions
- cost boundary

Example:
Instead of drafting a CRM update in chat, the system prepares or writes the CRM record in the actual system.

Graduate only when:
- one complete task works end to end
- the result lands in the correct real system
- completion is verified
- failures are visible
- the human does not need to manually copy/paste the middle steps

Status:
**AI-NATIVE LEVEL 2 — EXECUTION**

---

## LEVEL 3 — DELEGATION

Source concept:
AI owns whole jobs, not isolated tasks.

Espejo interpretation:
The Commander delegates a measurable job with a trigger, rules, tools, completion criteria, and review loop.

A whole job includes:
- trigger
- objective
- inputs
- steps or decision space
- tools
- expected output
- verification
- escalation conditions

Examples:
- qualify a lead
- prepare a weekly growth report
- research and score prospects
- generate and validate a proposal draft
- run a mobile QA pass

Source insight preserved:
Prefer named jobs over vague agent titles. “Prepare Monday content brief” is more testable than “CMO Agent.”

Graduate only when:
- the agent repeatedly completes the whole job
- outputs are ready for review rather than rewrite
- known failures are handled or escalated
- performance is measured

Status:
**AI-NATIVE LEVEL 3 — DELEGATION**

---

## LEVEL 4 — AUTONOMY

Source concept:
The system triggers itself and runs without manual initiation.

Espejo interpretation:
A workflow or agent may self-trigger only after it has earned autonomy.

Possible triggers:
- schedule
- webhook
- new lead
- new sale
- status change
- new email or event
- monitoring condition

Autonomy requires:
- explicit trigger
- pass/fail checks
- safe stop
- failure alert
- bounded retries
- cost limits
- logging
- permission limits
- verification
- escalation
- human approval for consequential actions

Important distinction preserved from source:

**Workflow**
A fixed sequence that runs predictable steps.

**Agent**
Chooses the next action dynamically toward a goal.

Do not use an agent where a deterministic workflow is enough.

### AUTONOMY GATE

An agent may not be promoted to Level 4 unless:

1. Level 0–3 requirements are already satisfied.
2. Success criteria are explicit.
3. Eval performance is acceptable.
4. False-success risk is understood.
5. Failure recovery has been tested.
6. Security boundaries are defined.
7. Tool permissions use least privilege.
8. Cost per run is measured or bounded.
9. Maximum iterations / retries are defined.
10. Human approval boundaries are explicit.
11. Logging and observability are active.
12. A safe-stop path exists.

Graduate only when:
- the workflow reliably self-triggers
- it completes without manual initiation
- failures stop safely and alert appropriately
- consequential actions remain within approval policy

Status:
**AI-NATIVE LEVEL 4 — AUTONOMY**

---

## LEVEL 5 — COMPOUND

Source concept:
You architect, it scales. Reusable systems produce more output without proportional increases in manual effort.

Espejo interpretation:
Build reusable factories, not isolated automations.

A compound system should:
- reuse common capabilities
- learn from verified results
- improve templates, prompts, SOPs, and routing
- share infrastructure across businesses or jobs
- increase output without matching increases in manual labor
- expose cost and quality metrics
- prevent degradation as volume increases

Important correction:
The source describes additional runs as effectively costing nothing. Espejo does not adopt that literally.

Every scaled system must account for:
- model inference
- API usage
- hosting
- storage
- databases
- communications
- observability
- maintenance
- human review
- failure handling

Graduate only when:
- one reusable system supports multiple runs or jobs
- quality remains acceptable at higher volume
- operating cost is known
- learning from results improves future execution
- human operating effort grows materially slower than output

Status:
**AI-NATIVE LEVEL 5 — COMPOUND**

---

# AI-NATIVE MATURITY FIELD

Every important Espejo agent, workflow, or business process should declare:

**CURRENT AI-NATIVE LEVEL: 0 / 1 / 2 / 3 / 4 / 5**

Also record:

- Current level:
- Evidence:
- Missing gate:
- Next promotion test:
- Human approval boundary:
- Cost per run:
- Verification method:

Do not promote a system because it sounds sophisticated.

Promote only when the gate is demonstrated.

---

# PROMOTION RULE

Use:

**ASSIST → EXECUTE → DELEGATE → AUTONOMOUS → COMPOUND**

No skipping levels for important workflows.

A system may remain at a lower level permanently if that is safer, cheaper, or more reliable.

More autonomy is not automatically better.

---

# CORE SOURCE-DERIVED PRINCIPLES TO KEEP

From the playbook:

- AI-native maturity is about autonomy, not tool count.
- Clean up the process before automating it.
- Context matters more than clever prompting.
- AI becomes materially more useful when it can work inside real systems.
- Whole jobs are better units of delegation than vague agent roles.
- Autonomy should be earned.
- A workflow follows fixed steps; an agent chooses steps.
- The highest level is reusable systems that compound output and learning.

---

# ESPEJO ADDITIONS

The Espejo AI OS adds requirements that are not explicit in the source:

- evaluation before autonomy
- bounded loops
- cost-per-success measurement
- security review
- least privilege
- source verification
- explicit failure recovery
- safe stops
- human approval boundaries
- regression testing
- cross-agent observability
- reusable infrastructure across businesses

---

# AGENTIC ENGINEERING CHECK

Before designing or upgrading an agent, answer:

## FOUNDATION
Is the underlying process documented, simplified, and worth automating?

## CONTEXT
Does the agent have the right current business context?

## EXECUTION
Can it complete the task in the actual system?

## DELEGATION
Can it own the whole job with review-ready output?

## AUTONOMY
Has it earned self-triggering execution through evals, guardrails, and recovery?

## COMPOUND
Can the same infrastructure support more runs, jobs, or businesses without quality collapse?

---

# DEFINITION OF SAFE AUTONOMY

Safe autonomy means:

**Self-triggered + bounded + observable + verified + recoverable + cost-controlled + permission-limited + human-governed**

Anything less should not be called production autonomy in the Espejo AI OS.

---

# SOURCE

MEZ, **“5 Steps to AI Native Playbook”**, Notion page:
https://mezcorp.notion.site/5-Steps-to-AI-Native-Playbook-b336e20f7fe34e4e977a9757359cbf84

Source structure preserved:
Base Camp → Context → Execution → Delegation → Autonomy → Compound.
