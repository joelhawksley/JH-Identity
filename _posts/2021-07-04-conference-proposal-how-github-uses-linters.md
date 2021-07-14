---
layout: post
title: "Conference proposal: How GitHub uses linters"
---

## Abstract

The GitHub code base is growing at over 25% every year through contributions from over 1000 engineers, clocking in at over 1.7 million lines of Ruby. In this talk, we'll share how we use linters to keep our codebase healthy by ensuring best practices are applied consistently, feedback loops are as short as possible, and code reviews bring the most value, all without creating too much friction.

## Details

This talk is given through a series of case studies that demonstrate how we use linters at GitHub.

I introduce the topic of linting by discussing why we use linters:

- They ensure our practices are applied consistently.
- They shorten the feedback loop of the development process.
- They give us room to provide higher value code reviews.

I then share examples of how we use linters at GitHub today, discussing the advantages and disadvantages of each approach:

- Custom Rubocops
- AST-driven auto-correction
- Auditing written copy to ensure it matches our style guide, using ERBLint
- Extracting linters to gems for use across repositories
- Global counters for patterns we want to avoid
- Per-file counters as an improvement on global counters
- Intelligent code analysis with CodeQL
- Accessibility linting with Axe
- Domain boundary enforcement with Packwerk
- Fanning out large refactors to other teams with Areas of Responsibility and Error Budgets
- Using reporting tools like Datadog to track technical debt
- Using linters to enforce production deployment compliance requirements
- Designing linters to avoid merge conflicts
- Non-blocking linters that "nudge" engineers towards best practices

Finally, I conclude with our takeaways for how we're thinking about our approach to linting for the future.

## Pitch

Whenever I tell people what it's like to be an engineer working on the GitHub code base, they are often amazed by just how much we use linters. It's one of the most significant differences between the GitHub code base and any other one I've seen.

This talk is a "behind the curtains" look at how we approach the practice of linting in one of the largest Ruby code bases in the world. While it is a Rails codebase, our linters run in an environment without Rails present, thus making this talk more appropriate for RubyConf. I will intentionally avoid any Rails-specific content.

I'm a staff engineer at GitHub, working on ensuring our user interface is implemented in a consistent manner. My work often involves building linters that help us adhere to agreed-upon best practices.

I have a decent amount of public speaking experience- I've spoken at several conferences, including a couple of times at RailsConf. I've also appeared on a handful of Ruby-related podcasts.

## Bio

Joel is an engineer on the Design Infrastructure team at GitHub, where he works to help engineers build consistent user interfaces in one of the largest Ruby code bases in the world.
