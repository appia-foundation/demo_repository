# Extra exercises

These follow on from the exercises in the [README](../README.md#try-it-yourself-suggested-exercises). Each one says what you should see when it works.

| # | Exercise | Skills practised |
|---|---|---|
| 8 | Raise an issue with the practice form | Forms and labels |
| 9 | Ask for a Working Group decision | Automation |
| 10 | Review a pull request with a suggested change | Reviewing |
| 11 | Accept a suggestion on your own pull request | Collaboration |
| 12 | Open a draft pull request | Working in progress |
| 13 | Create and resolve a merge conflict | Conflicts |
| 14 | Find who changed a line, and when | History |
| 15 | Write a table in Markdown | Markdown |

## 8. Raise an issue with the practice form

1. Open **Issues**, then **New issue**, then **Spec change (practice)**.
2. Pick any specification, and describe a problem you can see in `specs/sample-specification.md`.
3. Choose **Editorial** as the type of change. Leave the other answers as they are.
4. Create the issue and reload after about 20 seconds.

**You should see:** labels for your spec, `status:new` and `non-substantive`, and a short comment from the automation.

## 9. Ask for a Working Group decision

1. Raise another issue with the practice form.
2. Choose **Yes, it blocks v1.0**, and tick **This needs a Working Group decision**.
3. Create it and reload.

**You should see:** `blocks-v1.0` and `status:needs-wg-decision`, and no `status:new`.

Now edit the issue, set the block question back to **No**, and save. The `blocks-v1.0` label disappears.

## 10. Review a pull request with a suggested change

1. Open a pull request someone else has made, or ask a colleague to open one.
2. On **Files changed**, hover over a line and click the **+**.
3. Click the **±** icon and change the wording inside the suggestion box.
4. Click **Start a review**, then **Finish your review**, and choose **Comment**.

**You should see:** your suggestion, shown as a before-and-after, with an **Apply** button for the author.

## 11. Accept a suggestion on your own pull request

1. Ask a colleague to leave a suggestion on your pull request (exercise 10).
2. Open the comment and click **Commit suggestion**.
3. Click **Commit changes**.

**You should see:** a new commit on your branch with the new wording, and the thread ready to be marked **Resolved**.

## 12. Open a draft pull request

1. Create a branch and make a small edit.
2. Open a pull request, and in the green button's menu choose **Create draft pull request**.
3. Look at the **Draft** label, then click **Ready for review**.

**You should see:** the pull request changes from grey to green, and reviewers can now be asked.

## 13. Create and resolve a merge conflict

1. Create two branches from `main`, called `yourname/conflict-a` and `yourname/conflict-b`.
2. On branch A, change the title line of `specs/sample-specification.md` to one wording, and commit.
3. On branch B, change the **same line** to a different wording, and commit.
4. Open a pull request from A into `main` and merge it.
5. Open a pull request from B into `main`.

**You should see:** "This branch has conflicts that must be resolved". Follow [When things go wrong](when-things-go-wrong.md#there-is-a-merge-conflict) to fix it.

## 14. Find who changed a line, and when

1. Open `specs/sample-specification.md`.
2. Click **Blame**, at the top of the file.
3. Click a commit message next to any line.

**You should see:** who last changed that line, when, and in which pull request.

## 15. Write a table in Markdown

1. Edit `PARTICIPANTS.md` on a branch.
2. Add a table of three terms and their definitions, using the [Markdown cheat sheet](markdown-cheat-sheet.md).
3. Use the **Preview** tab to check it.

**You should see:** a formatted table, with the same number of columns in every row.
