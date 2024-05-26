# AnkiTemplate
A minimalist Anki deck template, with vocab, kanji and cloze card types

## Installation

Download `Sample deck.akpg` and import into Anki

## How to use

The deck has three note types; there are a few examples of each note type included to give you some idea of how it looks and what it can do. Some comments on these:

- The vocabulary note type produces up to four cards: kanji to reading, kanji to meaning, meaning to reading, and audio to reading. If the "Reading" field is blank on a card, it is assumed to be kana-only and the second card type is not produced. Of course, if there is no audio, then the fourth card type is not produced.

- The kanji note type makes two cards: kanji to reading, and kanji to meaning. There are fields for both on'yomi and kun'yomi readings, but also a "main reading" field which determines the reading which is tested.

## Yomitan integration

If you use yomitan, you may be interested to download `anki-templating.hbs`. In the yomitan settings, under "Anki", you can select "Configure Anki card templates…" and copy-paste the contents of the above file into the top text area at the bottom. The settings I use under "Configure Anki card format…" are then as follows, for vocab:

- Word: `{expression}`
- Reading: `{first-reading}`
- Other readings: `{other-readings}`
- Meaning: `{definition-1}`
- Other meanings: `{all-but-first-definition}`
- Part of speech: `{tags}`
- Audio: `{audio}`
- Sentence 1 JA: `{example-1-jp}`
- Sentence 1 EN: `{example-1-en}`
- Sentence 2 JA: `{example-2-jp}`
- Sentence 2 EN: `{example-2-en}`
- Sentence 3 JA: `{example-3-jp}`
- Sentence 3 EN: `{example-3-en}`

and for kanji:

- Kanji: `{character}`
- On'yomi: `{onyomi}`
- Kun'yomi: `{kunyomi}`
- Meaning: `{kanji-meanings}`
