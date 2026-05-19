# Contributing to AI-Native Startup OS

This operating system is meant to be forked, modified, and improved.
If you have a better way to run an AI-native company, share it.

## What You Can Contribute

### Skills (reusable workflows)

Skills are the most valuable contribution. If you've built a workflow that makes
your AI-native company run better, package it as a skill and share it.

```
skills/
├── customer-discovery/        ← Interview frameworks, question templates
├── competitive-analysis/      ← Market research workflows
├── security-audit/           ← Automated security review scripts
├── deployment-pipeline/      ← CI/CD templates for AI-native companies
├── measurement-framework/    ← Analytics setup, Sean Ellis test scripts
└── [your-skill-name]/        ← Your contribution here
```

Each skill should include:
- `README.md` — What it does, when to use it, how to set it up
- The actual workflow files (scripts, templates, prompts)

### Templates

Improvements to `SCOPE.md`, `MEASUREMENTS.md`, `LAUNCH-CHECKLIST.md`,
or `RHYTHM.md` — things you found missing or got wrong.

### Translations

If this OS is useful in your language, translate it.

## How to Contribute

1. **Fork** this repository
2. **Create a branch** (`git checkout -b my-awesome-skill`)
3. **Commit your changes** (`git commit -m "Add customer discovery skill"`)
4. **Push** (`git push origin my-awesome-skill`)
5. **Open a Pull Request**

## Guidelines

- **One skill per PR** — Makes review easier
- **Include a README** in your skill directory explaining what it does
- **Keep it tool-agnostic** — This OS works with any AI model
- **No self-promotion** — Contributions should add genuine value

## Questions?

Open an issue. Or better yet, open a PR with what you think should change.

---

*This OS thrives on contributions. The best operating system is the one
that gets better every time someone runs it.*
