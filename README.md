# Mitra — CMAT & MAH-CET Mentor

**Mitra** is a personal study companion for Indian MBA entrance exams **CMAT** (NTA) and **MAH MBA/MMS CET**.

It helps you aim for a **95 percentile** with:

- **Mentor chat** — ask concepts, shortcuts, day plans, or stress questions. Works offline with smart built-in replies; live AI mentor when `XAI_API_KEY` is set.
- **Practice** — original questions across Quant, DI, Logical, Verbal with explanations.
- **Topic tracker** — mark Core / High priority topics as Not started / Learning / Done.
- **Study plan builder** — realistic plans based on remaining days and daily hours.
- **Score strategy** — paper order, weekly rhythm, and review rules tailored to each exam.

Built with React, TanStack Router/Start, Tailwind CSS, and localStorage for progress.

## Quick start

```bash
npm install
npm run dev
```

Open http://localhost:8080

### Live mentor (optional)

Set the environment variable:

```bash
export XAI_API_KEY=your_xai_key
```

Without it, Mitra still answers common questions (plans, stress, percentages, etc.) from the built-in knowledge.

## Features at a glance

| Tab        | What it does                                      |
|------------|---------------------------------------------------|
| Chat       | Talk to Mitra about concepts, plans, or mindset   |
| Practice   | Timed-feel MCQs with immediate feedback + why     |
| Topics     | Track readiness on Core / High / Support topics   |
| Plan       | Generate a personalised study plan                |
| Score      | 95-percentile strategy & weekly rhythm            |

Progress (exam choice, topic status, mistakes) is saved in the browser.

## Exam coverage

- **CMAT** — Quant, DI, Logical (incl. syllogism), Language, Innovation & Entrepreneurship, GK awareness
- **MAH-CET** — Logical Reasoning, Abstract Reasoning, Quant, Verbal (no negative marking strategy)

## Tech stack

- React 19 + TypeScript
- TanStack Router & Start
- Tailwind CSS 4
- Vite
- Optional: xAI API for live chat

## Project structure

```
src/
  routes/
    index.tsx          # Main Mitra UI (all tabs)
    __root.tsx         # Document shell
  lib/mentor/
    content.ts         # Topics, questions, strategy
    chat.ts            # Server function for live mentor
  styles.css           # Design system (warm paper + teal)
public/
  favicon.svg
```

## Notes

- Auth and database features from the original scaffold are disabled (`VITE_AUTH_ENABLED=false`).
- Designed for desktop and mobile.
- All practice questions are original and educational; always cross-check official NTA / CET Cell notices for dates and pattern changes.

## License

MIT — feel free to fork and adapt for your own exam prep.

---

Made with care for students targeting 95 percentile.
