# Answer key: sample specification flaws

All in `specs/sample-specification.md`.

| # | Location | Flaw | Type |
|---|----------|------|------|
| 1 | Section 3, definition of *assessment body* | Spelling error: "assesment" | Editorial |
| 2 | Section 4 | **Two sections are numbered 4.2** ("Quality management" and "Change control"). The second should be 4.3, and its requirement ID, REQ-4.2.3, should be REQ-4.3.1. | Structural |
| 3 | Section 4.2 (second), final paragraph | An unnumbered requirement ("The provider must make a Declaration of conformity...") with no REQ ID, and it uses "must" where the rest of the document uses "shall". | Technical / Editorial |
| 4 | Section 4.2 (second), final paragraph | "Declaration of conformity" is used but **not defined** in section 3. | Terminology |
| 5 | REQ-4.2.2 | Uses "should" (a recommendation) while nearly everything else uses "shall" (a requirement). Possibly intentional, but worth a question. | Technical |
| 6 | Section 3 and 5.1 | **Assessor** vs **assessment body** are used in different places (REQ-5.1.1 vs REQ-5.1.2). The roles are defined separately, but the requirement is ambiguous about who records the outcome. | Terminology |
| 7 | Annex A | The table is **incomplete**: it omits REQ-4.2.3, REQ-5.1.2, REQ-5.2.1 and REQ-5.2.2. | Content |
| 8 | Section 2 | The normative reference is listed, but the document does not cite ISO/IEC 17000 anywhere in the body text. A normative reference should normally be referred to in the text. | Technical |
| 9 | Front matter | "Version 0.1 (draft)" has no date. | Editorial |

Use this key to guide discussion when people report back, and to check the pre-opened pull request doesn't conflict with a flaw people are meant to find.
