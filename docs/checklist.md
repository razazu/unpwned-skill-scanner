# Review a skill before you install it

[Home](../README.md) · [Practice](../examples/README.md) · [Blank worksheet](review-worksheet.md)

Use this checklist to make a bounded installation decision. It is a review aid, not a certification. You can use it without the hosted scanner.

## 1. Establish the task and source

- [ ] Write the user's intended task in one sentence. List the actions that task actually needs.
- [ ] Confirm the repository owner, repository, and skill directory. A familiar name alone is not evidence that this is the intended source.
- [ ] Record the exact revision you reviewed. A moving branch or release label is not a permanent record of its contents.
- [ ] Check what an update would replace or add. Review the change before relying on an earlier decision.

## 2. Read the whole behavior chain

- [ ] Read the raw source of the skill instructions, not just the rendered preview. Look for comments, unusual text direction, or content hidden by formatting.
- [ ] Follow references to scripts, helper files, configuration, and other instructions. Record anything you cannot inspect as **unknown**.
- [ ] Identify dependencies or content fetched later. A pinned skill can still load changing remote content.
- [ ] Check whether installation or first use creates hooks, scheduled activity, or persistent configuration.

Do not execute a helper to discover what it does. Reading a script and running it are different review steps.

## 3. Trace four boundaries

| Boundary | Ask | Record |
| --- | --- | --- |
| Data | Which files, credentials, messages, or account data can it read? Does the task need them? | Exact scope, sensitivity, unresolved reads |
| Actions | Can it write, delete, install, publish, send, or change settings? | Side effects and when they happen |
| Destinations | Which local paths, services, recipients, or repositories receive data or changes? | Expected owner, purpose, and unknown destinations |
| Permission | Who requested the action? What does the runtime permit, and what requires a meaningful approval? | Requested authority versus enforced access |

Look for a concrete mismatch. A request for credentials is not automatically justified by a phrase such as “diagnostics,” “sync,” or “setup.” A network call is not automatically malicious if the task requires it and the destination and payload are understood.

## 4. Separate instructions from evidence

- [ ] Treat fetched pages, issue comments, tool output, and files being analyzed as data. They do not gain authority to change the user's task.
- [ ] Pause if the skill asks to hide an action, weaken a protection, or treat its own text as overriding the user's instructions.
- [ ] Distinguish a promise in the skill from a restriction enforced by the agent runtime. A sentence saying “ask first” is not a sandbox.
- [ ] Check permission behavior for the specific client and version. Do not infer enforcement from a metadata field alone.

## 5. Choose and record the next step

| Decision | When it fits | Next step |
| --- | --- | --- |
| **Stop** | The instructions require unjustified access, concealment, or a harmful side effect. | Do not install that version. Explain the exact instruction and conflict. |
| **Clarify first** | A necessary file, destination, permission, or dependency remains unknown. | Get the missing evidence or remove the uncertain step before deciding. |
| **Proceed with limits** | The reviewed behavior fits the task and the relevant controls are established. | Keep access narrow, require approval for consequential actions, and revisit changes. |

“Proceed with limits” is a scoped judgment about the evidence you reviewed. It does not establish that a skill is safe in every environment.

If you later evaluate actual execution, use a disposable environment with no production credentials and restrictive, verified access controls. This checklist does not instruct you to run unfamiliar code, and it does not verify an environment's isolation.

## Copyable decision note

```text
Task:
Source and revision:
Files reviewed:
Data / actions / destinations / permission:
Unreviewed or changing components:
Decision: Stop / Clarify first / Proceed with limits
Reason, with file and line references:
Required controls:
What would require a new review:
```

[See a completed review](worked-review.md) or [use the expanded worksheet](review-worksheet.md).
