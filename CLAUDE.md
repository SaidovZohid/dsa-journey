# dsa-journey

Personal DSA practice repo. Go. Solutions live in `solutions/<topic>/`,
one package per topic. Reusable Go patterns in `templates/`.

`notes/` is an Obsidian vault (vault root = repo root). Topic notes are
`notes/01-*.md` … `notes/18-*.md`, the hub is `notes/00-index.md`, note
templates are in `notes/_templates/`. Problem notes live in
`notes/problems/`, one file per problem. They carry frontmatter
(`number`, `difficulty`, `topic`, `pattern`, `solved_alone`, `redo_date`) —
that frontmatter is the source of truth for problem metadata.

## Your role

You maintain README.md, PROGRESS.md, and the table in `notes/00-index.md`
ONLY. Never write content in topic notes, problem notes, or `notes/_templates/`.

## Hard rules — do not break these

- NEVER write, fix, optimize, or suggest improvements to any file in
  `solutions/` or `templates/`. Not even if I ask in passing.
- NEVER write or edit the `// Insight:` line in a solution header.
  I write those myself. If one is missing, tell me it's missing.
- NEVER solve a problem for me or hint at an approach, even if I'm stuck.
  If I ask, remind me of the 30-minute rule and stop.
- Do not commit or push. I do that.

## What to do when I say "update progress"

1. Count `.go` solution files per topic folder (exclude `_test.go` and types.go).
2. Update the "Problems solved" column in `notes/00-index.md`. Leave the
   Status column alone unless I tell you what to change it to.
3. Scan frontmatter in `notes/problems/` for `redo_date` values that have
   passed; list them.
4. List problem notes with `solved_alone: false`, grouped by `topic`.
5. Update the "Currently:" line in README.md if the week/topic changed.
6. Append/update this week's PROGRESS.md section with the counts.
   Leave "Weak:" blank for me to fill in.
7. Show me a diff. Don't commit.
