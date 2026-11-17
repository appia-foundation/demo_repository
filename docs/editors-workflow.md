# The editor's workflow

Editors look after one specification each. This page covers the routine, from picking up an issue to the chair merging your work. In the real repository your specification has its own branch, named like `spec/03-organizational-risk-management`. In the sandbox, practise with a branch you create yourself (see exercises 6 and 7 in the README).

## The routine

```text
Issue  →  Your spec branch  →  Pull request into dev  →  Working Group review  →  Chair merges
```

1. **Pick up an issue.** Issues for your spec are assigned to you. Read it and reply if it is unclear.
2. **Update your branch** with the latest from `dev` (see below).
3. **Make the change** on your spec branch, in small steps, each with a clear commit message.
4. **Open a pull request** from your branch into `dev`. Link the issue with `Closes #12`.
5. **Answer review comments** by adding more commits to the same branch.
6. **A chair merges** once the Working Group has approved. You do not merge into `dev` yourself.

## Statuses on an issue

| Label | What you do |
|---|---|
| `status:new` | Read it, then reply or move it on. |
| `status:editor-review` | You and the other editors are discussing it. |
| `status:needs-wg-decision` | It is with the Working Group. Do not change the text until it decides. |
| `status:accepted` | Make the change and open a pull request. |
| `status:not-accepted` | Explain why in a comment, then close it. |

## Bringing the latest `dev` into your branch

Do this before you start work, and again if your pull request says it is out of date.

**In the browser:**

1. Click **Pull requests**, then **New pull request**.
2. Set **base** to your spec branch and **compare** to `dev`.
3. If it shows changes, click **Create pull request**, then **Merge pull request**.

**In GitHub Desktop:** choose your branch, then **Branch**, **Update from dev**.

If it reports a conflict, see [When things go wrong](when-things-go-wrong.md).

## Writing good commit messages

- Start with what changed, in plain words: `Define "conformity assessment" in clause 3`.
- One idea per commit where you can.
- Mention the issue number if there is one: `Fix reference in 4.2 (#12)`.
- Avoid messages like `update` or `changes`.

## Opening the pull request

The pull request form has a checklist. Fill it in honestly. In particular:

- Choose the **type of change**. It helps the Working Group see what kind of review is needed.
- Check **Files changed** shows only what you meant to change.
- Use **Draft** if it is not ready yet. Click **Ready for review** when it is.

## Editorial changes

Typos, formatting and links that do not change the meaning can go straight to a pull request. Label it `non-substantive`. The Working Group is still defining exactly where editorial ends and substantive begins, so when in doubt, raise an issue and ask.

## Keep these habits

- Small pull requests are reviewed faster.
- Never edit `dev` or `main` directly.
- Check how the formatted text looks, using the **Preview** tab before you commit.
- Reply to every review comment, even if only to say "done".
