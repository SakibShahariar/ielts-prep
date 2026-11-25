# IELTS Prep — Band 8–9

Private collection of IELTS study notes and the OpenCode skills built to support them.
Target band: **8–9** (not merely 8+).

## Structure

```
ielts-prep/
├── writing/     Task 1 (classes 1–4), Task 2 (class 1), templates, linkers, model answers
├── reading/     Reading master book (all question types)
├── listening/   Listening master book (all question types)
├── speaking/    Speaking master book (all three parts)
└── skills/      Mirrors of the four OpenCode skills
```

## What is where

### writing/
- `IELTS-Writing-Task1-Band8-9-Notes.md` — master file: all Task 1 classes, synonym bank
- `IELTS-Writing-Task2-Band8-9-Notes.md` — master file: Task 2 class 1 (more classes to come)
- `task1-templates-by-type.md` — one fixed frame plus type-specific language
- `ielts-writing-linkers-and-synonyms.md` — linkers and adjective/adverb tables
- `task1-model-answers-practice.md` — full Band 8–9 model essays
- `archive/` — older duplicate per-class files, kept for reference

### reading/, listening/, speaking/
One master Band 8–9 book per section, each built from official IELTS sources.

### skills/
- `ielts-writing-teacher` — grades essay responses against the descriptors
- `ielts-reading-coach` — reviews answers with passage evidence
- `ielts-listening-coach` — reviews answers with transcript evidence
- `ielts-speaking-coach` — grades spoken answers against the official Band 8/9 descriptors

## Working locally

The four study folders are available at their original short paths via symlinks:

```
~/ielts-writing  ->  ielts-prep/writing
~/ielts-reading  ->  ielts-prep/reading
~/ielts-listening -> ielts-prep/listening
~/ielts-speaking ->  ielts-prep/speaking
```

Edits made through those paths are made directly inside the repo — no manual copying needed.

**Skills are different.** OpenCode loads skills from `~/.config/opencode/skills/`. The copies
in `skills/` are a mirror. After changing a skill locally, sync it with:

```bash
cd ~/ielts-prep
cp -r ~/.config/opencode/skills/<skill-name> skills/
git add -A && git commit -m "Update <skill-name> skill" && git push
```

## Status

- Task 1 classes 1–4: captured and upgraded to Band 8–9
- Task 2 class 1: captured; further classes expected
- Reading, Listening, Speaking: complete master books

All model answers are for learning patterns — never memorise them in the exam.
