# Deadpan Reductive Observation

A Codex agent skill for turning ordinary observations into concise, deadpan reductions that feel obvious in retrospect.

Instead of adding a conventional punchline, the skill strips away the subject's usual framing and describes what people are actually doing:

> a video meeting is just six people watching one person discover the mute button

## What it does

- Rewrites an observation as one short, confident, deadpan line.
- Finds the mundane behavior, contradiction, ritual, or inconvenience underneath the subject.
- Uses understatement instead of setup-and-punchline joke structure.
- Produces genuinely different angles when alternatives are requested.
- Researches current or subject-specific details when stronger, more topical options would benefit from them.
- Returns only the rewritten observation by default.

## Install

### With Codex Skill Installer

Ask Codex to install this repository:

```text
$skill-installer Install the skill from https://github.com/johndkane/deadpan-reductive-observation--agent-skill
```

### Manually

Clone the repository into your user skills directory.

macOS or Linux:

```bash
git clone \
  https://github.com/johndkane/deadpan-reductive-observation--agent-skill.git \
  "$HOME/.agents/skills/deadpan-reductive-observation"
```

Windows PowerShell:

```powershell
git clone `
  https://github.com/johndkane/deadpan-reductive-observation--agent-skill.git `
  "$env:USERPROFILE\.agents\skills\deadpan-reductive-observation"
```

Codex detects newly installed skills automatically. Restart Codex if the skill does not appear immediately.

## Use

Invoke the skill explicitly by mentioning it in your prompt:

```text
$deadpan-reductive-observation

Planning a weekend trip with friends usually involves lots of discussion, but nobody commits.
```

Expected style:

```text
a weekend trip with friends is just four group chats slowly agreeing not to go anywhere
```

You can also request alternatives or researched angles:

```text
$deadpan-reductive-observation

Give me eight genuinely different versions of this observation. Research the topic first and favor specific, recognizable behavior:

Grocery shopping while hungry makes you buy things you never planned to get.
```

Codex may also select the skill automatically when a request clearly asks for this style.

## Style principles

A strong result is:

- recognizably true;
- concrete rather than abstract;
- surprising without becoming elaborate;
- concise enough that nothing can be removed;
- observed rather than visibly “written”; and
- left unexplained.

The skill avoids forced catchphrases, elaborate metaphors, generic meme language, and minor rewrites presented as distinct alternatives.

## Repository structure

```text
.
├── SKILL.md           # Skill metadata and complete behavior instructions
├── agents/
│   └── openai.yaml    # Codex display metadata
└── README.md
```

This is an instruction-only skill. It has no runtime scripts or package dependencies.

## Development

Keep changes focused on the behavior defined in [`SKILL.md`](SKILL.md). The YAML frontmatter must retain a valid `name` and a concise, discriminating `description`; the remaining Markdown is the instruction set Codex loads when it invokes the skill.

Before submitting a change:

1. Confirm the skill still produces one concise line by default.
2. Test explicit invocation with `$deadpan-reductive-observation`.
3. Test an alternatives request for meaningfully different angles.
4. Verify factual or topical lines do not invent details.
5. Validate the skill structure with Codex's `skill-creator` tooling.

For the underlying format and discovery rules, see OpenAI's [Create skills documentation](https://developers.openai.com/docs/build-skills).
