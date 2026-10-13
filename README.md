# Mami Quiz

A standalone Albanian midwifery quiz application copied from nursery-quiz. The original React quiz engine, styling, answer feedback, scoring, shuffle, and exit behavior are preserved.

## Development

```bash
npm install
npm run dev
npm run build
npm run lint
```

## Questions

The 15 starter topics have empty JSON arrays in `src/questions/mami/`. Topic names are editable in `src/data/structure.json`. No clinical questions have been added.

Each question uses `{ id, question, answers, correct, explanation }`, optionally with `image` and `imageAlt`. Use globally unique stable IDs, for example `mami-lindja-001`. `correct` is a zero-based answer index. Images belong in `public/question-images/`.

Until questions are added, starting a quiz shows the existing empty-topic message. Lessons use all questions; exams randomly select up to 50.

This app has no backend, accounts, or browser persistence. Netlify static build settings are included; hosting is not configured.