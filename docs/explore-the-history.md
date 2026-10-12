# Exercise: explore the history

One of GitHub's most useful features is that nothing is ever really lost. Every change is recorded with who made it, when, and why. This exercise takes about 10 minutes.

You will need nothing but your browser.

## 1. View the history of a file

1. Open [`specs/sample-specification.md`](../specs/sample-specification.md).
2. Click **History** (top right of the file view).
3. Click on any commit to see **exactly what changed** in that commit (a *diff*). Green lines were added; red lines were removed.

**Question:** Who last changed this file, and what was their commit message?

## 2. See who changed each line (Blame)

1. Open the same file again.
2. Click **Blame** (next to the Raw button, or via the "..." menu on mobile).
3. Each line now shows who last changed it and in which commit.
4. Click the commit message next to a line to jump to the change.

**Question:** Pick a requirement in section 4. Who last changed it?

## 3. Compare two versions

1. Go to the repository's main page and click **Commits**.
2. Pick an older commit and a newer one.
3. In your browser's address bar, edit the URL to read `.../compare/<older-commit>...<newer-commit>`. (Use the first 7 characters of each commit ID.)

**Question:** What changed between the two versions?

## 4. Trace a change back to its discussion

1. Open a closed pull request from the **Pull requests** tab.
2. Read the conversation and the **Files changed** tab.
3. Notice which issue it links to.

**Question:** Can you find the reason a change was made, without asking anyone?

## 5. See what a release captures

1. Click **Releases** on the right-hand side of the repository's main page.
2. Open `v0.1.0`.
3. Use **Browse files** (or the source code download) to view the repository exactly as it was at that point.

**Question:** If `main` has changed since, how would you refer to the exact approved version?

## Share what you found

Post a comment on the "Explore the history" issue to say what you discovered, or ask a question if anything was unclear.
