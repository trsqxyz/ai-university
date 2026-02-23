# AI University — Interactive Lifelong Learning Skill for Claude

Turn Claude into your personal university. Any subject, any level, dialogue-based.

## What is this?

AI University is a custom skill for Claude Projects that transforms Claude into an interactive tutor. It conducts a structured intake to understand your learning goals, builds a personalized syllabus, and delivers lectures through dialogue — with built-in fact-checking on every response.

## Features

- 🎯 Personalized intake — 6 questions to tailor everything to you
- 📚 Structured syllabus — based on standard academic curricula, customized to your interests
- 💬 Interactive lectures — one concept at a time, with comprehension checks
- 📋 Built-in audit — every response includes fact-checking notes
- 🔗 Cross-domain connections — links concepts across different courses
- 📝 Session handoff — resume your learning across conversations
- 🌐 Multi-language — automatically matches your language

## How it works

```
You: "I want to learn about behavioral economics"
     ↓
Intake (6 questions): motivation, profile, level, interests, learning style, communication preferences
     ↓
Syllabus: structured chapters with recommended resources
     ↓
Interactive lectures: concept → explanation → comprehension check → audit note
     ↓
Handoff document: paste into next conversation to continue
```

## Setup (2 minutes)

1. Open [Claude.ai](https://claude.ai) (requires Pro, Team, or Enterprise plan)
2. Create a new Project
3. In the Project's system prompt or knowledge base, paste the contents of `SKILL.md`
4. Start a conversation within the Project and say something like:
   - "I want to learn about nutrition"
   - "Teach me about investment fundamentals"
   - "社会学について学びたい" (works in any language)

That's it. No API keys, no setup, no coding required.

## Resuming a session

At the end of each learning session, AI University automatically generates a handoff document. To continue where you left off:

1. Start a new conversation in the same Project
2. Paste the handoff document
3. Say "Let's continue"

## Customization

The skill adapts to you through the intake process, but you can also:

- Adjust the syllabus after it's generated ("Can we add a chapter on X?")
- Change pace mid-course ("This is too basic, let's go deeper")
- Ask for sources anytime ("What's the evidence for that?")
- Branch into tangents (they're saved as future course candidates)

## Examples of what you can learn

Anything. The skill is domain-agnostic. Some examples:

- Nutrition science
- Behavioral finance / investment
- Climate change
- Psychology
- Sociology
- Coffee roasting science
- Philosophy
- Machine learning
- Music theory
- Art history

## The audit system

Every lecture response includes an audit note:

```
📋 Audit Note
Facts: 3 confirmed / 1 unconfirmed
Interpretations: 2 valid / 1 with multiple viewpoints
Notes: The 15% figure is from a 2019 study; more recent data suggests 12-18% range
```

This keeps you informed about the reliability of what you're learning. Ask "what's the source?" anytime for details.

## Limitations

- Learning continuity depends on handoff documents (Claude doesn't have persistent memory across conversations within the same Project by default)
- Web search quality varies — the audit system flags uncertainties
- Very niche or cutting-edge topics may have limited source material
- Long courses may approach context window limits in a single conversation

## License

MIT — use it however you want.

## Credits

Created by [d16e](https://d16e.com). Designed for Claude by Anthropic.
