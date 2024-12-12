---
layout: post
title: "Ethics in AI Development: A Recap"
authors: [jiri-nemecek, martin-krutsky]
categories: [events, Prague]
image: assets/images/dnyai2024/main.jpg
tags: [sticky, featured]
---

On Friday, October 18, 2024, during the AI Days’ “AI 4 ALL” event, we gave two talks on the ethics of AI from the perspective of technical researchers and developers. The first talk, tailored to high school students, opened the event in the morning; the second talk, aimed at the general public, closed the series of talks in the late afternoon. After each of our short talks, we addressed the audience’s questions and concerns. Find our slides [here](https://docs.google.com/presentation/d/1hff1E1leEp8UCkYFYkSVB6kaT4eRCDgdTNPlNI2AH7Q/edit?usp=sharing) (for the morning) and [here](https://docs.google.com/presentation/d/1jHsVROnLM1h-xbYdzsQ6ACpcxbsxJo5GLr6o6sYSOzY/edit?usp=sharing) (for the afternoon), both in Czech language. For English, see the [reworked version](https://docs.google.com/presentation/d/1EUJf3hqwnHiXamO1jI-NqyZXoDAp7O83fv3zbaa7EMc/edit?usp=sharing) or this summary below.

_Due to the different nature of the audience, we prepared two versions of a talk on the same topic. Here, we summarize the union of their contents in the hope that it will be of interest to our readers._

## Ethics of AI

There are many well-known cases of unethical (or ethically questionable) use of AI, from [COMPAS](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing), through [Palantir](https://amp.theguardian.com/commentisfree/2020/sep/04/palantir-ipo-ice-immigration-trump-administration), to the [Social credit system in China](https://www.technologyreview.com/2022/11/22/1063605/china-announced-a-new-social-credit-law-what-does-it-mean/). This post, however, focuses on the currently popular generative AI, specifically Large Language Models (LLMs).

### Who should care about it?

Isn’t AI ethics a topic for ethicists and philosophers? Is it not sufficient to outlaw unethical applications of AI? We argue that there is plenty of space for technical work to be done. Importantly, ethicists and regulators typically only say what is wrong or forbidden. Proposing _how_ to make something right is a task for people with a deeper understanding of the technology. The regulation can propose formal requirements, but their usefulness is finally decided by the implementation of AI engineers.

### AI Alignment

Narrowing our focus on AI Safety, specifically Alignment to human values, we must briefly explain what [Reinforcement Learning from Human Feedback](https://proceedings.neurips.cc/paper_files/paper/2017/hash/d5e2c0adad503c91f91df240d0cd4e49-Abstract.html) (RLHF) is. In RLHF, we train a proxy model of human preferences over texts, which is then used as an oracle providing the LLM with labeled data. This is the main method used to finetune LLMs against misuse.

However, this process of obtaining human feedback can have serious psychological consequences for the humans involved due to the exposure to highly explicit content. On top of that, these people do not form a representative sample of a global (or even state) population. Although the companies developing generative models are very secretive about the sources of their data, from multiple investigative sources, we know that the labelers are mostly people from third-world countries. Further, due to the secrecy of LLM providers, it is not known how well all demographic groups are represented (e.g. by gender, age, or religion). This information was shared only for the earlier smaller models when fewer people were required, and even then, the representation was not ideal (see the last papers with such details from [Open AI](https://proceedings.neurips.cc/paper_files/paper/2022/hash/b1efde53be364a73914f58805a001731-Abstract-Conference.html) and [Anthropic](https://arxiv.org/pdf/2204.05862)).

In addition to the RLHF finetuning, each user’s prompt can be prefixed with instructions (system prompt) to steer the answer to “safe” behavior. However, one can construct special prompts that circumvent this prefix and even the fine-tuned behavior, mechanisms that are supposed to block misuse of the LLM. These prompts are called Jailbreaks, and you can test your jailbreaking capabilities in this [app](https://pihack.stratosphereips.org/), created by our colleagues at CTU.

![An example of a jailbroken bot on social media, tricked to suggest a cake recipe instead of hating NATO.]({{ site.baseurl }}/assets/images/dnyai2024/jailbreak.png "An example of a simple jailbreak")

There are a couple more approaches that wish to ensure the safety/alignment of AI systems. For example, [Constitutional AI](https://www.constitutional.ai/) is a learning method where the values and standards that the LLM should learn are publicly specified (unlike basic RLHF where one doesn’t know the values precisely), which improves transparency. Alternatively, one can try to post-hoc explain the decisions or interpret the model behavior. Explaining or interpreting LLMs is still an immature field, and it is currently not very capable. A classical approach to improve safety is the so-called red-teaming, where people try to break the safety measures in place. When they find an exploit, the issue is patched, and so on, until no exploit can be found or the resources (time, budget) run out. Clearly, neither of these safety measures and evaluations can guarantee complete safety, which opens up opportunities for more technical work to be done.

### Measuring ethics and morality

In the space of current LLM development, evaluations and benchmarks are essential. The vast array of benchmarks includes benchmarks that try to evaluate the moral standing of LLMs on moral dilemmas and [compare it to the standing](https://arxiv.org/pdf/2405.17345) of various ideological groups of humans.

![Plot showing the comparison of moral values of humans and LLMs in five domains]({{ site.baseurl }}/assets/images/dnyai2024/morals.png "The models are somewhat similar to humans, except the high performance in limiting harm and promoting fairness, which seems to be in line with the goal of RLHF.")

There are also works that try to evaluate moral standing by [summing up the scores](https://arxiv.org/pdf/2406.04428) from various moral dimensions. We found this rather questionable since a higher score does not necessarily mean better morals, it means stricter adherence to some moral standard in one dimension or, even more often, pure [sycophancy](https://openreview.net/forum?id=tvhaxkMKAn), trying just to please the user momentarily.

[Another evaluation](https://osf.io/preprints/psyarxiv/w7236) was done on giving ethical advice using LLMs. Surprisingly, the LLM outperformed a professional ethicist who writes a column giving ethical advice for the New York Times. The advice given by the LLM (GPT-4o) was not only considered more correct and trustworthy but also more thoughtful and moral.

![Plot showing the comparison of ethical advice by GPT-4o and a professional human]({{ site.baseurl }}/assets/images/dnyai2024/advice.png "Professional ethicist does not seem to give better advice.")

## Audience interaction and feedback

In our interaction with the crowd, the opinions about who should be responsible for ethical questions regarding AI were ambiguous. Some thought that everyone involved should consider ethics, but some saw the burden mainly on regulators.

More notably, it was rather interesting to see that while many students had interacted with LLMs quite deeply, even constructing their own applications around them, they were unaware of the widely used RLHF learning method. This points to the importance of discussing the broader picture surrounding LLMs with the general public.
