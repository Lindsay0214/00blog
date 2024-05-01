---
title: Establishing Better Code Review Principles and Standards for Your Team
excerpt: In recent years, the way we work has undergone a significant transformation, largely due to advancements in technology and changing attitudes toward work-life balance. One of the most notable changes has been the rise of remote work, allowing employees to work from the comfort of their own homes.
publishDate: 'May 1 2024'
tags:
  - Code Quality
  - Code Review
seo:
  image:
    src: '/post-1.jpg'
    alt: A person standing at the window
---

![A person standing at the window](/post-1.jpg)

**Note:** This post was created using Chat GPT and explainthis.io E+ plan content to demo.

In this article, we delve into how teams should approach Code Reviews. For those aspiring to reach senior levels, understanding Code Review from a team perspective is crucial. Senior engineers are not only responsible for conducting Code Reviews but also play a key role in developing and refining Code Review guidelines and processes, as well as fostering a positive Code Review culture.

## Establishing a Code Review Process

If your team lacks a formal Code Review process, I recommend taking the initiative to help establish one.

Here are common steps in the engineering team's Code Review process:

- First, after writing the code, push it to a remote branch and complete automated checks via Continuous Integration (CI), which we will discuss more in the next section.
- If the automated checks pass, you can then request a Code Review for the branch to be merged. Modern code repository tools like GitHub and GitLab offer diff tools that allow you to easily identify code changes.
- Next, invite relevant personnel for the Code Review. Many code repository tools will automatically scan the submitted code and assign it to those who have previously worked on related parts of the code. 
- The relevant personnel provide feedback on the Pull Request (PR), and the PR author makes adjustments based on this feedback. This back-and-forth process should not drag on too long and continues until the reviewers feel the code is satisfactory and give a 'LGTM' (Looks Good To Me), indicating the Code Review is passed, and the code can be merged.


## What to Check in CI

Given the valuable time of engineers, certain basics should be ensured through automated tools integrated into the CI process before starting a Code Review. This prevents wasting other engineers' time on issues that automated tools can handle.

Currently, many teams implement the following checks in CI, which are recommended for adoption:

1. Type checking to ensure no errors in data types.
2. Static analysis: Commonly includes linting to ensure adherence to the repository's linting rules and style checks. Code Reviews should not focus on style issues, which should be handled by static analysis tools.
3. Testing: Most teams include a standard for test coverage, failing the CI if the coverage does not meet a certain threshold.
4. Performance testing: Many performance testing tools can be integrated into CI. For web frontends, for instance, Google's Lighthouse (link) can be integrated, and some teams set it up so that if a PR causes a score drop in Lighthouse, it fails.
5. Build verification to ensure the code builds successfully.

## Recommended Code Review Principles and Standards for Teams
After passing the checks set in CI, the actual Code Review begins. Here are some recommended principles for teams:

### Complete Reviews Promptly:
Delay in Code Review means delay in feature delivery. Ideally, Code Reviews should be completed within a day, including multiple feedback rounds until the final approval and code merge. From a team perspective, it's crucial to ensure engineers have enough time. If engineers are too busy to review, then engineering managers need to help redistribute workloads.

### Clear Commit Messages
If using Git for version control, engineers need to commit their code before sending a PR. Well-standardized commit messages make it easier for reviewers and future maintainers to navigate through commits.

A common industry practice for commit messages includes using a prefix to indicate the type of commit and keeping the message concise.

The Conventional Commit Messages open-source project provides a detailed explanation of this:
- feat for new feature-related commits.
- fix for bug fixes.
- refactor for refactoring changes.
- style for style adjustments.
- test for test-related changes.
- chore for uncategorized changes.

## Include a Test Plan in PRs

It's recommended to not only describe the changes in a PR but also include a Test Plan. This helps reviewers understand the changes better and provides an opportunity to refine the test plan during the Code Review.

Below is an example of a Test Plan by former Meta engineer Dan Abramov in an open-source project submission.


## Include Demos in PRs

For frontend-related changes, including web and mobile (iOS and Android), it is advisable to include a demo standard. The most common method is to add a screen recording, allowing reviewers to quickly grasp the changes. This is very helpful for reviewers to get up to speed quickly.
Below is an example of a screen recording demo by former Meta engineer Dan Abramov in an open-source project submission.

## Fostering a Positive Culture
Code Review is a reflection of an engineering team's culture. This is why it's highly recommended to inquire about a team's Code Review culture during interviews to gauge





