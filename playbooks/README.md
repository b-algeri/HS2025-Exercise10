# Playbooks and skills: what is here and how to install it

This branch holds a working method for Claude, in two forms.

| File | Purpose |
|---|---|
| `playbooks/chat-project-instructions.md` | Short method for regular claude.ai chats |
| `.claude/skills/fable-playbook/` | General method: plan, work in steps, verify, report |
| `.claude/skills/coding-homework/` | Programming assignments |
| `.claude/skills/math-homework/` | Math problems and proofs |
| `.claude/skills/report-writing/` | Reports and write-ups |

## Installing

**Regular claude.ai chats, always on.** Paste the text of `chat-project-instructions.md` into Settings > Profile (personal preferences), or into a project's instructions.

**Regular claude.ai chats, as skills.** Zip each folder under `.claude/skills/` separately, so that the zip contains the folder with its `SKILL.md` inside, and upload each zip in Settings > Capabilities > Skills. Code execution must be enabled. A skill loads when the task matches its description.

**Claude Code on your own computer, every repo.** Copy the skill folders into your home directory:

```sh
git clone -b claude/opus-task-playbook-i64veg https://github.com/b-algeri/HS2025-Exercise10.git playbook-tmp
mkdir -p ~/.claude/skills
cp -r playbook-tmp/.claude/skills/* ~/.claude/skills/
```

**One specific repo.** Copy `.claude/skills/` into that repo and commit it. To make the general method load on every task there, also copy `CLAUDE.md`.

## Using

Skills load on their own when the task matches. To call one by hand in Claude Code, type `/fable-playbook`, `/coding-homework`, `/math-homework` or `/report-writing`.

## Keeping them useful

Edit the `SKILL.md` files as you learn what your courses expect: required notation, citation style, allowed libraries, autograder formats. Specific rules help more than general ones.

Do not merge this branch into `main` of this exercise repo: the submission check requires a pull request to change nothing except one file in `submissions/`.
