# Reviewing a pull request

Review is how the Working Group stays in control of what goes into the specifications. Nothing reaches the staging branch until it has been seen and approved. This page shows how to review well, even if you have never used GitHub.

## Open the pull request

1. Go to the **Pull requests** tab and open the one you have been asked to review.
2. Read the description first. It says what changed, why, and which issue it answers.
3. Click **Files changed** to see the edits.

## Reading the changes

- **Red** lines were removed. **Green** lines were added.
- For text, click the small **document icon** (the rich diff) on a file to see the changes as formatted text instead of Markdown symbols.
- Use the **Viewed** tick on each file to keep track of where you are.

## Leaving comments

1. Hover over a line and click the blue **+**.
2. Write your comment.
3. To propose exact wording, click the **±** icon (Add a suggestion) and edit the text inside the box.
4. Click **Start a review**, not **Add single comment**. This keeps all your comments together.

A suggestion lets the author accept your wording with one click, so use it for small wording and typo fixes.

## What to look for

| Check | Question to ask |
|---|---|
| **Meaning** | Does the change say what the issue asked for, and nothing more? |
| **Requirements** | Is "shall", "should" or "may" used deliberately? Did a requirement become weaker or stronger by accident? |
| **Terms** | Are defined terms used consistently? Is a new term defined? |
| **References** | Do references and clause numbers still point to the right place? |
| **Other specs** | Could this affect another specification? If so, say so in a comment so the issue can be linked. |
| **Scope** | Is it one topic, or several mixed together? |

## Finishing your review

Click **Review changes** and choose one:

- **Comment**: general feedback, no decision.
- **Approve**: you are happy for it to go ahead.
- **Request changes**: something must be fixed first. Say what.

## How this fits the approval process

Your approval is one input. In the real repository the Working Group decides, by consensus or a 75% vote. When it has approved, a chair applies the `wg-approved` label and merges into `dev`. Approving on GitHub on its own does not merge anything.

## Good manners

- Be kind and specific. Comment on the text, not the person.
- Explain why, and offer an alternative where you can.
- If you disagree, say so once, clearly, and let the discussion continue in the thread.
- Mark a thread **Resolved** only when the question has actually been answered.
