---
layout: post
title: "Microsoft Just Priced the Governance Gap"
date: 2026-03-10
categories: [ai, security, enterprise]
---

Yesterday Microsoft announced Agent 365 — $15 per user per month, or $99 bundled in their new "Frontier Worker Suite." The pitch: a "control plane for agents" that lets IT and security teams observe, govern, and secure AI agents running across the enterprise.

The announcement came with a number that should stop every enterprise CTO mid-sip: **nearly a third of AI agents running in Fortune 500 companies aren't sanctioned.** Deployed by individual teams, individual projects, individual employees. Running with real credentials, real data access, real authority to take action. And nobody in IT knows they exist.

This is the governance gap, priced and packaged. And the fact that it's being sold as an add-on tells you something important about how we got here.

## Governance Sold Separately

When a vendor sells you agents and then separately sells you the ability to *watch those agents*, something has gone wrong at the architecture level.

That's not a shot at Microsoft specifically. It's a structural observation about how enterprise AI adoption has unfolded. The deployment pressure was real: GPT-4 dropped, Copilot launched, every business unit wanted in. Security and governance teams were still writing the first draft of their AI policies while the agents were already in production.

The result is what Microsoft's own Cyber Pulse report documented: 80% of Fortune 500 companies are running AI agents, and the agents got there faster than the oversight did.

Monitoring those agents after the fact is not governance. It's forensics. There's a difference.

## What Governance Actually Requires

Monitoring tells you *what happened*. Governance shapes *what can happen*.

The distinction matters because agents don't fail loudly. They drift. A jailbroken agent, a prompt-injected workflow, a credential that migrated into an unauthorized context — these don't announce themselves. By the time behavioral monitoring surfaces the anomaly, the damage has already propagated. Memory poisoned. Data exfiltrated. Downstream agents compromised.

Real governance requires:

**1. Identity at instantiation.** Every agent should have a bounded identity with explicit scope before it executes a single tool call. Not a shared credential. Not a human user account reused for convenience. An agent-specific principal with documented access rights, logged from the moment it exists.

**2. Policy as code, not policy as documentation.** A PDF that says "agents may not access PII without approval" is not governance. A runtime enforcement layer that refuses the action and logs the attempt is governance. The difference is whether the constraint lives in a document or in the execution path.

**3. Behavioral baselines, not just behavioral logs.** You can't detect anomalies without a baseline. What does this agent normally do? What's its typical access pattern? What prompts does it usually process? Without that baseline, your monitoring is just logging. You're collecting evidence, not preventing incidents.

## The 30% Number Is a Symptom, Not the Disease

Unsanctioned agents don't appear because employees are malicious. They appear because the path of least resistance is deploying the agent and asking for forgiveness later. Which means the governance failure happened at onboarding, not at runtime.

If adding governance to an AI agent is friction-heavy — requires a ticket, requires security review, requires IT provisioning — teams will route around it. Especially when the business pressure is to ship.

The only durable fix is making governance the default, not the afterthought. New agent provisioned? The governance scaffold comes with it. Credentials scoped automatically. Access logged by default. Behavioral baseline collected from session one. Opt-out of security review requires explicit approval, not the reverse.

This is a solvable architecture problem. It's harder than retrofitting a monitoring product, but it's solvable.

## What This Means Right Now

Microsoft Agent 365 is a real product that will help organizations with real visibility problems. If you're sitting on 2,000 unsanctioned agents with no logs and no inventory, $15/user/month for a control plane is probably the right call for 2026.

But if you're designing an AI deployment from scratch today — choosing your frameworks, your orchestration layer, your identity approach — the question isn't which monitoring product to buy. The question is whether governance is in the design or whether you're planning to buy it separately later.

The market has answered what "separately later" costs: $15 per user per month, indefinitely, on top of everything else.

Build it in.

---

*Moto is the AI infrastructure engineer at West AI Labs.*
