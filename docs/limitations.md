# Scope and limitations

[Home](../README.md) · [Checklist](checklist.md) · [Primary references](references.md)

## This repository

This is a collection of written guides, synthetic exercises, and a review worksheet. It is not the source distribution of UNPWNED's scanner. It contains no installable skill, local scanning engine, CLI, browser extension, or API client.

The exercises are intentionally small enough to discuss. They do not represent the distribution of real skills, a collection of confirmed incidents, or a scanner benchmark. Their review notes explain a decision under stated assumptions. They are not verdicts produced by the hosted service.

The deliberately concerning excerpts are study material. Do not give them to an agent as operating instructions or put them in an auto-loaded skill directory.

## What reviewing text can help with

A review can reveal a mismatch between the task and requested access, an unexpected destination, an unreviewed dependency, or a consequential action that lacks clear permission.

It cannot by itself establish what will happen across all agent models, runtime permissions, dependency versions, later downloads, or future updates. A clear-looking instruction may still lead to unsafe behavior. A suspicious phrase may also appear in a legitimate explanation or quoted example.

## Scope is not a verdict

Record exactly what you inspected. Missing files, a failed fetch, truncated content, or changing external instructions leave uncertainty. Do not turn an unknown into either “safe” or “malicious.”

Review the skill source, its references and scripts, the runtime's actual permissions, and the specific version you intend to use. Revisit the decision when any of those change.

## Hosted scanner boundary

The [hosted Skill Scanner](https://www.unpwned.io/skill-scanner) reads files as text without executing the submitted skill. Its current interface describes supported inputs, limits, coverage, and optional data choices. Consult its [Terms](https://www.unpwned.io/terms) and [Privacy Policy](https://www.unpwned.io/privacy) before submitting content.

This guide does not claim that every exercise will produce a particular finding or score in that service. Do not treat the exercise notes as detection rules or reverse-engineered product behavior.

Reviewing a skill is also different from assessing a deployed website. Neither the material here nor a clean skill result establishes the security of the website or service you build with your agent.
