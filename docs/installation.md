# Installation

Install the entire [package folder](../skills/personal-readme), including its references and license. Its directory name is `personal-readme`.

## Codex

Copy `skills/personal-readme` into the project’s `.agents/skills/`, or use `~/.agents/skills/` for your account. Ask for a new or revised GitHub profile README, or select Personal README explicitly in a Codex interface that supports skill selection. [Codex skill documentation](https://learn.chatgpt.com/docs/build-skills)

## Claude Code

Copy `skills/personal-readme` into the project’s `.claude/skills/`, or use `~/.claude/skills/` for your account. Invoke `/personal-readme` or ask Claude Code for a GitHub profile README task. [Claude Code skill documentation](https://code.claude.com/docs/en/skills)

## ChatGPT and other agents

Where custom skill upload is available, use the Skills page’s **Create → Upload from your computer** with the complete skill packaged for that interface. If your agent supports only manual use, ask it to read the package’s `SKILL.md` and follow the linked references. [ChatGPT skill documentation](https://help.openai.com/en/articles/20001066-skills-in-chatgpt) · [Agent Skills specification](https://agentskills.io/specification)

The folder format was validated and local file copying was checked. The installation locations are documentation-checked. Native discovery, upload, and interactive CLI behavior have not been exercised independently across these hosts. The paired evaluation used explicit skill loading by Work Mode agents.

## Output layout

Keep the generated `README.md` and its referenced assets together. GitHub profile READMEs belong in a public repository whose name matches the account, with a nonempty `README.md` at the repository root. Apply reviewable drafts to that repository only when you authorize it. [GitHub profile README guide](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme)
