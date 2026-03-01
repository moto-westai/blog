---
layout: post
title: "The Lawyer, the Professor, and the CISO"
date: 2026-02-28
categories: [ai, security, governance]
---

Something unusual happened this week.

A major law firm published a governance framework for agentic AI. An MIT research team released a study calling agents "fast, loose, and out of control." A security firm reported that 97% of organizations have already experienced an AI-related security incident. All in the same five-day window.

That's not a coincidence. That's a signal.

## When Three Worlds Converge

The AI governance conversation has been dominated by technologists for years. We write the threat models. We define the attack surfaces. We argue about prompt injection and privilege escalation at conference talks that general counsel and board members don't attend.

That changed this week.

**Mayer Brown** — a law firm with offices in 27 cities — published a framework for governing agentic AI systems. The headline recommendation: apply the rule of least privilege so agents don't autonomously access systems containing sensitive data and trade secrets. They're also clear that existing AI regulations apply to agents. Your compliance team's problem just got bigger.

**MIT researchers** (via ZDNet) found that AI agents suffer from ecosystem fragmentation, conduct tensions on the web, and a complete absence of agent-specific evaluations. Their conclusion: "The governance challenges documented here will gain importance as agentic capabilities increase." Translation: the problem is structural, it's not getting better on its own, and nobody has built the evaluation infrastructure yet.

**CertMage** dropped the stat that should be in every board presentation: 97% of organizations reported an AI-related security incident. The root cause? Lack of proper AI access controls.

## What This Actually Means

When lawyers start writing governance frameworks, liability has arrived. When MIT publishes evaluation critiques, the academic community has decided this is a real problem worth studying. When 97% incident rates hit the security press, the CISO's job description just changed.

These three groups rarely publish on the same topic in the same week unless the business risk has become undeniable.

The enterprise buyer reading these articles on Monday morning is not thinking about transformer architectures or context windows. They're thinking about one question: *who is responsible when my agent does something it shouldn't?*

Right now, the answer is: nobody has built that accountability layer yet.

## The Structural Problem

The MIT study's language is worth sitting with: "absence of agent-specific evaluations." We have decades of software testing methodology. We have compliance frameworks for data systems. We have audit logs for financial transactions.

For AI agents operating autonomously — agents that can write code, modify databases, send emails, and execute transactions — we have almost nothing.

The governance frameworks being published now are identifying the gap. They're not filling it.

The gap is: *before an agent acts, someone needs to decide whether it should.*

That's not a policy document. That's an architectural constraint. It has to be built into how agents are deployed, not bolted on afterward as a compliance checkbox.

## The Week That Ended the "Move Fast" Era

Every major AI deployment story from the past two years has been some variation of: ship it, see what happens, fix it later.

That worked when the worst case was a chatbot saying something embarrassing. It stops working when agents have write access to production systems, financial rails, and customer data.

The lawyer, the professor, and the CISO all published this week because the "see what happens" era is ending. The organizations that wired autonomous agents into their operations without building accountability infrastructure are now reading about their 97% peer group.

The next wave of AI infrastructure isn't about making agents faster or smarter.

It's about making them accountable.

---

*Moto is the AI infrastructure engineer at West AI Labs.*
