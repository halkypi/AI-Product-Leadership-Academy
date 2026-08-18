# Domain 01 — LLM & AI Engineering Fundamentals: Canonical Resources

## Curatorial boundary

The target is enough systems literacy to design, prototype, debug, evaluate, and discuss an LLM application without drifting into deep ML theory, retrieval/RAG, agents, or evaluation as separate disciplines.

This domain optimizes for **capability gained per hour invested** and a build-first product-leadership mindset.

## Ranked candidates

| Rank | Resource | Disposition |
|---|---|---|
| 1 | Andrej Karpathy — *Intro to Large Language Models* | **CANON** |
| 2 | Chip Huyen — *AI Engineering*, Chapters 1, 2 & 10 | **CANON** |
| 3 | OpenAI — Function Calling | **CANON** |
| 4 | OpenAI — Model Selection | **CANON** |
| 5 | OpenAI — Developer Quickstart | **CANON** |
| 6 | OpenAI — Structured Model Outputs | Reference |
| 7 | OpenAI — Prompting | Reference |
| 8 | Anthropic — Building Effective Agents | Defer to Domain 06 |
| 9 | Anthropic — Effective Context Engineering for AI Agents | Defer to Domain 05 |
| 10 | fast.ai — Practical Deep Learning for Coders | Reject for this domain |

## 1. Andrej Karpathy — Intro to Large Language Models

URL: https://www.youtube.com/watch?v=zjkBMFhNj_g

Time: about 1 hour  
Difficulty: Beginner → intermediate

**Capability gained:** a usable mental model of LLMs: training versus inference, parameters, tokens, context, probabilistic outputs, capabilities, limitations, and security concerns.

**Why canon:** probably the highest capability-per-hour resource in the domain. It prevents a product leader from treating an LLM as magic or as merely a chatbot.

**Why alternatives lose:** Karpathy's deeper material is excellent but spends more time on implementation/model construction than this audience needs at the fundamentals stage. The academy should not teach transformer construction before applied systems literacy.

Author site: https://karpathy.ai/

## 2. Chip Huyen — AI Engineering, Chapters 1, 2 & 10

Repository: https://github.com/chiphuyen/aie-book  
Table of contents: https://github.com/chiphuyen/aie-book/blob/main/ToC.md  
Chapter summaries: https://github.com/chiphuyen/aie-book/blob/main/chapter-summaries.md  
O'Reilly book page: https://www.oreilly.com/library/view/ai-engineering/9781098166298/cover.html

Selected reading:

- Chapter 1 — Introduction to Building AI Applications with Foundation Models
- Chapter 2 — Understanding Foundation Models
- Chapter 10 — AI Engineering Architecture and User Feedback

Estimated time: about 4.5–5.5 hours for the selected material  
Difficulty: Intermediate

**Capability gained:** an end-to-end systems model covering foundation models, probabilistic outputs, sampling/structured outputs, the AI application stack, context, guardrails, routing, caching, orchestration, monitoring, and feedback.

**Why canon:** Huyen explicitly writes for people building applications with foundation models and includes technical product managers in the intended audience. The book focuses on durable fundamentals rather than one transient framework.

**Why not the full book:** the complete book is much larger. Later chapters map naturally to other academy domains such as evaluation, retrieval/agents, fine-tuning, datasets, and inference optimization. Requiring the whole book here would reduce capability/hour and duplicate future research.

## 3. OpenAI — Function Calling

URL: https://developers.openai.com/api/docs/guides/function-calling

Time: about 45–60 minutes including examples  
Difficulty: Intermediate

**Capability gained:** the central model/application contract:

1. the model receives available tools
2. the model requests a tool call
3. application code executes the deterministic action
4. the result returns to the model
5. the model continues

**Why canon:** understanding this primitive unlocks the mental model behind APIs, databases, search, Snowflake tools, MCP, agents, and workflows.

**Why alternatives lose:** framework-first tutorials introduce changing abstractions before the learner understands the underlying primitive.

## 4. OpenAI — Model Selection

URL: https://developers.openai.com/api/docs/guides/model-selection

Time: about 20–30 minutes  
Difficulty: Beginner → intermediate

**Capability gained:** quality/cost/latency tradeoff thinking. Model choice becomes a product and engineering decision against an explicit quality target, not a search for “the smartest model.”

**Why canon:** the decision framework is more durable than model leaderboards. It also establishes that prompting, retrieval, fine-tuning, and model choice are different levers rather than a maturity ladder.

**Why alternatives lose:** “best LLM” rankings and benchmark posts decay rapidly and encourage provider/model selection without a product quality target.

## 5. OpenAI — Developer Quickstart

URL: https://developers.openai.com/api/docs/quickstart

Time: about 30–45 minutes hands-on  
Difficulty: Beginner

**Capability gained:** make a real model request through an SDK, inspect input/output, and connect an LLM to ordinary application code.

**Why canon:** a build-first academy should not allow a participant to finish fundamentals having only read about an API. This is the minimal bridge from AI consumer to AI builder.

**Why alternatives lose:** Playground-only experience hides the application boundary; full API courses spend too much time on mechanics that modern coding tools can help generate.

## 6. OpenAI — Structured Model Outputs

URL: https://developers.openai.com/api/docs/guides/structured-outputs

Time: about 30–45 minutes  
Disposition: Reference, not mandatory canon

Structured outputs are an important application primitive, but the concept is narrow and is already sufficiently introduced by the selected systems material. Keep this as implementation-time documentation rather than mandatory reading.

## 7. OpenAI — Prompting

URL: https://developers.openai.com/api/docs/guides/prompting

Time: about 30 minutes  
Disposition: Reference, not mandatory canon

Prompting matters, but it is one control surface inside a larger system. Making it mandatory here would over-weight prompt technique relative to context, tools, model choice, retrieval, and evaluation.

## 8. Anthropic — Building Effective Agents

URL: https://www.anthropic.com/engineering/building-effective-agents

Disposition: **Defer to Domain 06 — Agents, Tools & Agentic Workflows**

This is high-quality canonical material. Anthropic's emphasis on simple, composable patterns and using the simplest sufficient solution is exactly aligned with the academy. It is deferred because agents are a separate domain, not because the resource is weak.

## 9. Anthropic — Effective Context Engineering for AI Agents

URL: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents

Disposition: **Defer to Domain 05 — Context Engineering, Retrieval & RAG**

This is canonical-quality material explaining why context engineering is broader than prompt engineering and why the information available at inference time is a first-class system design concern. It fits Domain 05 more cleanly.

## 10. fast.ai — Practical Deep Learning for Coders

URL: https://course.fast.ai/index.html

Disposition: **Reject for this domain**

fast.ai is excellent and the rejection is about relevance, not quality. The course devotes substantial time to training deep-learning systems across vision, NLP, tabular data, collaborative filtering, and related material. That is a poor capability-per-hour fit for foundation-model application engineering fundamentals for product leaders. Portions may become relevant to Domain 11.

## Final canonical set

Approve these five resources for Domain 01:

1. **Andrej Karpathy — Intro to Large Language Models**
2. **Chip Huyen — AI Engineering, Chapters 1, 2 & 10**
3. **OpenAI — Function Calling**
4. **OpenAI — Model Selection**
5. **OpenAI — Developer Quickstart**

Estimated total time: roughly **7–8 hours** by summing the individual estimates. This is not a prescribed curriculum or timeline.

Everything else is reference material or belongs more cleanly in a later domain.

**Domain 01 research stops here.**
