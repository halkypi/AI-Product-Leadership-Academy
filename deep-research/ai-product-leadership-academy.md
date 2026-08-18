# AI Product Leadership Academy: Capability Domain Canon

## Curatorial decision

The academy should **not** mirror the usual taxonomy of generative-AI courses. A list such as “prompting, RAG, agents, fine-tuning, vector databases” is organized around technologies rather than the capabilities a product leader needs.

For this audience and environment, I would organize the canon around **twelve capability domains**, with the first eight forming the core. The ranking optimizes for the outcomes in the problem statement: becoming a stronger AI user, finding valuable AI opportunities, leading delivery, collaborating with engineering/data science, governing risk, and independently building prototypes.

Several signals from current practitioner guidance drive this structure:

OpenAI's current production guidance treats model choice, context, retrieval, tools, evaluation, cost, latency, safety, and deployment as interacting parts of an AI system rather than independent tricks. Its evaluation guidance explicitly notes that generative systems are variable enough that conventional deterministic software tests are insufficient by themselves. Anthropic's engineering guidance has moved in the same direction: from simple LLM calls toward context engineering, tool design, evaluations, and agent harnesses. Anthropic explicitly characterizes context engineering as broader than prompt engineering and advises starting with simple LLM/API patterns before adding unnecessary agentic complexity. The enterprise platforms in the stated environment now expose these same primitives directly. Snowflake offers AI functions, semantic analysis over structured data, retrieval, agent orchestration, Python execution, custom tools, and governed data access; GitHub Copilot has evolved beyond autocomplete into repository-aware coding agents capable of planning, editing code, and producing pull requests. That leads to the following ranking.

## Ranked capability domains

| Rank | Capability domain | Priority | Capability unlocked |
|---|---|---|---|
| **1** | **LLM & AI Engineering Fundamentals** | Essential | Understand what modern AI systems actually are, what models can and cannot do, and how an AI application is assembled |
| **2** | **AI Product Discovery & Opportunity Framing** | Essential | Identify where AI creates genuine user/business value and choose the right AI approach |
| **3** | **Evaluation, Reliability & AI Quality** | Essential | Define “good,” measure it, diagnose failures, and make evidence-based ship/no-ship decisions |
| **4** | **AI-Assisted Building: Python, Git & GitHub Copilot** | Essential | Independently turn product ideas into working software and communicate with engineers through executable artifacts |
| **5** | **Context Engineering, Retrieval & RAG** | Essential | Ground models in enterprise knowledge and systematically improve what the model knows at inference time |
| **6** | **Agents, Tools & Agentic Workflows** | Essential | Design systems that reason over tasks, invoke tools, take actions, and operate across multiple steps |
| **7** | **Responsible AI, Security & Governance** | Essential | Assess risk, design controls, establish human oversight, and participate credibly in enterprise governance |
| **8** | **Snowflake AI & Data Application Engineering** | Essential for this environment | Build AI directly where governed enterprise data lives |
| **9** | **AI-Native Knowledge Work & Delegation** | High | Use AI continuously to accelerate PM research, synthesis, analysis, writing, decision support, and execution |
| **10** | **Human-AI Product Design** | High | Design appropriate autonomy, feedback, trust, failure recovery, uncertainty, and human oversight into products |
| **11** | **ML & Data Science Fundamentals for Product Leaders** | Supporting | Work intelligently with data scientists and recognize when classical ML is preferable to generative AI |
| **12** | **AI Strategy, Economics & Portfolio Management** | Supporting | Make build/buy/platform/model choices and reason about AI investments at product and portfolio level |

The ranking is deliberately **not a learning sequence**. It represents the expected value of finding exceptional canonical material in each domain.

### LLM & AI Engineering Fundamentals

**Rank: highest priority.**

This is the foundational technical literacy of an AI product leader, but it should be taught as **systems literacy rather than ML theory**.

The required mental model includes models and inference, tokens and context, APIs, structured outputs, tool calling, multimodality, embeddings at a conceptual level, model selection, latency, cost, nondeterminism, prompting as one control surface, and the major techniques for changing system behavior.

Why it is first: without this domain, PMs cannot reliably distinguish a model problem from a context problem, retrieval problem, data problem, tool problem, evaluation problem, UX problem, or ordinary software problem. OpenAI's own optimization guidance explicitly treats prompting, RAG, and fine-tuning as different levers for different problems rather than a maturity ladder; its model-selection guidance frames model choice as a quality/latency/cost tradeoff. This domain is also where **“prompt engineering” belongs**. Prompting is useful; a standalone Prompt Engineering domain is not. Anthropic now describes context engineering as the broader task of controlling all information available to the model, while OpenAI's documentation similarly places instructions within a larger system of context, tools, retrieval, and evaluation. **Canonical boundary:** enough understanding to design, prototype, debug, evaluate, and discuss an LLM application. Not transformer mathematics, gradient derivations, pretraining theory, or model architecture surveys.

### AI Product Discovery & Opportunity Framing

**Rank: second.**

This is the most important distinctly **product-leadership** domain.

The skill is not “brainstorm AI use cases.” It is being able to determine:

> What user or business problem exists, what task is being improved, why AI is appropriate, what level of quality is required, what human role remains, what data/context is available, what failure costs are tolerable, and whether generative AI is even the right technology.

Google's current guidance explicitly distinguishes generative AI from traditional AI and recommends a business-value-driven approach to defining AI use cases. Google's ML material separately treats *problem framing* as a core capability for mapping real-world problems to ML solutions. This domain ranks above agents or RAG because technology selection should follow problem selection. A PM who can build an agent but cannot identify a high-value problem is not yet an AI product leader.

It also protects against one of the most common AI-product pathologies: **solution-first roadmaps**, where teams start with “we need a chatbot/agent/copilot” and then search for a problem.

**Canonical boundary:** opportunity discovery, task decomposition, AI suitability, outcome definition, workflow redesign, feasibility/value/risk assessment, and AI-versus-non-AI choices.

It should not become generic PM instruction.

### Evaluation, Reliability & AI Quality

**Rank: third.**

This deserves its own domain and should sit much higher than most AI-product programs place it.

Generative AI changes the PM's relationship with acceptance criteria. A feature can “work” technically while producing unacceptable behavior on a meaningful subset of inputs. OpenAI therefore defines evals as a way of testing AI systems despite their variable output and recommends continuous evaluation against representative data; Anthropic similarly argues that evaluations make failures and behavioral changes visible before they reach users. For product leaders, the capability is broader than running an evaluation framework. It includes:

defining success criteria; building representative test sets; choosing deterministic, rubric, human, and model-based graders; understanding precision/recall and task-specific metrics where relevant; error analysis; regression testing; evaluating retrieval separately from generation; measuring agents at outcome and trajectory level; and balancing quality against latency and cost.

This is arguably the **single biggest difference between ordinary software product management and competent AI product management**. The PM has to participate in defining what “good enough” means.

Anthropic's 2026 agent-evaluation guidance emphasizes precisely this challenge: agents can take multiple valid paths and interact with tools and state, making evaluation more complicated than checking one deterministic output. **Canonical boundary:** eval-driven product development and reliability. Observability belongs here insofar as it enables diagnosis and continuous quality improvement.

Generic analytics and experimentation remain normal PM competencies and do not need duplication.

### AI-Assisted Building: Python, Git & GitHub Copilot

**Rank: fourth.**

This should be a distinct academy capability rather than assuming “technical people already know it.”

The target is not turning PMs into software engineers. The target is making **working software a normal product-thinking medium**.

A competent participant should be able to use Python, libraries, APIs, notebooks/scripts, Git repositories, tests, environment configuration, and an AI coding agent to turn an idea into a testable application. GitHub Copilot's current capabilities now include repository research, implementation planning, code modification, branches, and pull-request creation, while GitHub explicitly recommends checking Copilot's work rather than treating generated code as inherently correct. That changes what “technical enough for a PM” can reasonably mean.

There is also evidence that AI coding tools materially alter software work. GitHub's enterprise study with Accenture used an RCT design, while subsequent GitHub research found measurable improvements in functional correctness in its controlled coding study. These studies concern developers rather than PMs, so they should not be overgeneralized, but they support treating AI-assisted coding as a serious work modality rather than a novelty. Anthropic's observed Claude Code usage likewise shows a substantially higher share of automation than ordinary Claude.ai interactions, reinforcing the distinction between conversational AI use and agentic software building. **Canonical boundary:** prototype-grade engineering literacy, AI-assisted coding, testing/debugging, Git, and executable artifacts.

Not computer-science fundamentals, algorithm interview preparation, or “learn Python” coursework for its own sake.

### Context Engineering, Retrieval & RAG

**Rank: fifth.**

I would **merge RAG and Context Engineering**, rather than make them separate domains.

RAG is an implementation pattern. Context engineering is the broader capability.

Anthropic defines context engineering as curating and maintaining the optimal information available to the model during inference. Retrieval is one major mechanism for doing that, alongside instructions, tool outputs, memory, summaries, state, and other contextual material. OpenAI likewise describes RAG as supplying domain-specific context to the model and notes that major customer deployments can achieve substantial accuracy improvements using prompting plus retrieval without model fine-tuning. The domain should therefore cover:

context construction; embeddings conceptually; semantic and keyword retrieval; chunking; metadata; ranking; grounding; citation; retrieval evaluation; query transformation; enterprise knowledge boundaries; memory/state; context-window management; and knowing when retrieval is unnecessary.

Snowflake makes this especially relevant. Cortex Search is explicitly designed to support RAG over Snowflake data, and current Cortex Agents can use retrieval over enterprise documents as one tool within a larger workflow. **Canonical boundary:** getting the *right information* into the model at the right moment.

A separate “vector databases” domain would be too implementation-specific.

### Agents, Tools & Agentic Workflows

**Rank: sixth.**

Agents clearly belong in the canon, but **not at the top**.

This is an important curatorial distinction.

Anthropic's influential practitioner guidance recommends beginning with the simplest possible system and increasing autonomy only when the problem warrants it; it distinguishes deterministic workflows from more autonomous agents. Current OpenAI documentation similarly describes agents as applications that plan, call tools, collaborate across specialists, and maintain enough state to complete multi-step tasks. The durable capability is therefore not “learn LangChain” or “build a multi-agent crew.” It is understanding:

agent versus workflow; orchestration; tools/function calling; state; planning; execution; tool ergonomics; MCP and related interoperability concepts; permissions; approvals; failure recovery; autonomy boundaries; agent evaluation; and the circumstances in which a simple LLM call or deterministic workflow is better.

The emphasis on **tools** is crucial. Anthropic's engineering work argues that tool interface quality materially influences agent performance, while MCP has emerged as an open protocol for exposing external systems to agents. Snowflake now exposes the same architecture directly: Cortex Agents can orchestrate Cortex Analyst, Cortex Search, analytical search, Python code execution, custom functions, MCP connectors, and other tools. **Canonical boundary:** agentic system design and product judgment.

Framework-specific “agent tutorials” should generally be rejected unless they teach durable underlying patterns.

### Responsible AI, Security & Governance

**Rank: seventh, but mandatory.**

Its rank should not be interpreted as optionality.

NIST's AI Risk Management Framework is explicitly lifecycle-oriented, using **Govern, Map, Measure, and Manage** functions; its Generative AI Profile extends that approach to risks specific to generative systems. NIST's AI RMF 1.0 is currently being revised, which is another reason the academy should teach the risk-management mental model rather than memorization of one fixed policy document. The GenAI profile identifies issues including confabulation, privacy, information integrity, information security, intellectual property, and human-AI configuration, demonstrating why “responsible AI” cannot be reduced to fairness training or an annual compliance module. Modern agents add new concerns. OpenAI's current agent-safety material warns about prompt injection and private-data leakage through connected tools and recommends reducing privileges and attack surfaces; human approval and automated guardrails are separate control mechanisms. For PMs, the capability is:

risk identification; appropriate-use decisions; data/privacy awareness; security and prompt injection; human-in-the-loop design; access control and least privilege; transparency; incident thinking; red teaming; evaluation for safety; and working constructively with legal, security, compliance, privacy, and model-risk teams.

**Canonical boundary:** practical product risk management.

Not ethics philosophy detached from product decisions, and not regulation memorization.

### Snowflake AI & Data Application Engineering

**Rank: eighth overall, but much higher for immediate organizational applicability.**

Snowflake should get a dedicated domain because the stated environment is Snowflake-centric and because the platform now spans enough of the applied-AI stack that “Snowflake knowledge” is no longer synonymous with SQL.

Current Snowflake functionality includes AI functions over text and multimodal data, Cortex Search, Cortex Analyst for natural-language interaction with structured enterprise data, Cortex Agents, Python integration, and traditional Snowflake ML/model-registry capabilities. Cortex Agents specifically operate inside Snowflake's governed environment and inherit data-access controls through configured tools, which makes the platform especially relevant to enterprise AI product leaders. Snowflake also exposes an increasingly important pattern: applying generative AI directly to unstructured data and combining semantic AI operations with ordinary SQL. Its current analytical-search architecture, for example, combines retrieval, AI extraction/filtering/aggregation, and SQL rather than relying on naïve top-*k* RAG alone. **Canonical boundary:** enough Snowflake AI to prototype and reason about enterprise architecture, security, economics, and feasibility.

Do not turn this into Snowflake certification preparation.

### AI-Native Knowledge Work & Delegation

**Rank: ninth.**

This domain directly addresses the goal that PMs should **use AI daily**, and its capability-per-hour is extremely high.

Experimental evidence from the BCG/HBS study found that generative AI produced substantial speed and quality gains on tasks lying inside the model's capability frontier while producing worse outcomes on a task outside that frontier. The important lesson is not a universal productivity percentage; it is the “jagged frontier”: users must learn through repeated use where AI is strong, where it fails, and when verification is necessary. Ethan Mollick has subsequently argued that AI use is evolving from conversational “co-intelligence” toward delegating longer-running work to agents, making **task delegation and verification** more durable skills than clever prompt construction. The domain should cover:

task decomposition; delegation; research; analysis; synthesis; critique; writing; structured reasoning support; using multiple modes/tools; verification; managing context; reusable instructions; and deciding when AI should not be used.

**Canonical boundary:** becoming an effective AI-augmented knowledge worker.

No prompt libraries, “50 magic prompts,” persona tricks, or prompt-engineering theater.

### Human-AI Product Design

**Rank: tenth.**

AI UX differs from ordinary deterministic software UX because the system can be uncertain, variable, wrong, proactive, and increasingly autonomous.

Google's People + AI Research work explicitly positions its guidebook as a toolkit for teams building human-centered AI products, while its current material targets the product lifecycle and responsible human-AI interaction. The durable questions include:

How much autonomy should the AI have?  
When should it ask the user?  
How are uncertainty and limitations communicated?  
How does the user correct it?  
How does the product recover from failures?  
What should be automated versus suggested?  
What evidence or provenance should users see?  
When is human approval mandatory?

These issues grow rather than shrink as systems become more agentic. Anthropic's 2026 work on agent autonomy concludes that effective oversight increasingly requires both post-deployment monitoring and better human-AI interaction mechanisms for managing autonomy and risk. **Canonical boundary:** product interaction design for probabilistic and autonomous systems.

Generic UI design does not belong.

### ML & Data Science Fundamentals for Product Leaders

**Rank: eleventh, intentionally.**

This domain belongs in the academy, but the academy's principles correctly reject making classical ML the center.

PMs still need enough understanding to collaborate effectively with data science around:

supervised versus unsupervised learning; classification/regression/ranking/recommendation; train/validation/test; labels; leakage; features; overfitting; precision/recall; thresholds; offline versus online performance; experimentation; drift; inference; model lifecycle; and why data quality often matters more than algorithm novelty.

Google continues to treat ML problem framing and managing ML projects as foundational competencies, and its current enterprise guidance explicitly asks teams to choose between generative AI, traditional predictive AI, or combinations of them rather than defaulting everything to LLMs. Snowflake itself continues to support conventional ML development and model lifecycle management alongside its generative-AI capabilities. That makes this domain necessary for PM–DS partnership, but it does **not** justify teaching calculus, backpropagation, neural-network derivations, or an academic survey of ML algorithms.

**Canonical boundary:** model-and-data literacy required to make product decisions.

### AI Strategy, Economics & Portfolio Management

**Rank: twelfth.**

This is important but deliberately last.

The failure mode would be creating PMs who can discuss “AI transformation” and platform strategy without having personally built or evaluated a serious AI system.

The useful strategic capability is downstream of technical understanding:

build versus buy; model/provider choice; proprietary versus commodity advantage; data advantage; switching costs; model portability; cost/latency/quality tradeoffs; central platform versus embedded teams; workflow redesign; automation versus augmentation; organizational adoption; portfolio prioritization; and where durable differentiation actually resides.

Current provider documentation reinforces the economic nature of engineering decisions: OpenAI explicitly frames model selection around quality, latency, and cost, while Snowflake separately meters AI-function, retrieval, and agent-related consumption. Current field evidence also argues against simplistic “AI automates everything” strategy. Anthropic's Economic Index distinguishes augmentation from automation and continues to find substantial variation by task, interface, and deployment mode. **Canonical boundary:** strategy grounded in actual system economics and product capability.

Generic “AI is transforming every industry” material should not enter the canon.

## Boundary decisions

The biggest opportunity to keep the eventual reading list small is to **collapse overlapping buzzword domains before selecting resources**.

| Candidate domain | Decision | Reason |
|---|---|---|
| **LLMs** | Merge into **LLM & AI Engineering Fundamentals** | Models only matter in the context of systems built around them |
| **AI Engineering** | Keep, combined with LLM fundamentals | Central capability |
| **Prompt Engineering** | **Reject as standalone** | A useful technique, but subordinate to context, evaluation, tools, and system design |
| **Context Engineering** | Keep | Durable abstraction |
| **RAG** | Merge into **Context Engineering, Retrieval & RAG** | RAG is one context-supply pattern, not an independent discipline |
| **Embeddings / Vector DBs** | Do not create separate domains | Implementation concepts inside retrieval |
| **Evaluation** | Keep as standalone | Distinct and critical product-leadership capability |
| **Agents** | Keep | Durable architecture, but only after simpler systems are understood |
| **MCP** | Do not create separate domain | Important protocol inside agents/tools, not a product-leadership capability itself |
| **GitHub Copilot** | Merge with **AI-Assisted Building** | The durable skill is AI-native software creation, not one product UI |
| **Python** | Merge with **AI-Assisted Building** | Medium for building, not the academy's subject |
| **Snowflake AI** | Keep | Environment-specific enough to justify a dedicated applied domain |
| **AI Product Management** | **Reject as one broad bucket** | Too vague; split into discovery/opportunity, evaluation, UX, governance, and strategy |
| **AI Strategy** | Keep, but low | Highest value after hands-on grounding |
| **Responsible AI** | Keep | Enterprise deployment demands explicit risk-management capability |
| **AI UX** | Keep as **Human-AI Product Design** | Probabilistic/autonomous products introduce distinct interaction problems |
| **Classical ML** | Keep narrowly | Necessary for PM–DS partnership and choosing the right technology |
| **Fine-tuning** | Do not create separate domain | Optimization technique inside AI Engineering |
| **MLOps / LLMOps** | Do not create separate PM domain | Production lifecycle concepts belong in AI Engineering, Evaluation, Snowflake, and Governance |
| **AI literacy** | **Reject** | Too passive for a build-first academy |
| **Certifications** | **Reject as a capability domain** | Credential is not capability |

This consolidation is supported by current practitioner architectures. OpenAI treats prompt engineering, retrieval, fine-tuning, evaluation, production optimization, and model selection as interdependent levers; Anthropic puts prompts inside the broader discipline of context engineering and recommends adding agent complexity only when needed.

## Why this ordering

The top of the ranking deliberately alternates **product judgment and building competence** rather than front-loading theory.

The central capability loop is:

**understand what AI systems can do → identify worthwhile problems → define measurable quality → build something real → improve its context → add autonomy where justified.**

That is not proposed as a curriculum sequence; it explains why these domains have unusually high leverage. Evaluation belongs near the center because every later capability becomes more rigorous when PMs can measure outcomes rather than judge demos subjectively. OpenAI and Anthropic both now put evaluation at the center of production AI development. The environment-specific tools come after the durable concepts in the ranking. Snowflake and GitHub Copilot are exceptionally relevant here, but individual platform features change faster than the underlying concepts of model behavior, evaluation, retrieval, tool use, access control, and software construction. GitHub Copilot's feature surface has already expanded from inline completion to autonomous repository-level agents, while Snowflake's AI surface now spans functions, retrieval, structured-data reasoning, agents, and code execution. Governance is mandatory but should be **embedded in actual product decisions**, not delivered as detached compliance literacy. NIST's own framework takes this lifecycle view: risk management spans governance, mapping context, measurement, and active management rather than a one-time review gate. Finally, strategy is intentionally downstream. The academy's stated principles—practical, product-first, Python-first, build-first—are better served by producing leaders whose strategic opinions come from direct experience with the capabilities, failure modes, economics, and constraints of working systems.

## Phase boundary

**Recommended canonical domain order**

1. **LLM & AI Engineering Fundamentals**
2. **AI Product Discovery & Opportunity Framing**
3. **Evaluation, Reliability & AI Quality**
4. **AI-Assisted Building: Python, Git & GitHub Copilot**
5. **Context Engineering, Retrieval & RAG**
6. **Agents, Tools & Agentic Workflows**
7. **Responsible AI, Security & Governance**
8. **Snowflake AI & Data Application Engineering**
9. **AI-Native Knowledge Work & Delegation**
10. **Human-AI Product Design**
11. **ML & Data Science Fundamentals for Product Leaders**
12. **AI Strategy, Economics & Portfolio Management**

For purposes of the requested process, **LLM & AI Engineering Fundamentals is the highest-priority domain**.

**Phase One stops here.**
