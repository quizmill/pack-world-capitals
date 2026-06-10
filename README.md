# Capitals of the World — quizmill learning pack

An **expert-level** practice question bank for the capital cities of the
world — 45 multiple-choice questions spanning five continents, with a
deliberate focus on the capitals people reliably get wrong: moved
capitals (Astana, Naypyidaw, Nusantara), multiple-capital countries
(South Africa, Bolivia, the Netherlands), and classic confusion pairs
(Australia → Canberra, Côte d'Ivoire → Yamoussoukro).

This is a learning pack for [quizmill](https://github.com/quizmill/quizmill),
the open-source practice-app engine: the pack is pure JSON, and the
engine turns it into an installable, offline-first practice app with a
mistakes-review loop.

**▶ Try it: https://world-capitals.quizmill.dev**

| Continent | Questions | Sample traps |
|---|---|---|
| Europe | 9 | Netherlands (Amsterdam vs The Hague), Switzerland's federal city Bern |
| Asia | 10 | Kazakhstan → Astana, Myanmar → Naypyidaw, Indonesia → Nusantara |
| Africa | 10 | Côte d'Ivoire → Yamoussoukro, Tanzania → Dodoma, South Africa's three capitals |
| The Americas | 10 | Bolivia (Sucre vs La Paz), Chile's congress in Valparaíso, Belize → Belmopan |
| Oceania | 6 | Palau → Ngerulmud, Micronesia → Palikir, Nauru (no official capital) |

Difficulty skews hard (~60% at levels 4–5), with a few easy warm-ups.
Every explanation teaches why the answer is right *and* why the tempting
distractor is wrong.

## Run it

```
git clone https://github.com/quizmill/quizmill
cd quizmill && npm install
npm run pack:use quizmill/pack-world-capitals
npm run dev
```

`npm run build` then produces a fully static app in `out/` — deploy it
to any static host and install it to your home screen (it works
offline).

## Sources & review status

All 45 questions are LLM-authored (`source: "generated"`) and currently
carry `reviewStatus: "draft"` — the facts were cross-checked at authoring
time (including the tricky moved/multiple-capital cases), but they have
not yet had a formal human review pass. Corrections welcome.

## Contributing

Corrections and new questions are welcome via PR. From a quizmill
checkout, validate your changes with:

```
npm run pack:validate /path/to/pack-world-capitals
```

Question ids are immutable once published (users' attempt history points
at them) — never renumber existing questions; add new ones.

## License

MIT — see [LICENSE](LICENSE).
