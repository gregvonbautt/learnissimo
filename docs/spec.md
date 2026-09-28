# Learnissimo — Specification

## Content structure

A **topic** is the top-level unit of study — a knowledge domain, a book, a curriculum. A topic is organized as an ordered hierarchy of **sections**, nested to any depth, mirroring the order the material is meant to be learned in. A topic is simply the outermost section — the one with no parent.

At any point in that hierarchy, alongside further sub-sections, a user can attach a **statement** — free text capturing one or more ideas from what they are studying — and any number of **quiz items**, such as a single-choice question, a multiple-choice question, an ordering task, or similar. A point needs a statement, at least one quiz item, or both, to exist.

A statement and its quiz items can be linked to one or more exact locations in a **source** — a position within a PDF, or a URL — so the user can jump back and reread the underlying material. A source stands on its own, independent of any topic, and can be linked from many different topics.

## Creating and editing

A user can directly create and edit sources, sections, statements, and quiz items.

Learnissimo can also bootstrap statements and quiz items automatically from a source, adding them into a new section or merging them into an existing one. The exact division of labor between manual and automatic modes, and anything in between, is not yet specified.

## Taking a quiz

A user takes a quiz against any section, including a topic, by choosing how it is assembled along two dimensions: **order** — following the section's defined order, or randomized — and **size** — the whole section, or a portion sized to a time budget, such as a 10-minute or 20-minute attempt. The exact mechanics for selecting a partial attempt are not yet specified.

## History and progress

Every attempt is recorded in full: which quiz items were shown, what the user answered, and whether each answer was correct.

Answering a quiz item counts toward the section it belongs to and every section above it, up to the topic — so progress is visible at every level of the hierarchy, not only where the quiz item itself sits.

For any section, Learnissimo derives, from this history:
- a measure of how well the user knows it
- a confidence level for that measure, based on how many times its quiz items have been answered
- a trend showing whether it has improved or degraded over time

The exact formulas behind these measures are not yet specified.

## Access and platform

Learnissimo is a web application, usable from a browser. It is responsive, and its mobile experience is fully usable, since taking a quiz is expected to happen in short, on-the-go moments. Access is authenticated through a third-party provider, such as Google or Facebook.
