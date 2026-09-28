# The Road Ahead: From Using AI to Building It

**Townhall Address — 15 minutes, formal, one-way delivery**
**Presented by: Technical Manager & Architect, on behalf of leadership**

---

# PART 1: OUTLINE

## 1. Purpose of Today's Address (45 sec)
On behalf of leadership, this session outlines the company's strategic direction as the technology landscape evolves. Distinguish from earlier sessions: "Earlier sessions were about AI helping us in our own work. Today is about what we will build for clients — and we are already working toward it, with many client proposals underway in this area." Explicit line: "This direction concerns every team in this company — engineering, DevOps, QA, project management, design, HR and operations, communications — not only development."

## 2. The Evolution of Enterprise Technology (1 min)
Single timeline visual: manual processes → desktop applications → web applications → cloud & SaaS at scale → data & machine learning → AI agents. Narration: each phase changed how solutions are built, while the need for skilled people remained constant. Closing line: "In every one of these eras, it was never only programmers who made the shift work — it was testers, analysts, designers, and operations adapting alongside them."

## 3. Industry Outlook (1 min)
- Gartner: 40% of enterprise applications will integrate task-specific AI agents by end of 2026, up from less than 5% in 2025.
- McKinsey: 62% of organizations are experimenting with AI agents, yet fewer than 10% have scaled agents in any single business function — the gap between experimenting and delivering is where clients need a capable partner.

## 4. What Actually Goes Into an AI Agent (2 min)
An AI agent is a system, not just a model — with roles attached to each component:
- **Model:** the reasoning engine
- **Tools:** APIs, databases, and services it acts through *(integration — engineering work)*
- **Context & memory:** the knowledge it draws on *(clean data, well-defined workflows — BA/PM territory)*
- **Orchestration:** the loop that plans, acts, and checks results *(runs on infrastructure DevOps manages)*
- **Guardrails:** permissions, validation, human approval points *(QA and design own much of this)*

Key engineering shift: agents don't behave identically every time, so quality work shifts from "does it pass the test" to "is it accurate, consistent, and safe across many scenarios." Key message: the model is a small part; most of the work is engineering, quality, and judgement.

## 5. AI Agents and the Enterprise Foundation (1.5 min)
Reference stack: Data → Enterprise applications & APIs → Integration layer → Agent orchestration → User interfaces. Agents depend on clean data, well-designed APIs, secure authentication, and reliable infrastructure. The systems our teams build and maintain today are prerequisites for every agentic solution.

## 6. Standardization of AI Integration (1 min)
The Model Context Protocol (MCP) has become the common standard for connecting agents to tools and data, now governed by the Linux Foundation with backing from major technology companies. Existing APIs can be exposed to agents through standard interfaces, reducing custom integration effort and shifting focus toward business logic.

## 7. Common Architecture Patterns (1 min)
Name the five patterns: RAG pipelines, single-agent workflows, multi-agent orchestration, human-in-the-loop, and AI pipelines. Headline: "Five patterns dominate client demand." Framing: "These are the patterns dominating client demand across the industry." [pause] before the direction slide.

## 8. Our Strategic Direction (45 sec)
Headline: "We're building toward agentic solutions for clients." Supporting line: many client proposals already in progress; an expansion, not a replacement. Client interest in agentic solutions and AI pipelines is increasing, and we are already working on many client proposals in this area. The company is aligning its capabilities and future engagements accordingly, with continued full commitment to current projects and clients.

## 9a. Every Role Has a Place in This (2 min)
Headline: "What you do today is exactly what agent projects need." Technical delivery roles, each ~20–25 seconds:
- **Developers & architects:** Stays: API design, integration, data modeling, cloud. Grows: context engineering, agent evaluation, observability for AI systems.
- **DevOps:** Stays: CI/CD, infrastructure as code, monitoring, reliability. Grows: deploying and versioning agent systems, tracing agent behavior in production, managing model costs, securing what agents are permitted to do. Line: "Agentic systems are operationally heavier than traditional apps. Our DevOps capability is a competitive advantage here, not a support function."
- **QA:** Stays: test discipline, edge-case thinking. Grows: evaluation design for systems that don't behave identically every run. Line: "A deterministic app fails loudly; an agent fails plausibly. Catching that is a skill the whole industry is short on."
- **Project managers & BAs:** Stays: requirements, workflow mapping. Grows: defining what the agent does, where humans approve, and what "done correctly" means.
- **UI/UX & design:** Stays: user understanding. Grows: conversational flows, approval screens, transparency cues — an open frontier with few established conventions.

## 9b. And Beyond Delivery (2 min)
- **HR & operations:** Building capability for client agent work at this scale is an HR program — this team runs it. Line: "The transition we're describing today is, in large part, a program HR and operations will lead."
- **Communications:** Internally: keeping everyone informed as the transition progresses. Externally: positioning our AI capabilities credibly, without hype. Their judgement about tone and accuracy becomes more valuable as generated content floods the market.
- **Finance & administration:** Agent systems carry running costs (model usage) that traditional projects do not — a growing role in tracking AI usage costs across projects.

## 10. A Measured Approach (1.5 min)
Personal line: "I will admit — the pace of change in AI is overwhelming for me as well." Mastery of every tool is not the objective. Most agentic initiatives remain early-stage; Gartner expects over 40% of agentic AI projects to be canceled by 2027 due to unclear value and insufficient controls. The company will take on agent projects only where the value is clear and the controls are in place, prioritizing reliability over novelty and protecting our people from burnout.

## 11. Implementation Plan (1 min)
- Shortlist a small number of agent frameworks based on production readiness, integration support (including MCP), observability, and community maturity
- Establish reference architectures and reusable components from our first agent projects
- Expand the portfolio progressively as delivery experience grows

## 12. Supporting Our People (1 min)
- Dedicated learning time and structured upskilling paths, open to all departments
- Sharing what we learn — reference architectures and lessons from our agent proposals and projects — across every team
- Pathways to contribute to AI initiatives alongside current responsibilities
- Recognition of what we learn along the way, not only project launches
- Follow-up note: "Each department lead will follow up with specifics for their team."

## 13. Closing Statement (30 sec)
"The direction is clear, and the pace will be deliberate. The work every team does today is the foundation of what comes next. From using AI to building it — we will build the next chapter together."

---

# PART 2: SPEAKER SCRIPT

*Delivery notes: Speak at a calm, deliberate pace — roughly 130 words per minute. Pause markers [pause] indicate 2–3 seconds of silence. Total spoken time: approximately 15 minutes.*

---

## Slide 1 — Purpose of Today's Address

Good afternoon, everyone. Thank you for being here.

Today, on behalf of our leadership, I want to share where our company is heading as the technology landscape around us evolves — and what that direction means for our teams and the work we do every day.

In earlier sessions, we talked about how AI can help us in our own work. Today is different. Today is about what we will build for clients — and we are already working toward it, with many client proposals underway in this area.

Before I go further, let me say one thing clearly: this direction concerns every team in this company — engineering, DevOps, QA, project management, design, HR and operations, communications. This is not a development-team announcement. It is a company direction, and everyone in this room is part of it.

[pause]

## Slide 2 — The Evolution of Enterprise Technology

Let's start with some perspective.

Over the past decades, enterprise technology has moved through distinct eras. Companies first automated manual work with software. Desktop applications gave way to web applications. Then came cloud, SaaS, and the era of scale. In recent years, data and machine learning took center stage. And now, we are entering the era of AI agents.

Here is what matters about this timeline: each era changed *how* solutions were built. None of them changed *whether* skilled people were needed.

And in every one of these eras, it was never only programmers who made the shift work. It was testers, analysts, designers, and operations teams adapting alongside them.

[pause]

## Slide 3 — Industry Outlook

This shift is not speculation. Let me share two numbers from independent research.

Gartner projects that by the end of 2026, forty percent of enterprise applications will integrate task-specific AI agents. That is up from less than five percent in 2025.

McKinsey's latest global survey found that sixty-two percent of organizations are experimenting with AI agents — yet fewer than ten percent have scaled agents in any single business function.

That gap between experimenting and delivering is exactly where clients need a partner who can build these systems properly.

The direction of the industry is clear. The question for us is not whether this shift happens — it is how we position ourselves within it.

[pause]

## Slide 4 — What Actually Goes Into an AI Agent

So what is an AI agent, really? I want to demystify this, because an AI agent is a system — not just a model.

It has five parts.

First, the **model** — the reasoning engine that interprets a goal and decides what to do next.

Second, **tools** — the APIs, databases, and services the agent acts through. Connecting these is integration work — our engineering bread and butter.

Third, **context and memory** — the knowledge the agent draws on. That requires clean data and well-defined workflows, which is exactly the territory of our analysts and project managers.

Fourth, **orchestration** — the loop that plans, acts, and checks its own results. And all of it runs on infrastructure our DevOps team manages.

Fifth, **guardrails** — permissions, validation, and human approval points. Our QA and design teams own much of this.

There is one engineering shift worth stating simply. Unlike traditional software, agents do not behave identically every time. So quality work moves from asking "does it pass the test" to asking "is it accurate, consistent, and safe across many scenarios."

The takeaway: the model is a small part of an agent. Most of the work is engineering, quality, and judgement — and that is what this company does.

[pause]

## Slide 5 — AI Agents and the Enterprise Foundation

Now, where do agents sit relative to the systems we build today?

Think of it as a stack. At the base: data. Above that: enterprise applications and APIs. Then the integration layer. Then agent orchestration. And at the top: user interfaces.

Agents depend on clean data, well-designed APIs, secure authentication, and reliable infrastructure. They do not replace enterprise systems — they are built on top of them.

Which means the systems our teams build and maintain today are not becoming obsolete. They are prerequisites for every agentic solution.

[pause]

## Slide 6 — Standardization of AI Integration

Something important happened recently that makes this transition more practical.

The industry has converged on a common standard for connecting AI agents to tools and data — the Model Context Protocol, or MCP. It is now governed by the Linux Foundation, with backing from the major technology companies, including direct competitors who rarely agree on anything.

What this means in practice: the APIs we already build can be exposed to agents through standard interfaces. Custom integration effort goes down. And the focus shifts to where it should be — solving the client's business problem.

## Slide 7 — Common Architecture Patterns

Across the industry, a handful of architecture patterns now dominate: retrieval-augmented pipelines, single-agent workflows, multi-agent orchestration, human-in-the-loop systems, and AI pipelines.

These are the patterns dominating client demand across the industry.

[pause]

## Slide 8 — Our Strategic Direction

Which brings me to our own direction. We are building toward agentic solutions for clients.

Client interest in agentic solutions and AI pipelines is increasing, and we are seeing it in our own conversations. This is not a plan for someday — we are already working toward it, with many client proposals in this area. The company is aligning its capabilities and future engagements toward this area.

And let me be equally clear about the other half of that sentence: we remain fully committed to our current projects and our current clients. This is an expansion of what we do — not a replacement.

[pause]

## Slide 9a — Every Role Has a Place in This

Now — what does this mean for each of you? Agent projects need every one of these teams. Let me go team by team.

**Developers and architects.** Your API design, integration, data modeling, and cloud skills carry forward directly. What grows on top: context engineering, agent evaluation, and observability for AI systems.

**DevOps.** Your CI/CD, infrastructure, monitoring, and reliability work stays central. What grows: deploying and versioning agent systems, tracing agent behavior in production, managing model costs, and securing what agents are permitted to do. I will say this plainly: agentic systems are operationally heavier than traditional applications. Our DevOps capability is a competitive advantage here — not a support function.

**QA.** Your test discipline and edge-case thinking stay essential. What grows: evaluation design for systems that do not behave the same way every run. A deterministic app fails loudly. An agent fails plausibly. Catching that is a skill the whole industry is short on — and it makes QA more critical in this era, not less.

**Project managers and business analysts.** Requirements, workflow mapping, stakeholder translation — all of it carries forward. Agent projects succeed or fail on process definition: what the agent does, where humans approve, and what "done correctly" means. That is your work at its core.

**UI/UX and design.** Your understanding of users stays fundamental. What grows: conversational flows, approval screens, transparency cues — an open frontier with very few established conventions. Our designers get to help define them.

[pause]

## Slide 9b — And Beyond Delivery

And beyond the delivery teams.

**HR and operations.** Building capability for client agent work at this scale is an HR program, not a side activity — and this team runs it. The transition we are describing today is, in large part, a program HR and operations will lead.

**Communications.** How this direction is explained — to our own people, to clients, and externally — shapes whether it lands as opportunity or confusion. Internally, this team keeps everyone informed as the transition progresses. Externally, they position our capabilities credibly, without hype. And as generated content floods the market, their judgement about tone and accuracy becomes more valuable, not less.

**Finance and administration.** Agent systems carry running costs — model usage — that traditional projects do not. Finance takes on a growing role in tracking AI usage costs across our projects.

[pause]

## Slide 10 — A Measured Approach

Now I want to be honest with you about something.

I will admit — the pace of change in AI is overwhelming for me as well. New models, new frameworks, new announcements every week. If you feel that, you are not behind. You are simply paying attention.

Here is the good news: mastery of every tool is not the objective. Domain knowledge and integration skills matter more than ever — and those are built over years, not weekends.

The industry data supports a careful pace. Most agentic initiatives out there remain early-stage, and Gartner expects over forty percent of agentic AI projects to be canceled by 2027 — due to unclear value and insufficient controls.

So our principle is this: we take on agent projects where the value is clear and the controls are in place. We prioritize reliability over novelty. And we protect our people from burnout. Chasing every trend is not a strategy — it is a risk.

[pause]

## Slide 11 — Implementation Plan

Practically, here is how we proceed.

We will shortlist a small number of agent frameworks — selected on production readiness, integration support including MCP, observability, and community maturity.

From our first agent projects, we will establish reference architectures and reusable components.

And we will expand the portfolio progressively, as our delivery experience grows. Depth before breadth.

## Slide 12 — Supporting Our People

None of this works without investing in you.

We will provide dedicated learning time and structured upskilling paths — open to all departments. We will share what we learn — reference architectures and lessons from our agent proposals and projects — across every team. There will be pathways to contribute to AI initiatives alongside your current responsibilities.

And we will recognize what we learn along the way — not only project launches.

Each department lead will follow up with specifics for their team in the coming weeks.

[pause]

## Slide 13 — Closing Statement

Let me close with this.

The direction is clear, and the pace will be deliberate. The work every team does today is the foundation of what comes next.

From using AI to building it — we will build the next chapter together.

Thank you.

---

# APPENDIX: Source References for Stats

## Gartner
- **Claim:** 40% of enterprise applications will integrate task-specific AI agents by end of 2026, up from less than 5% in 2025; agentic AI projected at ~30% of enterprise application software revenue by 2035 (best case).
- **Source:** Gartner press release, August 2025.
- **Link:** https://www.gartner.com/en/newsroom/press-releases/2025-08-26-gartner-predicts-40-percent-of-enterprise-apps-will-feature-task-specific-ai-agents-by-2026-up-from-less-than-5-percent-in-2025

- **Claim:** Over 40% of agentic AI projects will be canceled by end of 2027 due to escalating costs, unclear business value, and inadequate risk controls.
- **Source:** Gartner press release, 2025.
- **Link:** https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027

## McKinsey
- **Claim:** 88% of organizations use AI in at least one business function (up from 78% in 2024); 62% are at least experimenting with AI agents; 23% are scaling an agentic system; fewer than 10% have scaled agents in any single function.
- **Source:** McKinsey, "The State of AI in 2025: Agents, innovation, and transformation," November 2025.
- **Link:** https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai

## Model Context Protocol / Linux Foundation
- **Claim:** MCP donated to the Linux Foundation's Agentic AI Foundation in December 2025, with backing from major technology companies including OpenAI, Google, Microsoft, AWS, Cloudflare, and Bloomberg; adopted as the common standard for connecting AI agents to tools and data.
- **Source:** Linux Foundation / Agentic AI Foundation announcement, December 2025.
- **Link:** https://modelcontextprotocol.io
- **Background:** https://en.wikipedia.org/wiki/Model_Context_Protocol

---

*Note: Verify all links are live before publishing or distributing internally, as press release URLs occasionally change. If a link breaks, searching the claim text plus the source name will locate the current page.*
