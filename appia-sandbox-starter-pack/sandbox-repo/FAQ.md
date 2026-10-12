# Frequently Asked Questions

## Getting started

**Do I need to install anything?**
No. Everything in this repository can be done in your web browser. Tools like GitHub Desktop are optional.

**I can't see the repository, or I can't edit anything.**
You may not have been given access yet. Ask the sandbox maintainers (see the [README](README.md)) and mention your GitHub username.

**What is the difference between an issue and a pull request?**
An **issue** is a conversation about *what* should change or be looked at. A **pull request** is a *concrete proposed change* to the files. Many pull requests are linked to an issue.

**What is the difference between a branch and a fork?**
A **branch** is a separate line of work inside the same repository, and it is what you will normally use here. A **fork** is your own copy of a whole repository, used when you don't have permission to create branches in the original.

## Making changes

**I made a mistake in my edit. How do I fix it?**
Just edit the file again on the same branch and commit. If you already opened a pull request, it updates automatically. Nothing is permanent, and every version is kept.

**I accidentally edited `main`. What now?**
If branch protection is on, GitHub won't let you commit to `main`. If it did go through, tell a maintainer. Changes can always be reverted.

**How do I undo a change that was already merged?**
Open the merged pull request and click **Revert**. This creates a new pull request that reverses it.

**GitHub says there's a "merge conflict". What does that mean?**
Someone else changed the same lines you did. Click **Resolve conflicts** on the pull request and choose which version of each conflicting part to keep. If you're unsure, ask in a comment on the pull request.

**What does a good commit message look like?**
Short and specific: "Fix typo in section 3 definition of assessment body". Avoid "update" or "changes".

**What is a draft pull request?**
A pull request marked as not ready for review. Use it to share work in progress. Click **Ready for review** when you're done.

**Can I edit a file in Word and upload it?**
It is better to edit Markdown files directly in GitHub, because then the changes can be compared line by line. A Word file looks like a single blob to GitHub.

## Reviewing

**How do I comment on a specific line?**
Open the pull request, go to **Files changed**, hover over the line, and click the blue **+**.

**How do I suggest exact replacement wording?**
When commenting on a line, click the **±** (suggestion) button in the comment toolbar and type your replacement text. The author can accept it in one click.

**What is the difference between Comment, Approve, and Request changes?**
*Comment* gives feedback without a decision. *Approve* says you're happy for it to be merged. *Request changes* says something must be addressed first.

**Can I approve my own pull request?**
No. GitHub requires someone else to approve.

## Finding things out

**How do I see who changed a line, and why?**
Use the **Blame** view on the file. See [Explore the history](docs/explore-the-history.md).

**How do I find an old version of a document?**
Open the file's **History**, or browse to a **release** or tag.

**How do I search?**
Press `/` anywhere on GitHub to focus the search box, or use the filters at the top of the Issues and Pull requests tabs.

## Notifications

**I'm getting too many emails.**
Click **Watch** at the top of the repository and choose **Participating and @mentions** to only hear about things you are involved in. You can also unsubscribe from any single issue or pull request.

**How do I get someone's attention?**
Write `@their-username` in a comment.

## Markdown cheat sheet

| You type | You get |
|----------|---------|
| `# Heading` | A top-level heading (use `##` and `###` for lower levels) |
| `**bold**` | **bold** |
| `*italic*` | *italic* |
| `- item` | A bullet point |
| `1. item` | A numbered list |
| `[text](https://example.com)` | A link |
| `` `code` `` | `code` |
| `> quote` | A quoted paragraph |
| `#12` | A link to issue or pull request 12 |

Still stuck? Open an issue using the **Ask a question** template.
