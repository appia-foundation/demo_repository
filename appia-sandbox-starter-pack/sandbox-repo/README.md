# Appia Foundation Sandbox

Welcome! This repository is a **practice space** for Appia Foundation members. It exists so you can get comfortable with the GitHub workflow we will use to host and develop Appia specifications, without any risk of breaking something real.

> **Nothing in this repository is normative.** Anything you add, edit, or delete here is for learning purposes only. Please don't put confidential or sensitive information in this repo.

## Why GitHub?

The Appia membership has agreed to use GitHub to host our specifications. This gives us:

- **Version history**: every change is recorded, attributable, and reversible.
- **Transparent review**: proposed changes are discussed in the open before they are accepted.
- **Traceability**: issues and pull requests link decisions back to the people and discussions behind them.

## Orientation

📺 **Orientation recording / walkthrough:** `<INSERT LINK>`

If you are new to GitHub, start there, then come back and try the exercises below.

## What's in this repository

| File / folder | What it's for |
|---|---|
| [`specs/sample-specification.md`](specs/sample-specification.md) | A fictional specification to practise editing. It contains a few deliberate flaws for you to find. |
| [`GLOSSARY.md`](GLOSSARY.md) | Plain-English definitions of GitHub terms, with Word and email comparisons. |
| [`docs/how-appia-maps-to-github.md`](docs/how-appia-maps-to-github.md) | How our working group and approval process translates into GitHub. |
| [`docs/explore-the-history.md`](docs/explore-the-history.md) | A short exercise on seeing who changed what, and when. |
| [`FAQ.md`](FAQ.md) | Answers to common "what do I do if...?" questions. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | How to propose changes and what to expect from review. |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | How we work together. |
| [`PARTICIPANTS.md`](PARTICIPANTS.md) | Add your name here as your first exercise. |
| [`.github/`](.github/) | Issue and pull request templates, reviewer assignments, and an automated check. |
| **Issues** tab | Open exercises and "good first issues". |
| **Pull requests** tab | A pre-opened pull request for you to review. |
| **Discussions** tab | Open questions and general conversation. |
| **Releases** | An example of how an approved version is captured. |

## Before you start

1. Create a free account at [github.com](https://github.com/signup) if you don't already have one.
2. Make sure you have been given access to this repository. If you can't see it or can't edit it, contact `<INSERT CONTACT NAME / EMAIL>`.
3. (Optional) Install [GitHub Desktop](https://desktop.github.com/) if you prefer a graphical tool to the command line. You can do everything in this guide directly in your browser.

## The core workflow at a glance

```
Issue  →  Branch  →  Edit  →  Pull Request  →  Review  →  Merge
```

1. **Raise an issue** to describe what you want to change or discuss.
2. **Create a branch** to hold your proposed changes.
3. **Make your edits** on that branch.
4. **Open a pull request (PR)** asking for your changes to be merged.
5. **Respond to review comments.**
6. A maintainer **merges** the PR once it is approved.

---

## 1. How to create an issue

Issues are how we raise questions, report problems, and propose changes.

1. Go to the **Issues** tab of this repository.
2. Click **New issue**.
3. Give it a short, descriptive **title** (e.g. "Clarify definition of conformity assessment in Section 3").
4. In the description, explain:
   - **What** you'd like to change or discuss
   - **Why** it matters
   - **Where** it applies (section, file, line number if relevant)
5. Optionally add **labels**, an **assignee**, or tag colleagues with `@username`.
6. Click **Submit new issue**.

**Tip:** Search existing issues first to avoid duplicates, and keep each issue focused on a single topic.

## 2. How to create a branch

Never edit the `main` branch directly. Work on a branch instead.

**In the browser:**

1. On the repository's main page, click the branch dropdown (it says `main`).
2. Type a new branch name, for example `yourname/fix-typo-section-3`.
3. Click **Create branch**.

**Naming suggestion:** `yourname/short-description`, or reference the issue number, e.g. `issue-12-update-glossary`.

## 3. How to make a change

1. Make sure you are on **your branch**.
2. Navigate to the file you want to change and click the **pencil icon** (Edit).
3. Make your edits.
4. Scroll down to **Commit changes**, write a short message describing what you did (e.g. "Fix typo in introduction"), and choose **Commit directly to your branch**.

Making small, well-described commits makes review much easier.

## 4. How to create a pull request

1. Go to the **Pull requests** tab and click **New pull request**.
   (GitHub will also often show a "Compare & pull request" banner after you push to a branch.)
2. Set **base** to `main` and **compare** to your branch.
3. Add a clear **title** and **description** explaining what the change does and why.
4. Link the related issue by writing `Closes #<issue number>` in the description. The issue will close automatically when the PR is merged.
5. Request one or more **reviewers**.
6. Click **Create pull request**.

## 5. How to review a pull request

1. Open the PR and go to the **Files changed** tab.
2. Hover over a line and click the **+** icon to leave a comment on it.
3. When finished, click **Review changes** and choose:
   - **Comment**: general feedback
   - **Approve**: you're happy for it to be merged
   - **Request changes**: something needs to be fixed first
4. Be constructive and specific. Suggest alternatives where you can.

## 6. Merging

Once a PR has the required approvals, a maintainer will merge it. After merging, the branch can be deleted.

---

## Try it yourself: suggested exercises

| # | Exercise | Skills practised |
|---|----------|------------------|
| 1 | Open an issue introducing yourself | Issues |
| 2 | Create a branch and add your name to `PARTICIPANTS.md` | Branches, editing |
| 3 | Open a pull request for that change | Pull requests |
| 4 | Review a colleague's pull request and leave a comment | Reviews |
| 5 | Propose a change to a sample specification file and link it to an issue | End-to-end workflow |

## Ground rules

- Be respectful and constructive in all comments and reviews.
- Keep issues and PRs focused on one thing at a time.
- Don't worry about making mistakes: that is exactly what this repository is for.
- Anything that looks like a potential **security vulnerability** should not be reported here. Please follow the process in [SECURITY.md](SECURITY.md).

## Getting help

- Questions about GitHub usage? Open an issue with the label `question`.
- Need a hand directly? Contact `<INSERT CONTACT NAME / EMAIL>`.
- Want a refresher? Re-watch the [orientation](#orientation).

Happy experimenting!
