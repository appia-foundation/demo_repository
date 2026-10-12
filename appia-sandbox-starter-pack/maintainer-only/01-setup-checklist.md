# Setup checklist

Work through these in order. The tick-box items are one-off tasks.

## 1. Add the files

- [ ] Copy everything in `sandbox-repo/` into the root of the demo repository, keeping the folder structure (including the hidden `.github` folder).
- [ ] Keep your existing `SECURITY.md`. The README, CONTRIBUTING and issue config all link to it.
- [ ] Replace the placeholders listed in `00-READ-ME-FIRST.md`.
- [ ] Commit directly to `main` for this initial setup, **before** turning on branch protection.

## 2. Create labels

Go to **Issues → Labels → New label** and create:

| Label | Suggested use |
|-------|---------------|
| `proposal` | Applied automatically by the proposal template |
| `question` | Applied automatically by the question template |
| `exercise` | Sandbox practice tasks |
| `good first issue` | Easy starting points (GitHub surfaces this label) |
| `editorial` | Typos, wording, formatting |
| `terminology` | Definitions and consistent term use |
| `technical` | Requirements and scope |
| `documentation` | README, glossary, FAQ changes |

The first two **must exist** for the issue templates to apply them.

## 3. Create the teams (optional but recommended)

CODEOWNERS only works with teams or users who have **write** access.

- [ ] In the organisation, create teams such as `sandbox-maintainers` and `sandbox-spec-reviewers`, and give them write access to the repository.
- [ ] Update `.github/CODEOWNERS` to match the real team names, or swap in individual `@usernames`.
- [ ] Confirm the file shows no errors: open it in GitHub and look for a warning banner above the file.

## 4. Turn on branch protection

Use a **ruleset** (Settings → Rules → Rulesets → New ruleset → New branch ruleset):

- [ ] **Name:** `Protect main`
- [ ] **Enforcement status:** Active
- [ ] **Target branches:** Include default branch
- [ ] Enable **Restrict deletions** and **Block force pushes**
- [ ] Enable **Require a pull request before merging**
  - Required approvals: **1**
  - Optional: **Require review from Code Owners**
  - Optional: **Dismiss stale pull request approvals when new commits are pushed**
- [ ] Do **not** require status checks for now. The markdown lint is a demonstration and shouldn't block beginners.

Things to be aware of:

- Authors can't approve their own pull requests, so you need **at least two people** with write access to demo the full cycle.
- Repository admins can usually bypass rules. Check the **Bypass list** is what you intend.
- If you prefer the older interface, the equivalent is Settings → Branches → Add branch protection rule.

## 5. Check access and visibility

- [ ] Decide whether the repo is public or private. If private, add members individually or via a team.
- [ ] Set the access level members need. **Write** access lets them create branches directly in the repo. With **Read**, they must fork instead, which is more complicated for newcomers.
- [ ] Test with a non-admin account, or ask a colleague to confirm they can create a branch and open a pull request.

## 6. Enable Discussions

- [ ] Settings → General → Features → tick **Discussions**.
- [ ] Keep the default categories, or create: *Announcements*, *Q&A*, *Ideas*, *Show and tell*.
- [ ] Post the welcome message from `05-discussions-welcome-and-release-notes.md` and **pin** it.

## 7. Create the seed issues

- [ ] Create the issues in `02-seed-issues.md`, with labels as listed.
- [ ] Pin the introductions issue so it's at the top of the Issues tab.

## 8. Create the pre-opened pull request

- [ ] Follow `03-pre-opened-pull-request.md`.

## 9. Publish the `v0.1.0` release

- [ ] Go to **Releases → Draft a new release**.
- [ ] **Choose a tag → type `v0.1.0` → Create new tag on publish**, target `main`.
- [ ] Title and notes: see `05-discussions-welcome-and-release-notes.md`.
- [ ] Tick **Set as the latest release** and click **Publish release**.
- [ ] Do this **after** the pre-opened pull request is created, but make sure it is based on the state you want people to see.

## 10. Check the automation

- [ ] Open the **Actions** tab and confirm the *Markdown lint* workflow is listed and ran on your initial commit. If Actions is disabled for the organisation, you'll need to enable it or skip this step.
- [ ] Open the pre-opened pull request and confirm the check appears at the bottom.
- [ ] Note that markdownlint may report style warnings on files in the pack. That is fine for a demo, but you can tidy them or adjust `.markdownlint.json`.

## 11. Update the announcement

- [ ] Add the real repository URL and orientation link to the README and the email.
- [ ] Add the Discussions tab to the email if you want people to use it.
- [ ] Send a test link to one colleague before the full mailout.

## 12. Dry run

- [ ] Ask one or two people to go through the exercises cold and note where they got stuck. Fix the README or FAQ accordingly.
