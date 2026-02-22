# Quran Word-by-Word

Open-source word-by-word data for every word in the Quran — meanings, transliteration, Arabic roots, morphology, and grammatical analysis.

## What's Included

### Word-by-Word Translation
For each of the ~77,000 words in the Quran:
- **Arabic text** (Uthmani script with diacritics)
- **English meaning**
- **Transliteration** (Latin script pronunciation)
- **Page number** and **line number** (Madinah Mushaf layout)

### Morphology & Roots
- **3-letter Arabic root** (e.g., كتب for كِتَاب)
- **Part of speech** — Noun, Verb, Particle, Adjective, Pronoun, etc.
- **Verb form** (Forms I–X)
- **Lemma** (dictionary form)
- **Gender, number, case** markers
- **Morphological segmentation** — prefixes, stems, suffixes

### Multi-Language Word Meanings
- English (primary)
- Urdu, Hindi, Indonesian, Bengali, Turkish, Tamil, French, German, and more

## Directory Structure

```
words/            # Word-by-word data per surah (JSON)
morphology/       # Root, POS, lemma, verb form data
translations/     # Word meanings in multiple languages
```

## Usage

```json
{
  "surah": 1, "ayah": 1, "position": 1,
  "text_uthmani": "بِسْمِ",
  "translation": "In (the) name",
  "transliteration": "bis'mi",
  "root": "سمو",
  "pos": "noun",
  "case": "genitive"
}
```

## Data Sources & Attribution

- Word-by-word meanings: [Quran Foundation API](https://api.quran.com/api/v4)
- Morphology: [Quranic Arabic Corpus](https://corpus.quran.com) (Dr. Kais Dukes, University of Leeds)
- Enhanced morphology: [mustafa0x/quran-morphology](https://github.com/mustafa0x/quran-morphology)
- Multi-language WBW: [QUL / Tarteel AI](https://qul.tarteel.ai)

## License

MIT — Free for personal and commercial use. See [LICENSE](LICENSE).

Morphology data from the Quranic Arabic Corpus is under GNU GPL. See individual source licenses.
