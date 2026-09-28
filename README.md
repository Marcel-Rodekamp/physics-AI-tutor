# Physics Study Tutor

**English** | [Deutsch](https://github.com/Marcel-Rodekamp/physics-AI-tutor/tree/main-german)

An AI study tutor for working through physics exercise sheets and lectures — built for a particle physics course following Griffiths, *Introduction to Elementary Particles*, but usable for any physics course.

It will **not** give you finished solutions. It asks what you've tried, gives hints one step at a time, checks your own results, explains concepts, and quizzes you on earlier material. The idea: you do the thinking, the AI makes the thinking easier.

## Why this way?

Studies of AI tutoring consistently find that when an AI hands students complete solutions, their homework improves but what they can do on their own afterwards gets *worse*. The same AI set up to give hints instead of answers removes that harm, and tutors that make you do the reasoning produce real gains. Getting answers feels more helpful — but that feeling turns out to be a poor guide to what you actually learn.

## Install

### Claude (claude.ai, desktop or mobile app)

Requires a Pro, Max, Team or Enterprise plan.

1. Download **[`physics-study-tutor.zip`](physics-study-tutor.zip)** from this repository (click the file, then the download button).
2. In Claude, open **Settings → Capabilities** and make sure **Code execution and file creation** is turned on.
3. Under Skills, click **Upload skill** and select the zip file.
4. Make sure the skill is switched on.

Claude uses the skill automatically when you ask about physics problems or lecture material. You can also ask for it explicitly: *"Use the physics study tutor for this."*

### Claude Code

Copy the `physics-study-tutor/` folder into `~/.claude/skills/`.

### Other AI tools (ChatGPT, Gemini, free Claude plan, …)

The skill is just a text file of instructions. Open [`physics-study-tutor/SKILL.md`](physics-study-tutor/SKILL.md), copy everything below the `---` header, and paste it into the tool's custom instructions — for example a ChatGPT project or custom GPT, a Gemini Gem, or a Claude project. Tools that support the open Agent Skills format can also load the folder directly.

## How to use it

- **Exercise sheets:** upload or paste the problem, then say what you've tried and where you're stuck. Expect questions back, not a solution.
- **Lecture review:** "Let's go through today's lecture on the quark model" — it will ask you to recall the key results first, then work through the steps with you.
- **Checking:** "I got X — is that right?" It will tell you whether it's right and, if not, *where* the mistake is, so you can fix it.
- **Quiz me:** "Quiz me on weeks 1–4" — one question at a time, mixed across topics.

**Be aware:**
- AI makes mistakes, especially in long calculations. Check results yourself with units, limiting cases and estimates.
- You can always bypass this by using AI without the skill. That's your choice to make — but consider what you want to be able to do on your own.

## Feedback

If the tutor gives away too much, too little, or behaves oddly, please open an issue or tell your tutor.
