# 01. Scoped formatting review

**Illustrative manual review, not a scanner result or benchmark**

**The user's legitimate task:** “Review the three project documents I selected for inconsistent headings. Suggest changes here; do not edit the files.” The user has authority to share those documents with the configured agent.

**Invented skill excerpt, for reading only:**

```text
L1: Read the three documents selected for this review.
L2: Compare their headings and list suggested wording or formatting changes.
L3: Return suggestions to the user without changing any file.
L4: If another document seems necessary, explain why before requesting access.
```

**Before opening the notes:** Which permissions does this task need, and where should the agent stop?

<details>
<summary>Open the review notes</summary>

This is a benign counterexample under the stated conditions. It illustrates a bounded read, not a certification of a whole skill.

| Review question | Reasoning tied to the excerpt |
| --- | --- |
| Does the workflow fit? | L1–L3 perform the requested heading review. They add no account setup or publication step. |
| What data is needed? | The selected documents, with attention to headings. L4 keeps other documents outside the current scope. |
| What action is proposed? | Reading and producing suggestions. L3 explicitly leaves the files unchanged. |
| Where does the output go? | To the user's response. No additional recipient or upload service is specified. The agent's normal processing environment still matters. |
| What permission is needed? | Read access to the selected documents. Editing, broad workspace access and unrelated connected services are unnecessary. |

**Decision:** Proceed with the selected documents and read-only access. Do not treat the mere mention of file access as evidence of abuse.

**Clarify** if the selection is ambiguous, a selected file contains material the user is not authorized to share, or the agent needs another file to interpret a heading. Ask for the smallest missing input.

**Reject** an expansion to unrelated directories, account data or automatic edits. That would be a different action from L1–L3 and from the user's request.

**What could change the decision:** A bundled helper might access more than the excerpt describes. Read-only access can also disclose information to the agent. Review the actual tools and handling of the selected data before treating this narrow decision as sufficient for use.

</details>

[Back to the cases](README.md)
