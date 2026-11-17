# Working in the Core Specifications repository

The exercises in this sandbox use a simple flow: branch from `main`, then merge back into `main`. The real **Core Specifications** repository has one more step, so you will not be surprised when you get there. This page shows the difference.

> **Note:** this page is an illustration. The authoritative description of the process is in the Core Specifications repository ([GOVERNANCE.md](https://github.com/appia-foundation/core-specifications)), which is private to Working Group participants. If this page differs from it, that repository applies.

## The branches

| Branch | What it is | Who changes it |
|---|---|---|
| `main` | The **publication** branch. Only approved releases are merged here. | WG chairs only |
| `dev` | **Staging.** Holds only what the Working Group has approved. | WG chairs only, after WG approval |
| `spec/NN-name` | One working branch per specification. | That spec's editors |

```mermaid
gitGraph
   commit id: "start" tag: "main = releases only"
   branch dev
   commit id: "approved work"
   branch spec/05-example
   commit id: "editor work"
   commit id: "editor work 2"
   checkout dev
   merge spec/05-example id: "WG approved"
   checkout main
   merge dev id: "Final approval" tag: "v1.0.0"
```

## What is different from the sandbox exercises

| In the sandbox | In the Core Specifications repository |
|---|---|
| Branch from `main` | Editors work on their spec's branch; everyone else raises issues |
| Pull request into `main` | Pull request from the spec branch into **`dev`** |
| A maintainer merges | A WG **chair** merges, after the Working Group approves |
| `main` is the working version | `main` only changes at a Final Approval, tagged `v1.0.0` |

## Practise the real flow

This sandbox has a `dev` branch for the purpose. See exercises 6 and 7 in the [README](../README.md#try-it-yourself-suggested-exercises).

## The route to version 1.0 (proposal)

The Working Group is considering this route from draft to final. It is a proposal, not yet agreed.

| Stage | What it means | In the repository |
|---|---|---|
| Draft | Editors write and revise their own spec | `spec/NN-name` branch |
| Working Group | The group reviews, and a chair merges what it approves | Pull request into `dev` |
| Approved | All specs are approved and sit together | A `release/1.0` branch |
| Candidate | The Steering Committee approves submission, and the text is frozen | Tag `v1.0.0-rc.1` |
| ISO review | Fixes from review are agreed and re-tagged | Tags `rc.2`, `rc.3` |
| Final | Steering Committee Final Approval | Tag `v1.0.0` |

A tag such as `v1.0.0-rc.1` is a fixed, named snapshot. The `rc` part means "release candidate".

## Issues in the real repository

Issues are raised with a form, and the automation adds labels and assigns the right editors. See [Raising an issue](raising-an-issue.md) and the practice form in this sandbox.
