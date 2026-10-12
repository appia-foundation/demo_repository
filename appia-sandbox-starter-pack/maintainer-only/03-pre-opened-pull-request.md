# Pre-opened pull request

This gives people a real pull request to review. It's best done **after** the initial files are committed to `main` and branch protection is on.

## Steps

1. On the repository's main page, open the branch dropdown, type `demo/fix-assessment-body-typo` and click **Create branch**.
2. Open `specs/sample-specification.md` **on that branch** and click the pencil icon.
3. In the definition of **assessment body**, change `assesment` to `assessment`.
4. Commit with the message: `Fix typo in definition of assessment body`.
5. Click **Contribute → Open pull request**.
6. Fill in the template:
   - **Title:** `Fix typo in definition of assessment body`
   - **What does this change?** Corrects a spelling error in section 3.
   - **Why?** Consistency and readability.
   - **Type of change:** Editorial
7. Request a reviewer, or leave the field empty so anyone can pick it up.
8. Add a comment from the maintainer: "This is a practice pull request. Please review it as part of the 'Review the open pull request' exercise. Do not merge it. A maintainer will do that at the end."
9. **Do not merge.** Leave it open for people to review.

## Notes

- This fixes one of the flaws in the sample specification, so mention in the exercise issue that the typo is already being handled.
- When the exercise is over, approve and merge it yourself (using a second account if needed) to demonstrate the final step.
- Consider also opening a **draft** pull request with a half-finished change, to demonstrate what a draft looks like.
