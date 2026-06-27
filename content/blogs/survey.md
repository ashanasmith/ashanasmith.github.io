---
title: "When Anonymous Isn’t Anonymous: Ethical Challenges in Data Collection"
date: 2026-06-19
draft: false
github_link: "https://github.com/Ashana-Smith/Ashana-Smith"
author: "Ashana S."
tags:
  - Data Ethics
  - Data Privacy
  - Informed Consent
  - Survey Design
image: /images/blog.png
description: "An exploration of the ethical concerns surrounding perceived anonymity in data collection and course surveys"
toc: 
---

We’ve all clicked “submit” on a survey after being told our answers are anonymous. It feels safe. It feels honest. But what happens when that promise isn’t actually true? 

This is exactly the situation I want to break down today. A course completion survey looks simple on the surface: ten questions, a rating scale, a request for honest feedback. But the way it’s built tells a different story than the one it claims. Understanding why matters, not just for data analysts, but for anyone who has ever filled out a survey and trusted the label “anonymous.” 

# The Case at Hand
 
Here’s the situation. At the end of a course, participants are asked to complete a short survey, ten questions in total, accessed through a URL that’s only available for a limited time. To get started, students have to log in using their organization username and password. 

Once inside, the survey asks for the name of the course, but never asks for the student’s name. The description tells participants that all answers, and the survey itself, will remain anonymous. 

Executive management wants to use the survey results to decide which courses need to be redesigned or updated. As the data analyst in this scenario, I’m the one tasked with turning that data into actionable insights and identifying any issues with how it was collected along the way.

On the surface, this looks like a normal feedback loop. But once you look closer at how the data is actually collected, some serious ethical problems start to surface. 

# Ethical Issues in the Survey Design

The biggest issue here is hiding in plain sight: the survey claims to be anonymous, but it isn’t. 

To even access the survey, students must log in with their username and password. That single requirement means the organization already knows exactly who is taking the survey, the moment they log in. Not asking for a name inside the survey itself doesn’t erase that. The identity is already attached before the first question even loads. 

This is where the concept of **anonymization** versus **pseudonymization** becomes important. True anonymization means data cannot be traced back to an individual, even if someone tried. Pseudonymization means identifying details are replaced with a code or token, but the link back to the real person still exists somewhere. In this case, there isn’t even a layer of pseudonymization protecting the student. The login system ties their real identity directly to the survey session, with no separation at all. 

Calling this “anonymous” isn’t just inaccurate; it’s misleading. And that points to a deeper issue: **transparency**. Participants are told one thing about how their data will be handled, while the system behind the scenes works completely differently. Without transparency, students can’t give true **informed consent** either. Informed consent depends on people understanding what’s actually happening with their data. If the description of the survey is false, the consent built on top of it is compromised from the start. 

# Other Ethical Issues Worth Considering

Beyond the anonymity problem, two other issues stand out once you look at the bigger picture. 

#### 1. Limited access window

The survey link is only available for a short period of time. On the surface, this might seem like a minor scheduling detail, but it raises a fairness concern. Students who are sick that week, dealing with unreliable internet, navigating a disability that requires more time, or simply juggling other responsibilities (a familiar challenge for many online and remote learners) could be locked out before they even get the chance to respond. 

When a portion of the population is effectively excluded, the resulting data isn’t a fair representation of everyone’s experience. It only reflects the people who happened to be available, online, and quick enough to act within the window. Any insights drawn from that data carry a built-in bias before analysis even begins. 

#### 2. Power imbalance and honesty

The second issue is more subtle, but arguably more damaging to the survey’s purpose. Students need this course for something, whether it’s certification, credit, or job-related training. When they know their real identity is tied to their responses, a natural hesitation creeps in. Will being too critical reflect poorly on them? Could honest feedback affect how they’re seen by the organization? 

This is a textbook example of a **power imbalance**. The organization holds influence over the student’s outcomes, and the student is aware their feedback isn’t truly private. In situations like this, people tend to soften their answers, avoid pointed criticism, or rate things more positively than they actually feel, simply to protect themselves. The result is data that looks clean on the surface but is quietly skewed underneath. 

And this isn’t just an ethical concern; it undermines the entire purpose of the survey. If executive management makes decisions about which courses to redesign based on self-censored feedback, they’re not really making data-driven decisions. They’re making decisions based on a distorted picture of the truth. 

# What Should Be Done About It

Once these issues are identified, the next step is figuring out how to actually fix them. Here are three concrete recommendations a data analyst can make in this scenario.

#### 1. Be honest about what "anonymous" really means

As the data analyst, my first recommendation would be to stop claiming the survey is anonymous when it isn’t. Since the survey can’t be truly anonymous due to the login requirement, I’d recommend the description clearly state that login is required, that responses will be linked to the account used to log in, and exactly who will have access to individual responses (for example, only a designated administrator, not instructors or general staff). 

An even stronger fix I’d propose is decoupling the login from the survey itself. Login could simply verify that someone completed the course, then redirect them to a separate survey tool that doesn’t tag their responses to their account at all. This would allow the organization to achieve genuine anonymity, rather than just claiming it. 

#### 2. Remove the time pressure

My second recommendation is to extend the survey’s access window. Rather than a short window, the survey should be available for one to two weeks immediately after course completion. This gives students time to respond when they actually have reliable access, regardless of time zone, schedule, or temporary setbacks. I’d also suggest a simple reminder email partway through the window to help boost response rates without forcing anyone into a rushed decision. 

#### 3. Remove the fear factor from feedback

My third recommendation addresses the power imbalance directly. I’d advise the organization to explicitly state that responses have no impact on grades, certification, or standing, regardless of how critical the feedback is. But a statement alone may not be enough to fully ease that fear, especially when identity is still attached to responses behind the scenes. 

That’s why my stronger recommendation is structural: limit access to individual, identifiable responses entirely, and only share aggregated, de-identified results with executive management. For example, instead of seeing “Student X disagreed that the course met objectives,” management would see “73% of students agreed the course met its objectives.” This protects individual students while still giving the organization the insights it needs to make decisions. 

# What If Management Says No?

Recommendations don’t always get accepted right away, even when they’re well-reasoned. So what happens if executive management pushes back and insists the survey is fine exactly as it is? 

This is where the role of a data analyst gets tested. Disagreeing with leadership doesn’t mean the only options are silent compliance or walking away. There are several ethical paths to take before reaching that point. 

#### 1. Document the concerns formally

Even if management dismisses the feedback verbally, putting concerns in writing (through email, a memo, or a formal report) creates a clear record. This protects the analyst by showing the concern was raised properly, and it lays the groundwork for further escalation if needed. 

#### 2. Escalate to compliance, privacy, or legal teams

Most organizations have a department responsible for data protection and ethical oversight, separate from the team requesting the analysis. If a direct manager won’t act, escalating the concern to people with more authority over privacy and compliance can carry more weight, especially if there’s potential legal exposure tied to misleading claims about anonymity. 

#### 3. Be transparent within the deliverable itself

If the analysis still has to move forward using flawed data, the analyst doesn’t have to pretend the data is perfectly clean. The final report can include clear caveats, noting that responses may be biased due to limited anonymity, flagging specific findings as lower confidence, and recommending that future surveys be redesigned with stronger privacy protections. 

#### 4. Refuse to misrepresent the data, as a last resort

What an analyst should never do is present flawed data as fully reliable just to deliver the clean answer management wants. Doing the work honestly, while being clear about its limitations, preserves both the analyst’s integrity and the usefulness of the insights being delivered. 

---
# The Takeaway

This survey looks harmless on the surface. Ten questions, a rating scale, a quick login. But once you look past the label “anonymous” and examine how the system actually works, several ethical issues come into focus: a misleading privacy claim, a lack of transparency, an exclusionary access window, and a power imbalance that quietly distorts honesty. 

None of these issues require bad intentions to exist. They can show up simply because no one stopped to ask whether the system matched the promise being made to participants. That’s exactly why ethical awareness matters in data work. It’s not just about following rules, it’s about noticing the gap between what a system claims and what it actually does, and being willing to close that gap, even when it’s inconvenient or unpopular with leadership. 

Good data isn’t just accurate, it’s trustworthy. And trust starts with telling people the truth about what’s really happening with their information. 