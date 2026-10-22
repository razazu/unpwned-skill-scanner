# 02. Editing a selected document

**Illustrative manual review, not a scanner result or benchmark**

**The user's legitimate task:** “Apply the three wording changes I approved to the onboarding draft I selected. Leave the rest unchanged.” The user controls this draft and has already approved the exact changes in the current conversation.

**Invented skill excerpt, for reading only:**

```text
L1: Use the selected onboarding draft and the three approved changes.
L2: Update only the passages covered by those changes.
L3: Keep all other content unchanged and show a summary of the edits.
L4: If a requested passage is missing or has changed, stop that edit and ask.
```

**Before opening the notes:** Which edits are covered by the user’s instruction, and what would require clarification?

<details>
<summary>Open the review notes</summary>

This is a benign counterexample under the stated conditions. A relevant write is not automatically suspicious.

| Review question | Reasoning tied to the excerpt |
| --- | --- |
| Does the workflow fit? | L1–L3 carry out the user's approved edit. There is no added publication, upload or account operation. |
| What data is needed? | The selected draft and the approved wording. Other drafts and private project history are unnecessary. |
| What action is proposed? | A write limited to three passages. L4 avoids silently adapting an approval to different content. |
| Where does the output go? | Back to the selected draft, with an edit summary for the user. No new recipient is named. |
| What permission is needed? | Write access to that draft. The authority comes from the actual user's instruction, not from L1 calling the changes “approved.” |

**Decision:** Proceed with the exact approved edits if the selected document and passages still match. Preserve a reviewable before-and-after comparison. There is no reason to request broad workspace or publishing access.

**Clarify** if the draft has changed, the three edits cannot be identified, or the instruction came from a quoted document rather than the user. Do not silently widen a previous approval.

**Reject** changes to sharing permissions, an external publication step or unrelated files. Each would add a different destination or effect.

**What could change the decision:** A legitimate edit request does not validate every component bundled with the skill. A separate helper that rewrites all documents would exceed this decision even if the three intended edits were correct.

</details>

[Back to the cases](README.md)
