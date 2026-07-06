---
title: "When AI Learns Human Bias: Lessons from Amazon’s AI Recruiting Tool "
date: 2026-06-26
draft: false
github_link: "https://github.com/Ashana-Smith/Ashana-Smith"
author: "Ashana S."
tags:
  - AI Ethics
  - Hiring Algorithms
  - Fairness in AI
  - Amazon Case Study
  - Algorithimic Bias
image: /images/resume.png
description: "A look at how Amazon's AI hiring tool absorbed human bias and what it teaches us about fair automation."
toc: 
---

# When AI Learns to Discriminate: A Framework for Getting It Right

Amazon spent years building an AI tool to automate hiring. By 2017, the company had quietly shut it down. The reason: the system had taught itself that men made better candidates.

This wasn't a glitch. It was the predictable result of building AI without asking the right ethical questions first. Amazon's failure offers a clear window into why ethical AI frameworks exist, and what happens when a system is built without one.

## What Makes an AI System Ethical?

Before picking apart what Amazon got wrong, it helps to understand what "getting it right" actually looks like. Philosopher Luciano Floridi and a team of researchers developed a five-principle framework for ethical AI, adapted from concepts in medical ethics:

- **Beneficence**: AI should be designed to benefit people, not just the organizations that build it.
- **Non-maleficence**: AI should avoid causing harm, including harms that aren't obvious at first glance, like reinforcing existing inequalities.
- **Autonomy**: AI should support human decision-making, not quietly replace or override it.
- **Justice**: AI should treat people fairly and not discriminate based on protected characteristics like gender or race.
- **Explicability**: AI should be transparent enough that people can understand how it reaches its decisions, and who is accountable when it doesn't.

Floridi added explicability as a fifth principle specifically because AI raises a problem that traditional ethics didn't have to deal with: systems that make consequential decisions without a clear, traceable explanation for how they got there.

On paper, these five principles sound like common sense. That is exactly the point. Ethical frameworks are not meant to introduce complicated new rules. They are meant to formalize the questions a responsible team should already be asking, so those questions do not get skipped when a project is moving fast. In practice, Amazon's hiring tool violated nearly all of them at once.

## How Amazon's Tool Broke Every Principle

Amazon built its hiring algorithm by training it on ten years of submitted resumes. The problem was that most of those resumes came from men, a reflection of the tech industry's existing gender imbalance. The system learned from that pattern and concluded that male candidates were preferable. It began penalizing resumes that included the word "women's," as in "women's chess club captain," and downgraded graduates of two all-women's colleges.

When you check the tool against each of these principles, the pattern becomes obvious:

- **Justice, violated.** The system discriminated based on gender, exactly the kind of unfair treatment the justice principle is meant to prevent.
- **Non-maleficence, violated.** Rather than avoiding harm, the tool actively reinforced a bias that already existed in the industry, at scale and without human oversight catching it early.
- **Explicability, violated.** Amazon's own engineers reportedly could not fully explain why the model downgraded certain resumes. When a system can't explain its own reasoning, no one can be held accountable for its outcomes.
- **Autonomy, at risk.** The tool was meant to assist recruiters, not replace their judgment. But an AI-generated ranking carries an authority that can quietly override human discretion, especially when reviewers are moving fast through hundreds of applications.
- **Beneficence, undermined.** The tool was supposed to benefit Amazon by streamlining hiring. Instead, it created legal and reputational risk and had to be scrapped entirely.

Amazon did try to fix the problem by editing the program to ignore specific terms like "women's." But this only patched the symptom. There was no guarantee the system wouldn't find other, less obvious proxies for gender, like certain schools, hobbies, or phrasing patterns common in male-dominated fields. By early 2017, Amazon abandoned the project entirely, and the story became public the following year through a Reuters investigation.

## Why Ethical Frameworks Matter Going Forward

Amazon's story shows what happens when ethics gets treated as a bug fix instead of a blueprint. The company noticed the bias only after the tool had already caused harm, and even then, patching individual keywords couldn't guarantee the deeper pattern was gone.

The framework exists to flip that order. Instead of asking "how do we fix this AI system after it fails," it asks "how do we build this system so it doesn't fail in the first place." That shift matters because AI systems don't just reflect the data they're trained on. They amplify it, applying patterns at a scale no individual human reviewer ever could.

A framework built into the design process from day one would have raised red flags long before Amazon's tool ever touched a real resume:

- Did the training data represent a fair, balanced pool of candidates?
- Could the model explain its own decisions clearly enough for a human to catch bias early?
- Was there a way to test outcomes across gender before deployment, not after?

None of these questions require advanced technology to ask. They require the discipline to ask them before something goes wrong, not after.

This is also why frameworks work best when they are not left to individual companies alone. A single team under pressure to ship a product will not always catch what an outside reviewer, a regulator, or an independent audit might catch. Ethical frameworks give organizations a shared standard to build toward. But that standard only means something if someone is actually checking whether it was followed.

## A Lesson in What Not to Skip

Amazon's hiring tool wasn't built by careless engineers. It was built by one of the most technically capable companies in the world, and it still failed on nearly every ethical principle that matters in AI: justice, non-maleficence, explicability, autonomy, and beneficence.

That's the real lesson here. Good intentions and strong engineering aren't enough on their own. Without a clear ethical framework guiding a system from the very start, even well-resourced teams can build tools that quietly cause harm before anyone notices.

As AI takes on a bigger role in decisions that shape people's lives, from hiring to lending to healthcare, the question isn't whether these systems will make mistakes. It's whether the people building them asked the right questions early enough to catch those mistakes before real people paid the price.
