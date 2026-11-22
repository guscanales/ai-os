# Intro to LLMs

Fictional course notes from 2026-10-10, revised 2026-11-21. No real school is implied.

## Core ideas

A token is a chunk of text the model processes. Context is the material available in a particular request. It is different from durable notes saved in the vault.

Retrieval selects source passages before the model answers. It can improve access to facts, but a retrieved passage may be stale or irrelevant. Keep source links beside an answer.

## Worked example

Question: when should a card payment be made? Retrieve [[Areas/Money/Debt Plan]], then state the planned date and distinguish a projection from an actual payment. Do not claim that a payment was sent.

## Check understanding

| Question | My answer |
|---|---|
| Why keep Markdown memory? | It survives switching models and conversations |
| What is retrieval recall? | How often the needed evidence appears in the retrieved set |
| Does fluent output prove correctness? | No, compare the answer with the source |

Next question: if the correct passage is retrieved but the answer is wrong, what should we measure next?
