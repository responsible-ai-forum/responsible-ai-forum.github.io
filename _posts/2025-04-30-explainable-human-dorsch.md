---
layout: post
title: "Explainable and Human-Grounded AI for Decision Support Systems"
authors: [jakub-peleska, martin-krutsky]
categories: [events, Prague]
image: assets/images/cetep/explain_human_dorsch.png
tags: [featured]
---


In a world increasingly shaped by algorithmic decisions, ensuring that artificial intelligence (AI) systems are explainable and trustworthy has never been more urgent. John Dorsch, a philosopher, AI ethicist, and postdoctoral researcher at CETE-P, argues that we've been looking at this the wrong way. In a recent presentation for our Responsible AI discussion group and his paper co-authored with Maximilian Moll, Dorsch introduces an original framework for understanding how AI can support, not replace, human judgment. The framework called the theory of epistemic quasi-partnerships (EQP) is grounded in a practical “RCC approach”, standing for: Reasons, Counterfactuals, and Confidence.

## The Problem: Explainability for Experts, Confusion for Users

Most AI explanations today are made by computer scientists for computer scientists. This leaves actual users facing complex visualizations and technical justifications that offer little meaningful insight. One of Dorsch’s central case studies involves AI decision support systems used by social workers to assess potential child abuse. These are scenarios where getting the decision right isn't just a matter of efficiency—it's a matter of life and safety.

Dorsch argues that AI outputs must go beyond numerical scores. They should include _reasons_, _counterfactuals_, and _justifications_ that align with the knowledge and reasoning styles of human users. For example, instead of just saying an intervention is recommended, the AI should explain: _What would have changed the recommendation? Which input mattered the most?_

Dorsch emphasizes the need for standardized metrics that evaluate explanation _quality_ from the user’s perspective, not just technical completeness. He also clarifies his stance on the often-misunderstood distinction between _interpretability_ (understanding of the model's inner workings) and _explainability_ (making decisions clear for end users). The latter can often be misleading or superficial, failing to serve the user's actual needs.


## Epistemic vs. Moral Trust

Dorsch emphasizes the importance of distinguishing between epistemic trust and moral trust. While people often speak of “trustworthy AI,” Dorsch warns against attributing moral agency to machines ("this AI is good"). AI can be _epistemically trustworthy_—reliable in the information it provides—but it is not a moral agent and should not be treated as such.

This distinction makes it clear that we shouldn't blindly follow AI just because it "seems confident." Instead, we should evaluate it as we do other information sources, much like we might trust a peer-reviewed article more than a social media post.


## Explanations and Human Psychology

Why do we explain things? According to cognitive psychology, explanations serve two primary purposes: helping us _predict_ behavior and _justify_ actions. Dorsch argues that AI explanations should do both. When an AI system justifies a recommendation, it helps foster trust—not just by being right, but by being _understandably_ right.

This is particularly important in domains like loan approval or legal sentencing, where users need context, not just outcomes. It's not enough to say "no loan approved"; people want to know _why_ and what might change that outcome in the future.


## AI as a Quasi-Partner—The RCC Approach

The central proposal of both the talk and the paper is the concept of AI as a _quasi-partner_ in decision-making. AI can process massive data sets and surface relevant insights, but lacks human judgment, ethical reasoning, and social accountability. In this sense, the AI can act _like a partner_, but cannot be a full one.

The goal, then, is not to replace human decision-makers, but to _augment_ them. To work effectively as a quasi-partner, AI must engage in sound epistemic practices—the same practices that humans use to build understanding and trust in one another’s decisions. These include:
- Providing Reasons: Clear, human-readable justifications for recommendations. John explores the nature of reasons, focusing on their stability and explanatory force, which allows for predictions in similar situations. He points out the absence of normative elements in this discussion, which complicates the understanding of what constitutes a reason.
- Exploring Counterfactuals: Explaining how a decision might change if key inputs were different. Dorsch introduces the concept of “nearby possible worlds.” This refers to small changes in circumstances that could alter outcomes—e.g., what if one more call had been made in a child welfare case? While powerful, this approach has limitations. How do we define what counts as “nearby”? And how do we know in advance what outcomes we’re aiming for? Dorsch acknowledges these challenges but argues that exploring such counterfactuals is essential for meaningful, human-grounded AI explanations.
- Stating Confidence: Offering calibrated measures of certainty to help users assess when to trust or challenge AI outputs. Here, we point out that offering a specific confidence value for each individual prediction is often not feasible, as most evaluation metrics—such as accuracy, F1 score, or ROC AUC—are calculated at a global level rather than on a per-instance basis.

This forms the Reasons, Counterfactuals, and Confidence (RCC) approach, a structured way to design AI explanations that align with human reasoning. We advocate for the inclusion of a _fidelity condition_ in AI explanation frameworks, ensuring that explanations genuinely reflect the model's actual reasoning, rather than generic or overly simplified interpretations.

## What the Research Shows

Dorsch’s theory is backed by empirical studies in explainable AI. Several key findings include:
- Confidence Works—But With Limits: Users tend to trust AI more when it states how confident it is. But this can lead to overreliance unless paired with other forms of explanation.
- Counterfactuals Enhance Understanding: Showing how slight changes in input would alter the outcome helps users grasp the logic behind a decision.
- Example-Based Justifications Reduce Bias: Prototype explanations—like “this case is similar to that one”—help users think critically rather than blindly defer to the AI.

- Crucially, methods like bar charts (feature graphs) often fail because they require additional technical interpretation. In contrast, explanations that resemble natural human reasoning—statements like “If X, then Y”—are more effective.


## Final Thoughts

As AI regulations like the EU AI Act push for transparency in “high-risk” systems, we urgently need ways to design AI explanations that non-experts can use responsibly. Dorsch’s EQP theory provides both ethical and practical guidance. It avoids the pitfall of anthropomorphizing AI—pretending it's human—and instead focuses on building useful, transparent partnerships between people and machines.
