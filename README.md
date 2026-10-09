# Napishi: agent skills for writing and speaking like a human

[![skills.sh](https://skills.sh/b/iamursky/napishi)](https://skills.sh/iamursky/napishi)

![A blue fountain pen nib pulls tangled gray strips into clean blue lines](/.github/images/cover.webp)

Two language-specific skills help Claude, ChatGPT, and Codex write clear prose and handle difficult conversations without sounding bureaucratic, salesy, or machine-made.

The skills combine two crafts with the same foundation: respect for the person on the other side of the words. They cover writing, editing, storytelling, persuasion, feedback, negotiation, emotional conversations, and the patterns that make generated prose feel synthetic.

## Language versions

Each version uses native clichés, bureaucratic constructions, usage guidance, and examples. The English skill is an adaptation, not a literal translation of the Russian one.

| Language | Skill name | Folder                             |
| -------- | ---------- | ---------------------------------- |
| Русский  | `napishi`  | [skills/napishi/](skills/napishi/) |
| English  | `write`    | [skills/write/](skills/write/)     |

Each folder is independently installable and contains its own `README.md`, `SKILL.md`, and `references/` directory.

## What they do

Use the skills to:

- draft or edit emails, messages, posts, articles, landing pages, newsletters, reports, and documentation;
- cut clutter, nominalizations, bureaucratic language, corporate jargon, clichés, and unsupported claims;
- preserve voice and useful detail instead of reducing prose to a sterile summary;
- diagnose clusters of AI-writing patterns and rewrite them naturally;
- find a premise, structure a story, or get past writer's block;
- prepare for conflict, disagreement, bad news, negotiation, praise, or criticism;
- answer with empathy without becoming vague, flattering, or manipulative.

Neither skill is intended for code-generation requests.

## Installation

### Via `npx skills`

```bash
# Russian
npx skills add iamursky/napishi/tree/main/skills/napishi

# English
npx skills add iamursky/napishi/tree/main/skills/write

# Both
npx skills add iamursky/napishi
```

### ChatGPT

1. Download the folder for the language you need, including `SKILL.md` and `references/`.
2. In the ChatGPT sidebar, open **Plugins → Skills**.
3. Select **Create → Upload from your computer** and upload the skill folder.
4. Select the skill with `@`, or make a relevant writing or conversation request.

### Claude Desktop / Web

1. Download the entire folder for the language you need.
2. Go to **Customize → Skills → + → Upload a skill**.
3. Upload the folder. The skill will activate automatically for relevant requests.

### Manual install for Claude Code

```bash
git clone https://github.com/iamursky/napishi ~/napishi

ln -s ~/napishi/skills/napishi ~/.claude/skills/napishi
ln -s ~/napishi/skills/write ~/.claude/skills/write
```

### Codex CLI

```bash
git clone https://github.com/iamursky/napishi ~/napishi

ln -s ~/napishi/skills/napishi ~/.codex/skills/napishi
ln -s ~/napishi/skills/write ~/.codex/skills/write
```

Invoke the skills explicitly with `$napishi` or `$write`.

## How they activate

`napishi` applies to Russian prose and conversation. `write` applies to English prose and conversation. They trigger on requests to draft, rewrite, edit, shorten, humanize, remove AI-writing patterns, develop a story, or prepare for a difficult conversation. Requests to write code are excluded.

## Authorship

These skills are original workflows assembled from long-standing principles of writing, editing, rhetoric, negotiation, and humane conversation. They do not reproduce or replace any single source. The sections on AI-writing patterns draw on Wikipedia's “Signs of AI writing,” available under CC BY-SA.

## License

See [license](license).
