# Learnissimo — Requirements

Learnissimo works with multiple types of sources. It starts with PDF documents, where a reference is an exact position within the PDF, and web pages, where a reference is a URL, and is meant to extend to other source types over time.

A test entry is grounded in a single fact and can take common shapes: single choice, multiple choice, ordering, and other equivalent shapes. Test entries are organized into ordered sections, and sections can be organized hierarchically, mirroring the chapters or topics found in the sources. A section is not tied to one source — it can combine entries drawn from several sources, so a topic can be covered using facts pulled from wherever they come from.

Creating and modifying tests works in three modes: fully automated, semi-automated through natural-language requests to change something, and manual, where anything can be adjusted directly.

Every test entry links back to its exact source location, so the learner can jump back and reread it at any point.

Taking a test isn't one fixed thing — a learner can take a quick refresher or a full, thorough pass over a section, and the size and makeup of the test follows from which mode they pick. The entries used and their order shouldn't be identical from one attempt to the next (exact mechanics TBD).

Learnissimo keeps a detailed history of every attempt — which entries were shown, what was answered, whether it was correct — and uses that history to tell the learner, for any topic or section, how well they know it, how confident that assessment is (based on how many times it's actually been tested), and how it has changed over time — improving or slipping.

The system is used through a browser, works well on mobile with an eye toward taking tests in short on-the-go moments, and sits behind third-party login (Google, Facebook, or similar) rather than its own account system.
