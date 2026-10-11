# What AI is good at, and where it fails

## Outcome

After this lesson you can look at a task and say whether AI is likely to do it well, do it badly, or do it well only if you check the result.

## Why it matters

People new to AI tend to make one of two mistakes. Some trust it with everything and get caught by a confident error in front of a client. Others see one error and decide it is useless. Both miss the point. An assistant is very good at some kinds of work and unreliable at others, and the dividing line is fairly predictable once you have seen it.

## The idea

An assistant writes the most plausible continuation of what you gave it. That makes it strong wherever "plausible and well-formed" is what you need, and risky wherever "exactly right" is what you need.

**Where it is strong**

- **Drafting and rewriting.** Emails, summaries, job descriptions, proposals. Changing tone, length or audience.
- **Working on text you supply.** Summarising a report, pulling action items out of notes, comparing two versions of a document.
- **Explaining.** Taking a concept you half understand and explaining it at your level, with examples, as many times as you need.
- **Generating options.** Twenty names, ten angles for a pitch, five ways to structure a workshop.
- **Structuring mess.** Turning rambling notes into a table, a plan or a checklist.
- **Critiquing.** Finding gaps, weak arguments and unclear sentences in your work when you ask it to.
- **Routine technical work.** Spreadsheet formulas, simple scripts, data cleanup.

**Where it fails, and what the failure looks like**

1. **Made-up facts.** Asked for a source, a statistic, a quotation or a legal case, the assistant may produce one that looks right and does not exist. In 2023 two New York lawyers filed a court brief citing six cases that ChatGPT had invented. The judge fined them and their firm $5,000 (Mata v. Avianca). The cases had realistic names, courts and quotations. Nothing in the text looked wrong.

2. **Out-of-date knowledge.** The model's knowledge stops at a training date. Ask about a tax threshold, a product price or who holds a job, and you may get an answer that was true a year ago. If the assistant searches the web it can do better, but only if it actually searched.

3. **Arithmetic and counting.** A language model is not a calculator. It can get a long multiplication wrong, miscount items in a list, or add a column and be off by a little. Many assistants can now run real calculations with a built-in tool, and when they do, the result is reliable. When they just "say" a number, treat it as a guess.

4. **Your specifics.** It does not know your company's policy, your customer's history or what was agreed in Tuesday's meeting unless you tell it. It will fill the gap with something typical instead of saying it doesn't know.

5. **Agreeing with you.** Assistants lean towards being agreeable. Ask "Is this a good plan?" and you tend to hear that it is. You have to ask for the weaknesses directly.

**A simple rule for deciding**

Ask two questions about any task:

- *Would I recognise a wrong answer?* If you can check it quickly, by reading the draft or testing the formula, use AI freely.
- *What does a wrong answer cost?* If an error would embarrass you, cost money or harm someone, verify against a source you trust, however good the answer looks.

Easy to check and low cost: go ahead. Hard to check and high cost: AI can help you prepare, but the answer needs independent verification.

## Worked example

Daniel is a finance analyst preparing a note on travel spending. He asks:

```
Our travel spend by quarter last year was 184,300, 212,750, 167,900 and
241,600. What's the total, the average, and the percentage change from
Q1 to Q4? Also, what is the typical travel spend as a share of revenue
for mid-sized professional services firms? Give a source.
```

The reply is neat and confident. Daniel checks it three ways.

- **The arithmetic.** He adds the figures himself: 806,550. He checks what the assistant gave. If it ran a calculation tool, it matches. If it did not, this is where a slip of a few thousand can appear. He then asks, "Show the calculation step by step using your analysis tool", and gets a verified figure.
- **The benchmark.** The assistant says "typically 2 to 4% of revenue" and names a survey. Daniel searches for the survey. He cannot find one with that title. The number may be roughly sensible, but he cannot cite it, so it stays out of the note.
- **The framing.** He asks the assistant to draft the commentary paragraph from his verified numbers. It is clear and well organised, which is the kind of work it is good at.

In the end he used AI for the writing and the structure, verified the arithmetic, and dropped the unsourced figure.

## Try it on your own work

1. List five tasks from your last working week.
2. For each, answer the two questions: would I recognise a wrong answer, and what would it cost?
3. Mark each one **go ahead**, **use and check**, or **verify independently**.
4. Take one "go ahead" task and do it with your assistant now.
5. Ask your assistant a factual question in your own field to which you already know the exact answer. See how it does. This calibrates your trust better than anything you can read.

## Ignore for now

- Benchmarks and league tables comparing models. They rarely predict how a tool will do on your tasks.
- Specialised AI products for law, medicine or finance. Learn the general tools first.
- Predictions about what AI will be able to do in five years. Work with what it does today.

## In the module session

The instructor shows each failure happening live, explains why fabrication occurs and why it cannot simply be switched off, and works through borderline tasks from your own jobs to decide which category they fall in.

## Check yourself

1. Why were the invented court cases so hard to spot?
2. An assistant gives you a total for twelve numbers. How do you find out whether to trust it?
3. Name one task of yours that is hard to check and costly if wrong. How would you use AI on it safely?
