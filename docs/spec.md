# Learnissimo — Specification

## Data model

A **source** is a document a fact can be grounded in — a PDF, referenced by an exact position within the document, or a web page, referenced by a URL. A source is optional: a fact does not need one, and where it has one, it can have more than one.

A **fact** is a single unit of knowledge. It may be extracted from a source, entered directly by the user, or be a pass-through reference to a source location with no separate text of its own. It can optionally carry a brief text statement of what it says.

A **quiz item** is a task that checks a fact — a single-choice question, a multiple-choice question, an ordering task, or similar. A quiz item can optionally reference a fact, and several quiz items can reference the same fact. A quiz item can also link directly to a source location, whether or not it references a fact.

A **section** is an ordered collection of quiz items. Sections form a hierarchy, mirroring the chapters or topics found in the sources. A section is not tied to a single source: the quiz items it contains can be grounded in facts from different sources.

## Creating and editing

A user can directly create and edit sources, facts, quiz items, and the section structure.

Learnissimo can also bootstrap facts and quiz items automatically from a source, adding them into a new section or merging them into an existing one. The exact division of labor between manual and automatic modes, and anything in between, is not yet specified.

## Taking a quiz

A user takes a quiz against a section by picking a mode — for example, a quick refresher or a full, thorough pass — which determines the number and makeup of quiz items used. The quiz items selected and their order vary from one attempt to the next. The exact selection and ordering mechanics are not yet specified.

## History and progress

Every attempt is recorded in full: which quiz items were shown, what the user answered, and whether each answer was correct.

For any section, Learnissimo derives, from this history:
- a measure of how well the user knows it
- a confidence level for that measure, based on how many times its quiz items have been answered
- a trend showing whether it has improved or degraded over time

The exact formulas behind these measures are not yet specified.

## Access and platform

Learnissimo is a web application, usable from a browser. It is responsive, and its mobile experience is fully usable, since taking a quiz is expected to happen in short, on-the-go moments. Access is authenticated through a third-party provider, such as Google or Facebook.
