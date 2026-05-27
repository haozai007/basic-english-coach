# Word List Guidance

This file is a compact working guide, not a full scholarly edition of Ogden's Basic English word list. If the user asks for exact historical completeness, verify against a reliable source before claiming exact coverage.

## Learning Groups

Use groups instead of alphabetical order when teaching.

### High-Use Operators

be, have, do, make, get, give, take, put, come, go, keep, let, see, say, seem, send, may, will

### People And Work

man, woman, person, people, friend, group, company, office, work, worker, owner, manager, customer, user, help, need, order, request, question, answer, problem

### Things And Information

thing, part, place, time, day, week, year, number, name, word, letter, account, list, note, copy, form, document, report, example, fact, news, idea

### Actions For Daily Practice

ask, answer, change, check, choose, come, do, get, give, go, have, keep, know, learn, make, move, open, put, read, say, see, send, take, talk, use, wait, write

### Qualities

able, bad, better, clear, different, early, good, great, high, important, late, little, long, low, new, old, open, public, ready, right, same, short, simple, small, strong, true, wrong

### Direction And Relation

about, across, after, against, among, at, before, between, by, down, for, from, in, into, near, of, off, on, out, over, through, to, under, up, with

## Vocabulary Drill Template

For each word:

1. English word
2. Chinese meaning
3. Simple English meaning
4. Basic-English-like example
5. User-context example
6. Memory hook
7. One recall question
8. Next review time

## Ebbinghaus-Style Spaced Review

Use this schedule as the default memory system for vocabulary. It follows the spirit of the Ebbinghaus forgetting curve: review soon after learning, then increase the interval.

### Default Review Intervals

For a newly learned word, schedule reviews at:

- 20 minutes later: quick recall.
- 1 day later: meaning and example recall.
- 2 days later: Chinese-to-English recall.
- 4 days later: fill-in-the-blank.
- 7 days later: sentence creation.
- 15 days later: mixed review.
- 30 days later: long-term check.

When exact dates are useful, calculate them from the user's current date. If exact dates are unknown, use relative intervals such as "tomorrow" or "in 4 days".

### Review Status

Use these labels after checking the user's answer:

- Again: wrong, blank, or only guessed. Review again in this session and tomorrow.
- Hard: partly right but slow or uncertain. Review tomorrow and in 2 days.
- Good: correct with minor hesitation. Review at the next planned interval.
- Easy: correct and quick. Move to the next longer interval.

### Daily Vocabulary Flow

For a daily lesson, use this order:

1. Due review words: test first, do not show answers first.
2. Error repair: explain only the words the user missed.
3. New words: teach 6 to 10 words unless the user asks for more.
4. Active use: ask the user to make 3 short sentences.
5. Schedule: list the next review time for each new or missed word.

### Same-Session Review

For words marked Again, test them again after 5 to 10 minutes or at the end of the lesson. Use a different question type, not the exact same prompt.

### Review Log Format

When the user wants a trackable plan, output a compact log:

```text
Word | Status | Next review | Note
make | Good | tomorrow | remember: make a change
clear | Again | end of lesson + tomorrow | confused with clean
```

The user can paste this log into a later chat to continue the review.

### Planning Pattern

When the user asks for study planning, suggest:

- Day 1: learn 8 to 10 words, then review after 20 minutes if possible.
- Day 2: review Day 1 words, add 6 to 8 new words.
- Day 3: review Day 1 and Day 2 due words, add fewer new words if there are many mistakes.
- Day 4: review Day 1 words with sentence creation.
- Day 7: mixed Chinese-to-English sentence practice.
- Day 15: workplace phrase practice using old words.
- Day 30: long-term recall check.

## Quiz Types

- English to Chinese meaning.
- Chinese to English word.
- Fill in the blank.
- Choose the simpler sentence.
- Make one sentence with the word.
- Listen-and-type style prompt, if the user practices pronunciation separately.
