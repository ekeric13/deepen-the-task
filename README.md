# Deepen the Task Skill

Explore unfamiliar work with professional methods, precise language, primary evidence, and independent validation.

A cross-harness skill for Codex, Claude Code, and other Agent Skills-compatible tools. The skill is in [`deepen-the-task/`](./deepen-the-task/SKILL.md).

Use it when you do not yet know what a professional would ask for. It identifies missing practices, primary source material, specific methods and tools, and independent validation. It explains useful domain terminology without expanding the assignment.

Ask for a prompt rewrite to receive a standalone prompt, or ask it to carry out the deeper task. A bare invocation with a task applies the deeper approach and executes within your existing authorization.

## Install With skills.sh

Authenticate to GitHub with an account that can read this private repository before installing.

```bash
npx skills@latest add ekeric13/deepen-the-task
```

## Install For Codex

From a local clone:

```bash
mkdir -p ~/.codex/skills/deepen-the-task
rsync -a deepen-the-task/ ~/.codex/skills/deepen-the-task/
```

Start a new session and invoke it:

```text
Use $deepen-the-task to rewrite this prompt for an unfamiliar domain using precise terminology, concrete methods, and independent validation. Return the rewritten prompt without executing it.
```

## Install For Claude Code As A Plugin

```text
/plugin marketplace add https://github.com/ekeric13/deepen-the-task
/plugin install deepen-the-task@deepen-the-task
```

Invoke the namespaced skill with `/deepen-the-task:deepen-the-task`.

## Install For Claude Code As A Personal Skill

```bash
mkdir -p ~/.claude/skills/deepen-the-task
rsync -a deepen-the-task/ ~/.claude/skills/deepen-the-task/
```

Then use `/deepen-the-task`.

## Verify The Skill

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ./deepen-the-task
```

## Inspiration

Inspired by Felix Rieseberg's [How to be more ambitious: A tutorial for humans with models](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/).
