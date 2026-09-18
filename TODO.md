# Todo

I wanted to make a skill installer for codex, I think they took out the way to upload skills via the GUI in the ChatGPT deskop app but you can still drag things into CODEX_HOME/.codex/skills/. Currently the issue is the `$Skill Installer` command runs an agentic loop and consume tokens... I want to create my own installer that takes in GitHub links, recursively searches the file tree for files named SKILL.md and then copies the parent directory to the correct system skill path.

You can also press a button to open modal which allows you to drag and drop files that will be put into the correct skill directory. The modal stays open until the users presses esc or the red x button and everything that gets uploaded displays on a list.

This `desktop app` sends a request to a `GitHub` repo's URL to find files named SKILL.md, get the raw content, validate its structure, and then install it directly to the `~/.codex/skills/` directory.

