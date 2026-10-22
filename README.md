# ☁️ AZ-900 Smart Quiz Builder (Unofficial)

An unofficial study tool for learners preparing for the Azure Fundamentals (AZ-900) exam. Built for the Power Learn Project Africa "Vibe Code for Learning" hackathon.

> Not affiliated with or endorsed by Microsoft. All practice questions are original and written for learning. No real exam questions are used.

## What it does

- **Smart Quiz Builder:** original practice questions across four topics (Cloud Concepts, Core Services, Security & Governance, Cost & SLA).
- **Instant explanations:** every answer shows why it is right in plain English.
- **AI explanations:** an "Explain it simply" button gives a beginner-friendly explanation with a real-life African analogy, in English or Swahili. An AI Study Buddy box answers any AZ-900 concept question. (Available on the Claude-hosted version; on other hosts the quiz works without it.)
- **Readiness Tracker:** accuracy per topic and overall, saved in the browser, with a simple readiness message.

## Live prototype

LIVE_LINK_HERE

## Run locally

Open `index.html` in any browser. No build step or dependencies.

## How it was built

Vibe-coded with Claude as an AI pair-programmer: I defined the learner problem, chose the features, reviewed and edited the questions, and iterated on the design. Single-file HTML, CSS and JavaScript; progress is stored with `localStorage`.

## Prompt engineering

Every AI call is built from a purposeful prompt with five parts:

1. **Role:** "You are a friendly AZ-900 tutor."
2. **Context:** the exact question, options and correct answer, so the explanation matches the quiz.
3. **Guardrails:** stay within the public AZ-900 skills outline, never invent Azure facts, and politely decline off-topic questions.
4. **Audience and style:** plain words for beginners, one African analogy (M-Pesa, matatus, mama mboga shops), under 120 words.
5. **Output format:** reply in the learner's chosen language and end with a "Remember:" memory hook of at most 8 words.

## Roadmap

- Larger question bank and timed mock mode
- Spaced-repetition review of missed questions

## Author

Nicole Muthee
