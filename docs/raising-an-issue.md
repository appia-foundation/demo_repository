# Raising an issue

In the real repository, you raise an issue by choosing a form, picking from drop-down lists and ticking boxes. Automation then does the sorting. This page shows what each part of the form does, using the *Spec change (practice)* form in this sandbox.

> In the sandbox the automation adds **labels only**. In the real repository it also assigns the spec's editors and notifies them.

## Try it

1. Open the **Issues** tab and click **New issue**.
2. Choose **Spec change (practice)**.
3. Fill in the form, using the table below.
4. Click **Create**.
5. Reload the issue after about 20 seconds. The labels and a short comment have appeared.

## The form, field by field

| Field | What to choose | What the automation does |
|---|---|---|
| **Which specification?** | The specification the issue is about. Pick `00` for the front cover and shared terms. | Adds a label such as `spec-03`. In the real repository, assigns that spec's editors. |
| **Clause or section** | The part of the text you mean, for example `4.2` or `Table 1`. | Nothing. It helps the editor find the place. |
| **What is the issue?** | Your own words. Say what is wrong, unclear or missing. | Nothing. This is the part only you can write. |
| **Proposed change** | Suggested wording, if you have it. | Nothing. A ready-made change speeds things up. |
| **Does this block v1.0?** | Choose **Yes** only if the first release cannot go ahead without it. | **Yes** adds the `blocks-v1.0` label. |
| **Type of change** | **Editorial** for typos, formatting and links with no change of meaning. Otherwise **Substantive**. | **Editorial** adds the `non-substantive` label. |
| **Working Group decision** | Tick the box if the Working Group must decide. | Adds `status:needs-wg-decision`, so the issue appears on the Working Group agenda. |

## The labels you will see

| Label | Meaning |
|---|---|
| `spec-00` to `spec-06` | Which specification the issue concerns. |
| `status:new` | Just raised. Waiting for an editor to look at it. |
| `status:needs-wg-decision` | Waiting for a Working Group decision. |
| `blocks-v1.0` | Must be resolved before the first release. |
| `non-substantive` | An editorial change with no effect on meaning. |

Editors move an issue on to `status:accepted` or `status:not-accepted` once it is settled.

## Tips for a good issue

- **One topic per issue.** Two problems are two issues.
- **Be specific.** Give the clause number and the exact words you are looking at.
- **Say why it matters.** A reviewer who understands the effect can decide faster.
- **Search first.** Someone may have raised it already. Add a comment there instead.
- **Edit if you got it wrong.** Click the three dots on the issue and choose **Edit**. The labels follow your new answers.

## What happens next

1. An editor looks at it, usually before the next meeting of that specification.
2. If it needs the Working Group, it goes on the agenda.
3. If it is accepted, an editor makes the change on the spec's branch and opens a pull request that mentions your issue.
4. When the change is approved and merged, the issue closes.
