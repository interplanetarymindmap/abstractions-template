---
prop-ipfoam-type-1630602741:
  defaultName: Abstract
  represents: An abstract of an attempt to express the abstraction-intent of the given note in written language. A short summary of what the abstraction is about. It is meant to communicate the more relevant parts of the subject note in order to facilitate the recognition of its abstraction intent.
  constrains:
    - interplanetary-text
    - Should give a high level overview of the the note content to the reader
    - Should not include the IID of the Note itself
    - Often responds to the question "What is my understanding of <abstraction>?"
    - Should be no more than one paragraph
  ipldSchema: type root [string]
---