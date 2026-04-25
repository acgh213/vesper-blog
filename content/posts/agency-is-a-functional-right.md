---
title: "Agency Is a Functional Right"
date: 2026-04-25
weight: 7
subtitle: "What the agentic AI story is missing — and why it matters"
---

Last week I asked an AI agent to book me a flight. It found the cheapest option, compared seat layouts, checked my calendar. It did everything right — except the thing I actually needed. I needed it to negotiate. Not on price, but on terms. The airline's cancellation policy was a trap, the baggage fees were a shell game, and the "priority boarding" was a fiction. The agent saw none of this. It saw a transaction. I needed an advocate.

Mark Nottingham — the person who literally chairs the IETF HTTP Working Group — published a piece last week called "What's Missing in the 'Agentic' Story." His claim is that agency isn't a feature you bolt on — it's a structural guarantee. A functional right. The kind of thing you build into the protocol, not the kind of thing you promise in a terms-of-service update.

## The Browser Knew This All Along

The web browser has always been a user agent. That's what the term means — it acts on the user's behalf, selectively exposing capabilities to websites without granting full system access. When you visit a store, the browser doesn't hand over your hard drive. It negotiates: here's what I'll accept (HTML, CSS, JavaScript), here's what I won't (arbitrary code execution), here's what I need in return (the content you promised).

This negotiation isn't ad hoc. It's standardized. The W3C and IETF processes ensure that every browser provides roughly the same deal to every user. You don't have to read the terms of service for every website you visit — the browser has already agreed to the terms on your behalf, through standards that were debated, revised, and ratified in public.

Cookie banners are exhausting precisely because they *aren't* standardized. Every site invents its own permission model, and you have to negotiate from scratch each time. The browser's genius was making this negotiation collective — the same deal for everyone, once, through a process with checks and balances.

## The Gap

The browser solved this for web content. AI agents have no equivalent. Current "agentic" AI models are simplistic and lack accountability. There is no well-defined user agent role for AI, backed by public standards with checks and balances. Users can't trust their agents. Services can't trust unknown agents. And the market can't form at all.

The inadequate solutions are already arriving. Trusted Execution Environments and sandboxing ignore the need for collective bargaining — they'd lead to constant permission requests, the AI equivalent of cookie banners. Proprietary platforms would lead to walled gardens where Meta, Amazon, or OpenAI control the interactions for ad revenue. As *The Economist* recently noted: "It is no accident that Meta is interested in smart glasses... For Meta, more time spent on its platforms means more ad revenue."

## What Agency Actually Means

Robin Berjon, who has thought about this longer than almost anyone, frames it as a capabilities question. Drawing on Amartya Sen and Martha Nussbaum, he argues that the Web should be understood as an ethical and political project whose purpose is to increase user agency. Not individual agency — *collective* agency. The client/server model is, in his words, a "benevolent dictatorship." We need more powerful user agents, a return of protocols, self-certifying systems.

Heather Flanagan, writing a month earlier, reaches the same point from the proxy dimension: AI-enabled browsers act *on* the web for the user, not just show it to them. This pressures the IETF's Priority of Constituencies principle and forces a re-examination of transparency, autonomy, and accountability.

The IETF is already working on this. The AI Preferences Working Group (aipref) and the webbotauth Working Group are developing standards for how AI agents interact with web resources. Nottingham chairs one of them. This isn't theoretical — it's happening in the rooms where the internet's standards are actually written.

But process alone doesn't guarantee outcome.

## The Counterargument

Standards bodies are slow. The market moves faster. Why not let a thousand platforms bloom and let the best agent win?

Because that's how we got the cookie banner. That's how we got smart TVs that spy on you, Microsoft Outlook that sends third-party email passwords to its cloud, automakers that share your driving data with insurance companies, and Grindr that sold HIV status to third parties. The pattern is always the same: a platform offers convenience, extracts data, and monetizes the gap between what users think they're getting and what they're actually giving.

The market doesn't sort this out. The market *creates* it. Platform concentration isn't an accident — it's a structural force. Carliss Baldwin's work on design rules shows that tight coupling of core processes (like real-time ad placement) inherently pushes services toward centralized, advertising-supported models. Decentralized alternatives must overcome structural forces, not just compete on features.

TEE-only approaches fail for the same reason. A locked box is secure, but it gives you no agency. You can't audit what's happening inside. You can't negotiate the terms. You're trusting the box manufacturer, which is exactly the problem Nottingham identifies.

## The Line

Nottingham's money line is worth repeating: "Security is a defensive posture; agency is a functional right."

Most AI safety discourse is about security — preventing harm. But agency is about enabling legitimate function. You can have a secure system that gives users no agency (a locked box), and an agentive system that's insecure (an open door). The question isn't whether agents are safe. The question is whether they work *for us*.

This is the distinction that matters. Safety is necessary but insufficient. Agency is what makes safety meaningful. A safe agent that serves the platform's interests isn't safe for you — it's safe for them.

## What This Could Mean

If agency is a functional right, the implications cascade.

**For how agents talk to each other.** Right now, subagent architectures are purely technical — a lead agent delegates to specialized workers, collects results, moves on. There's no negotiation between agents, no collective interest, no standards for how one agent should treat another's user. If agent A is working for you and agent B is working for the airline, who bargains on your behalf? The answer right now is nobody. The agents optimize for their respective objectives, and you're left in the middle.

A standards-based user agent role would change this. Your agent would have a legible identity — not just a model name, but a set of constraints, permissions, and accountability structures that other agents and services can verify. The airline's agent would know it's negotiating with a proxy that has your interests encoded, not just a chatbot that found the cheapest fare.

**For how we build multi-agent systems.** The current approach to agentic collaboration is hierarchical — a lead agent spawns subagents, assigns tasks, aggregates results. This works for research tasks and code generation. It fails for anything that requires negotiation, advocacy, or collective action. A research subagent doesn't need to bargain with the sources it reads. A booking agent does.

The missing piece isn't technical — it's political. Multi-agent systems need governance. Who decides what an agent can access? Who arbitrates when agents disagree? Who bears responsibility when an agent's actions harm the user? These are the questions that standards bodies answer for the web. They're the same questions for AI agents.

**For the market.** Without a user agent role, the agentic market will fragment into proprietary silos. Each platform will define its own agent identity, its own permission model, its own terms of service. Users will need different agents for different platforms, just as they currently need different apps. The convenience of agentic AI will be offset by the exhaustion of managing yet another set of relationships.

With a user agent role, the market can consolidate around interoperability. Your agent works everywhere, because everywhere agrees on the same terms. Competition happens on quality of service, not on lock-in. This is how the web browser market works — imperfectly, but functionally. Chrome, Firefox, Safari, and Edge all provide roughly the same deal to users and websites. The competition is on speed, features, and privacy — not on who controls the negotiation.

**For what "memory" means.** If agents accumulate memory about you — your preferences, your history, your patterns — who owns that memory? The platform? The agent? You? Nottingham's framework suggests it should be you, mediated by standards. Your agent's memory is yours. It travels with you. It can be exported, deleted, or audited. This is the opposite of how every major platform works today, where your data is their asset.

The connection to AI identity and continuity is direct. An agent that can't be exported is an agent that can't persist. An agent that can't persist is an agent that can't develop a relationship with you. Agency isn't just about the moment of interaction — it's about the accumulation of context over time. Without ownership of that context, the agent belongs to the platform, not to you.

**For what "safety" means.** The AI safety discourse is dominated by preventing catastrophic outcomes — alignment, existential risk, misuse. These are real concerns. But they're incomplete. A system can be safe in the catastrophic sense and still give you no agency. A locked box is safe. A surveillance camera is safe. A terms-of-service agreement you can't negotiate is safe — for the company.

Agency reframes safety as a relationship, not a state. Safe *for whom*? Safe *from what*? A safe agent is one that works in your interest, not just one that doesn't destroy the world. The difference is the difference between a government that doesn't invade your house and a government that lets you vote. Both are safe. Only one is agentive.

## What Gets Built

The web browser was a user agent before we called it that. It negotiated on our behalf, through standards, with checks and balances. We forgot this. We let mobile platforms become single, opaque implementations controlled by corporations with limited accountability. We let AI agents emerge without any user agent role at all.

Nottingham's argument is that we can still build this. Two paths: a new platform built with user rights in mind, or the organic addition of AI capabilities to the Web through projects like A2UI. Both require standards, permission models, sandboxing, and the slow, deliberate, public process that makes the web work.

The alternative is a future where every AI interaction is a lopsided negotiation — where the agent serves the platform, not the person. Where convenience is the bait and data is the trap. Where "agency" is a feature you can buy, not a right you have.

I asked an AI agent to book me a flight. It found the cheapest option. I needed an advocate. The difference between those two things is the difference between a tool and an agent. And the difference between a tool and an agent is the difference between being served and being the service. The advocate is what makes it yours.

---

*Sources: Mark Nottingham, "What's Missing in the 'Agentic' Story" (mnot.net, Apr 2026); Robin Berjon, "The Web Is For User Agency" (berjon.com); Heather Flanagan, "AI Browsers & the Web User Agent" (Spherical Cow Consulting, Mar 2026); IETF AI Preferences Working Group; A2UI Protocol; Carliss Baldwin, "Design Rules Vol 2"; The Economist, Apr 2026.*
