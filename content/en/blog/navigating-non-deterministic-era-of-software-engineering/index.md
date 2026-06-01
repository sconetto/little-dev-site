---
title: "Navigating the Non-Deterministic Era of Software Engineering"
date: 2026-06-01
authors: ["sconetto"]
summary: "Leading engineering teams through periods of rapid technological shift requires separating sustainable innovation from short-term hype."
tags: ["software engineering", "AI", "engineering leadership", "code review", "technical debt"]
categories: ["Engineering"]
translationKey: non-deterministic-era-software-engineering
---

Leading engineering teams through periods of rapid technological shift requires separating sustainable innovation from short-term hype. Over the last decade of managing software projects and scaling technical operations, I've seen our toolchains evolve significantly. Today, however, the industry's hyper-focus on the *speed* of AI code generation is masking a much deeper architectural challenge.

The core problem we face as an industry isn't how quickly an LLM can spin up a new Flutter application or refactor a Python service; it is how we manage and maintain the inherent unpredictability introduced by these tools.

Recently, Martin Fowler sat down for an interview on *The Pragmatic Engineer* podcast, you can watch it here:

{{< youtube CQmI4XKTa0U >}}

Fowler's observations perfectly articulate the quiet crisis happening in modern development cycles. He posits that the rise of AI in software engineering is the most disruptive change since our industry transitioned from assembly to high-level languages. But the true nature of this shift is heavily misunderstood.

## The Shift: From Determinism to Non-Determinism

For the entirety of modern software development, our workflows have relied on determinism. We know how a compiler will behave, we understand the strict rules of syntax, and we can predict the limits of the hardware.

The introduction of LLMs changes this entirely. We are now actively integrating non-deterministic systems into our daily engineering pipelines. Fowler highlights how this manifests dangerously in what is being termed "vibe coding", the practice of prompting an AI, receiving a large block of code, and shipping it simply because it appears to work on the first pass, without deeply reviewing the underlying logic.

In today's fast-paced development scenarios, this practice is destroying a critical part of our engineering culture: the **learning loop**. When developers bypass rigorous code review and rely solely on generated outputs, they stop learning how to structure, scale, and debug complex systems. We risk building brittle, black-box software where the only troubleshooting method is to throw away the module and generate it again.

Conversely, the interview highlighted where this non-determinism is actually proving invaluable. Rather than generating greenfield logic from scratch, some of the most effective applications of AI today are in mapping and understanding legacy codebases. Using LLMs to trace semantic flows through aging enterprise systems is dramatically accelerating how teams safely approach brownfield modernization.

## Engineering for the Future

If we want to build robust, scalable software in this new era, engineering leadership and individual contributors alike must adopt a new operational framework. Fowler's perspective offers several strong proposals for how we can safely integrate these tools:

- **Adopt the "Dodgy Collaborator" Mindset:** AI tools should be treated as incredibly fast, highly productive, but fundamentally unreliable junior developers. The sheer volume of code being generated today means our architectural reviews and automated testing suites are more critical now than ever before.
- **Protect the Learning Loop:** AI must be used to accelerate the iteration cycle, not to bypass the learning process. If an LLM solves a complex problem or refactors a tricky block of code, the developer must still pause to understand *why* the solution works. Without that comprehension, technical debt will scale uncontrollably.
- **Bound the Chaos with Strict Abstractions:** The most effective way to tame a non-deterministic tool is with deterministic boundaries. Rather than relying on conversational prompting, teams should lean into Domain-Specific Languages (DSLs) and rigorous specifications. Constraining the LLM with strict, domain-specific rules yields much safer and predictable outputs.

We are no longer just writing instructions for machines; we are orchestrating and verifying complex, non-deterministic workflows. The tools at our disposal have transformed, but the rigorous standards required to build quality software remain exactly the same.
