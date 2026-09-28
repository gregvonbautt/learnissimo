# Learnissimo — Design

## Content tree

Learnissimo's content — topics, sections, statements, quiz items, and source links — is represented as a single recursive tree of two node types.

A **container** is a node with an ordered list of children, where each child is either another container or a leaf. A **topic** is a container with no parent; a **section** is a container with a parent. The order of a container's children encodes the intended reading and learning order of the underlying material.

A **leaf** combines:
- an optional **statement**: free text, which can express one idea or several
- zero or more **quiz items**
- zero or more **source links**

A leaf needs a statement, at least one quiz item, or both — a leaf with none of these has no reason to exist.

A **source link** is typed by the kind of source it points to — for example, a position within a PDF, or a URL — carrying whatever fields that type needs to take the user to the exact spot: opening a PDF at that position, opening a URL in a new tab, or rendering the referenced content inline. A leaf's source links are shared by its statement and all of its quiz items; there is no separate link per quiz item.
