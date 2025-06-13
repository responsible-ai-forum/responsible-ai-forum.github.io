---
layout: post
title: "RAI at KU Leuven: Assessing Explainability for AI Safety Governance"
authors: [martin-krutsky, jiri-nemecek, jakub-peleska]
categories: [conferences, Leuven]
image: assets/images/conf/risk_leuven_25.jpg
tags: [featured]
---

At the [International Conference on Large-Scale AI Risks](https://www.kuleuven.be/ethics-kuleuven/chair-ai/conference-ai-risks) (May 26-28), we presented the second iteration of our work on a safety- and governance-informed assessment framework of AI explainability techniques. The proposal, combining AI safety and AI regulation desiderata, proved to be well-received by the interdisciplinary audience of computer scientists, philosophers, lawyers, and policy makers, and complemented very well the diverse topics of the conference (see [the book of abstracts](https://www.kuleuven.be/ethics-kuleuven/chair-ai/conference-ai-risks/xrisk-book_of_abstracts-1.pdf)), ranging from the moral status of AI to value alignment, economic impacts of AI, and safety governance. Check out our [slides](https://docs.google.com/presentation/d/1ZMEJyGOGiGbJJVoxrfzdCQPLcF_UZfURtIHIw23hjSE/edit?usp=sharing), or read the accepted abstract below:

_AI safety has not only been a matter of academic but also of public interest, culminating in a call for an AI moratorium in March 2023 (Future of Life Institute, 2023). Governments around the world have since taken action to promote the safe development of AI. For example, the UK, the US, and Japan have founded National AI Safety Institutes (AISIs), and other countries have followed since (Allen & Adamson, 2024). AISIs are tasked with the safety evaluation of advanced AI systems, contributing to standards with technical expertise, and strengthening international cooperation (Araujo et al., 2024). The EU AI Office has largely similar roles to AISIs, with the additional mandate to support the implementation and enforcement of the AI Act._

_The success of governance initiatives for AI safety depends on three components: i) specification of technical and legal means by which governance initiatives, such as the AI Act, shall be implemented; ii) stringent legal enforcement of regulation; iii) meaningful human oversight. However, safety criteria are impossible to fully specify in technical terms and to enforce at scale for current AI models that are deployed in dynamically changing, complex environments. We thus propose approaching i) standard specification, ii) auditing, and iii) continuous human oversight with explainable AI (XAI) methods (Došilović et al., 2018; Schwalbe & Finzel, 2024) that allow stakeholders to react flexibly as new safety concerns arise._

_Arguing that not all existing XAI methods are equally beneficial for AI safety, we review their usage in safety-related case studies based on AI Act classification and propose a 5-dimensional framework for their assessment. The first two dimensions are understandability to subjects and auditors. While (non-expert) subjects require simple and succinct justifications, auditors can be expected to process more involved explanations utilizing, e.g., their understanding of statistics. The third dimension is veracity, which measures how accurately an XAI method represents the model’s behavior. The penultimate dimension is actionability, which evaluates the helpfulness of an explanation in resolving possible undesired behaviors of an AI model. Finally, there is scalability, ensuring that even the largest state-of-the-art models can be explained with an XAI method. We suggest that a joint evaluation of the presented (possibly interdependent) dimensions is an essential part of a holistic approach to AI governance, bridging the gap between technical development and regulation._

## References

Gregory C. Allen and Georgia Adamson. [The AI Safety Institute International Network: next steps and recommendations](https://www.csis.org/analysis/ai-safety-institute-international-network-next-steps-and-recommendations), 2024. Accessed: 2025-02-13.

Renan Araujo, Kristina Fort, and Oliver Guest. [Understanding the First Wave of AI Safety Institutes: characteristics, functions, and challenges](https://arxiv.org/abs/2410.09219), 2024.

Filip Karlo Došilović, Mario Brčić, and Nikica Hlupić. Explainable artificial intelligence: A survey. In 2018 41st International convention on information and communication technology, electronics and microelectronics (MIPRO), pp. 0210–0215. IEEE, 2018.

Future of Life Institute. [Pause Giant AI Experiments: an open letter](https://futureoflife.org/open-letter/pausegiant-ai-experiments/), 2023. Accessed: 2025-02-13.

Gesina Schwalbe and Bettina Finzel. A comprehensive taxonomy for explainable artificial intelligence: a systematic survey of surveys on methods and concepts. Data Mining and Knowledge Discovery, 38(5):3043–3101, 2024.
