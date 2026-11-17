# Markdown cheat sheet

The specifications are written in Markdown, a simple text format. Every format we publish (web page, PDF, Word) is generated from it, so what you write here is what readers get.

> The real repository has its own Markdown guide with the exact conventions for clause numbers, tables and figures. Some of that is still being agreed. Use this page to learn the basics.

## The basics

| You type | You get |
|---|---|
| `# Title` | A top-level heading |
| `## Section` | A second-level heading |
| `### Subsection` | A third-level heading |
| `**bold**` | **bold** |
| `*italic*` | *italic* |
| `- item` | A bullet point |
| `1. item` | A numbered list |
| `[text](https://example.com)` | A link |
| `` `code` `` | `code` |
| `> quote` | A quoted paragraph |

## Headings and clauses

Headings carry the clause structure. Keep the levels in order: do not jump from `##` to `####`.

```markdown
## 4. Requirements

### 4.1 General

### 4.2 Records
```

## Lists

Leave a blank line before a list, or it will not appear as a list.

```markdown
The provider shall:

- keep records;
- review them yearly;
- make them available on request.
```

## Tables

Tables use `|` between columns and a row of dashes under the header.

```markdown
| Term | Definition |
|------|------------|
| **widget** | An item that is the subject of assessment. |
| **provider** | A person who makes a widget available. |
```

Check there is the same number of columns in every row. A missing `|` is the most common reason a table does not display.

## Links and cross-references

- A link to a web page: `[ISO](https://www.iso.org)`
- A link to a file in this repository: `[the glossary](../GLOSSARY.md)`
- A link to an issue or pull request: `#12`
- A link to a heading in the same file: `[see 4.1](#41-general)`

## Images

```markdown
![A diagram showing the three tiers of reference](assets/tiers.png)
```

Always add a short description between the square brackets. It is read aloud by screen readers.

## Requirement words

Use these deliberately. They have a fixed meaning in standards.

| Word | Means |
|---|---|
| **shall** | A requirement. |
| **should** | A recommendation. |
| **may** | A permission. |
| **can** | A possibility or capability. |

## Common mistakes

| Problem | Fix |
|---|---|
| A list shows as a line of text | Add a blank line before it. |
| A table does not display | Check every row has the same number of columns. |
| A heading shows as text | Add a space after the `#`. |
| Odd line breaks | Leave one blank line between paragraphs. Do not hard-wrap lines. |
| A link is broken | Check for a space between `]` and `(`. |

## Check your work

On GitHub, click the **Preview** tab while editing a file. It shows how the text will look.
