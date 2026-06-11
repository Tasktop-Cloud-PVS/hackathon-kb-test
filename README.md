# hackathon-kb-test

A test KB repo used during the Planview Hackathon (June 2026) to demonstrate the `pvm validate` command and `basic-memory-validate` pre-commit hook from [hackathon-kb-cli](https://github.com/Tasktop-Cloud-PVS/hackathon-kb-cli).

## Setup

```bash
pip install pre-commit
pre-commit install
```

## Demo: manual validation

```bash
pvm validate memory/
```

## Demo: pre-commit hook

Try creating a malformed note and committing it:

```bash
echo '# Bad note with no frontmatter' > memory/bad-note.md
git add memory/bad-note.md
git commit -m "test: add bad note"
# The hook will block the commit and show the error
```
