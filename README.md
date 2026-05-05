# Long-Form Research Conversation Handoff Prompt

A prompt template for creating structured Markdown handoff files when a long GPT research conversation becomes too long, slow, or difficult to continue.

This is **not a normal summary prompt**. It is designed to preserve research continuity so a new GPT conversation can continue from the current state without restarting from zero.

---

## What It Does

This prompt asks GPT to generate a downloadable Markdown handoff file that preserves:

- Research topic and direction
- Confirmed decisions
- Current progress
- Files, paths, datasets, and outputs
- Statistical or methodological details
- Code, Git, or pipeline status
- Open issues and blockers
- Immediate next actions
- User preferences and corrections
- Uncertain or unavailable information

---

## When to Use

Use this prompt when:

- A single research conversation has become too long or laggy
- You need to move the work into a new GPT chat
- You want to preserve research context, files, decisions, and next steps
- A simple summary would lose too much detail

---

## Best For

- Scientific research
- Literature reviews
- Thesis or manuscript writing
- Experimental result interpretation
- Statistical analysis
- Computational pipelines
- Code / Git / Codex-assisted workflows
- Research documentation

---

## Not For

This prompt is not meant for short or casual chats, such as:

- Travel planning
- Stock discussions
- General brainstorming
- Daily conversation
- Multi-topic casual chats

---

## Files

Main prompt:

```text
prompt/long_form_research_handoff_prompt.txt
```

Recommended repository structure:

```text
long-form-research-handoff-prompt/
├── README.md
├── LICENSE
├── CHANGELOG.md
└── prompt/
    └── long_form_research_handoff_prompt.txt
```

---

## How to Use

1. Open the long GPT research conversation you want to transfer.
2. Copy the full prompt from:

```text
prompt/long_form_research_handoff_prompt.txt
```

3. Paste it at the end of the old conversation.
4. Ask GPT to generate the Markdown handoff file.
5. Start a new GPT conversation.
6. Upload the generated handoff file.
7. Ask the new GPT to continue from the **Immediate Next Action** section.

---

## Suggested Prompt for the New Conversation

After uploading the generated handoff file, paste:

```text
I am continuing a previous long-form research conversation. Please read the attached Markdown handoff file first and treat it as the active memory of the previous conversation.

Do not restart the work, reinterpret the research direction from zero, or invent missing facts.

Continue from the “Immediate Next Action” section and preserve the confirmed decisions, research logic, files, paths, terminology, and constraints.
```

---

## Key Features

- Research-focused handoff structure
- Confirmed / inferred / uncertain information separation
- Source reliability labels
- Verification status labels
- Execution evidence priority
- Missing file handling
- No redesign without cause
- Emergency continuity block
- Fallback behavior if file generation fails

---

## Privacy Note

Before publishing examples or generated handoff files, remove:

- Private research data
- Unpublished results
- Personal information
- Student or patient information
- Internal file paths
- API keys or credentials
- Private repository names

The prompt template itself is safe to publish if it does not contain project-specific confidential content.

---

## License

MIT License.

See `LICENSE` for details.

---

## Version

Current release:

```text
v1.0.0
```
