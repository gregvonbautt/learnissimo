# Learnissimo — Requirements

- Learnissimo works with multiple types of sources, starting with PDF documents (referenced by an exact position within the PDF) and web pages (referenced by a URL), and extending to other source types over time.
- A quiz item is grounded in a single fact and takes the form of a task such as a single-choice question, a multiple-choice question, an ordering task, or similar.
- A quiz item can optionally carry a brief text statement of the fact it is grounded in, separate from the task itself.
- Quiz items are organized into ordered sections, and sections can be organized hierarchically, mirroring the chapters or topics found in the sources.
- A section can combine quiz items drawn from several sources, so a topic can be covered using facts pulled from wherever they come from.
- A user can manually edit quiz items and the section structure in a convenient way. There is also some way to bootstrap quiz items automatically from a source, including adding to or merging with an existing knowledge base rather than only starting fresh. The exact set of modes for creating and modifying quiz items, including anything in between manual and automatic, is to be worked out during implementation.
- A quiz item can optionally link back to an exact source location, so the user can jump back and reread it at any point; some quiz items stand on their own without a source reference.
- A user can take a quick refresher or a full, thorough quiz over a section; the size and makeup of the quiz follows from which mode they pick. The quiz items used and their order vary from one attempt to the next (exact mechanics TBD).
- Learnissimo keeps a detailed history of every attempt — which quiz items were shown, what was answered, and whether it was correct.
- Using that history, Learnissimo shows the user, for any section, how well they know it, a confidence level based on how many times it's been quizzed, and how that has changed over time.
- The system runs in a browser, works well on mobile with an eye toward taking quizzes in short, on-the-go moments, and uses third-party login (Google, Facebook, or similar).
