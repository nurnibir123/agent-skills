# Agent Skills

Socratic modes for learning and coding with Codex while keeping the reasoning in your hands.

Inspired by Jane Street’s **socratic-tutor** skill from its [agent_skills repository](https://github.com/janestreet/agent_skills). The tutor here is adapted from that skill; the coder extends the idea to everyday software development.

## Skills

- [socratic-tutor](codex/socratic-tutor/SKILL.md): learn through questions, diagnostic placement, a skill map, spaced review, and a final assessment.
- [socratic-coder](codex/socratic-coder/SKILL.md): write the code yourself while the agent coaches, reviews your attempts, and runs tests and diagnostic commands.

Both stay active throughout the current conversation until you explicitly turn them off. Requests for a direct answer or help implementing a specific part are temporary exceptions, after which coaching resumes.

## Install for Codex

Copy either or both skill folders from `codex/` into `~/.codex/skills/` (or `$CODEX_HOME/skills` if you use a custom Codex home). Keep each skill in its own directory, including its `SKILL.md` and any license file. Existing installations should be backed up or compared before replacement.

## Use

Activate a mode with `$socratic-tutor` or `$socratic-coder`, followed by your topic or coding task. Say **“turn off socratic mode”** to return to ordinary assistance.

The agent may inspect files and run checks proactively. In coding mode, you write the implementation and tests unless you explicitly request an exception. Ask for a hint when stuck, or say **“show me the solution for this part”** for a direct answer.

Modes persist within a conversation. To continue in a new conversation, activate the mode again or use **“save state”** and provide the saved state there.

## Attribution

The adapted tutor retains Jane Street’s copyright notice and [MIT license](codex/socratic-tutor/LICENSE.md). This project is an independent adaptation and is not affiliated with Jane Street.
