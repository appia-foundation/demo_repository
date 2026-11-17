# When things go wrong

Mistakes are normal here, and every version of every file is kept, so very little is permanent. Find your situation below.

## I edited the wrong branch

If you have not committed yet, copy your text, switch to the right branch and paste it in.

If you have committed, tell the repository administrator or ask in an issue. The commit can be moved or reverted without losing your work.

## I want to undo a change

1. Open the file and click **History**.
2. Find the version you want, and click `<>` to view the file at that point.
3. Copy the text back into the current file and commit it, with a message like `Restore earlier wording`.

For a whole pull request that has already merged, open it and click **Revert**. GitHub makes a new pull request that undoes it.

## My pull request shows too many files

You probably started your branch from the wrong place, or brought in changes by accident. Close the pull request, and ask the repository administrator to help re-create it from the right branch. Your edits are not lost.

## The pull request says "This branch is out of date"

Bring in the latest changes. See [The editor's workflow](editors-workflow.md#bringing-the-latest-dev-into-your-branch).

## There is a merge conflict

A conflict means two people changed the same lines and GitHub cannot choose between them. It looks like this in the file:

```text
<<<<<<< my-branch
The provider shall keep records for five years.
=======
The provider shall keep records for seven years.
>>>>>>> dev
```

To fix it in the browser:

1. On the pull request, click **Resolve conflicts**.
2. Decide which text is right. It may be one of them, or a mix of both.
3. Delete the three marker lines (`<<<<<<<`, `=======`, `>>>>>>>`) and the version you do not want.
4. Click **Mark as resolved**, then **Commit merge**.

If the two versions disagree on meaning, do not pick one alone. Add a comment on the pull request and ask the other author.

## The Markdown check failed

The red cross on a pull request is the automatic style check. Click **Details** to see what it found. It usually points to a line with a missing blank line or a heading level out of order. Fix it on your branch and the check runs again. In this sandbox the check is not required to merge.

## I cannot see or edit something

You may not have access yet, or you may be on a protected branch. Check which branch you are on. If you still cannot, contact the repository administrator and give your GitHub username.

## I am not sure what to do

Ask. Open an issue with the **Ask a question** template. Nobody minds, and the answer helps the next person.
