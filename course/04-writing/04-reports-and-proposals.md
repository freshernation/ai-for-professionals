# Reports and proposals

## Outcome

After this lesson you can produce a report or proposal of several pages with an assistant's help, working in stages so that the argument holds together and every figure is one you can stand behind.

## Why it matters

A long document that asks for a decision is the kind of writing with the most riding on it: a proposal for budget, a business case, a recommendation to the board. It is also where AI use goes most visibly wrong. Ask an assistant to "write a proposal for a new warehouse system" and you will get eight tidy pages with invented benefits, numbers from nowhere and a conclusion that fits any company. A reader who knows the business will see through it in a paragraph. The way to avoid that is to work in stages, bring the substance yourself, and use the assistant for structure, drafting and checking.

## The idea

**Don't ask for the whole document**

A long document produced in one go is generic and padded, and it is full of plausible invention, because the assistant has to fill every section whether or not you gave it anything to say. Work in stages.

**Stage 1: Reader and decision**

Before any writing, be clear about two things and tell the assistant both:

- **Who decides, and what do they care about?** A finance director reads for cost and risk. An operations director reads for disruption.
- **What exactly are you asking them to do?** Approve a sum, choose between options, or note a risk.

If you cannot state the decision in one sentence, the document is not ready to be written.

**Stage 2: Outline and agree**

```
I'm writing a [proposal/report] for [reader] asking them to [decision].
Here is what I know: [your notes, findings, figures].

Suggest an outline: section headings with two lines on what each must
establish. Tell me what a decision-maker would expect to see that I
haven't given you.
```

The last sentence of that prompt is the valuable one. It turns the assistant into a reviewer before you have written a word. Typical gaps it finds are the cost of doing nothing, the options you rejected, the risks, and what happens after approval.

Agree the outline before you draft.

**Stage 3: Gather the substance**

For each section, collect what is true: the data, the quotes, the costs, the findings. These come from you and your organisation. Where you lack something, go and get it, or mark it as missing. Do not let the assistant supply it.

**Stage 4: Draft section by section**

Give the assistant one section's material at a time:

```
Draft the "[section]" section. Use only the material below. Where
something is missing, write [NEEDED: what] instead of filling the gap.
Plain language, no more than [length].
```

Review each section before moving on. If you are working over several days, keep everything in one project or one long document, so that the assistant has the earlier sections in view.

**Stage 5: Write the summary last**

The summary at the front is the only part that some readers will read. Write it when everything else is settled. Ask for it to be drawn strictly from the document: "Write a summary of no more than 150 words: the decision asked for, the main reason, the cost, the main risk. Use only what is in the document."

**Stage 6: Check that it is consistent**

Long documents written in pieces contradict themselves. A figure is updated in one section and not in another. A term changes meaning halfway through. Ask:

```
Check this document for internal consistency. List every place where
a number, date, name or claim in one section doesn't match another
section. Also list any claim in the summary that the body doesn't
support.
```

Assistants are good at this check, and tired authors are bad at it. Verify each mismatch it reports. Do the arithmetic yourself, or have the assistant run the calculation with its analysis tool and show its working.

**Stage 7: Read it as the decision-maker**

Finally: "Read this as [the decision-maker]. What are the three questions you would ask before approving? What would make you say no?" Then answer those questions in the document, or have the answers ready for the meeting.

**The honest proposal**

A proposal that names its own weaknesses is more persuasive than one that hides them. Decision-makers know every plan has risks. If yours appears to have none, they will assume you have not looked. Use the assistant to find the weak points, and then deal with them in the open.

## Worked example

Omar is an operations manager at a company that distributes catering supplies from one warehouse. The warehouse runs on a fifteen-year-old system and a great deal of paper. He wants approval to replace it. The decision lies with the managing director and the finance director.

**Reader and decision.** He writes it down: *Approve 180,000 to replace the warehouse management system, to be live before the peak season in November.*

**Outline.** He gives the assistant his notes: supplier quotes, picking error rates, overtime costs, and the result of a two-week trial on one aisle. He asks for an outline and for what is missing.

The outline is sensible. The list of what is missing is more useful still:

> - **The cost of doing nothing.** You describe the benefits of the new system but not what the current one costs each year in errors, overtime and delays.
> - **Options considered.** Only one supplier and one approach are mentioned. A finance director will ask what else you looked at, including upgrading the existing system.
> - **Disruption during changeover.** You want to go live before peak. What happens to orders during the switch?
> - **What you are assuming.** The savings rest on the trial. How representative was one aisle?

Omar has answers to the first three in his head and on file. The fourth worries him, because it is a fair question.

**Substance.** He collects the material. Picking errors cost about 31,000 a year in returns and re-deliveries. Overtime that the trial suggests could be avoided comes to 44,000. He looked at two other suppliers and at an upgrade, and has notes on why he rejected each. On the trial, he writes down honestly that it covered the fastest-moving aisle, so the saving may be smaller across the whole warehouse.

**Drafting.** He drafts section by section. In the costs section, the assistant writes "[NEEDED: annual licence cost after year one]". He had left it out. It is 12,000 a year, and it changes the calculation.

**Summary.** Written last. It gives the decision, a saving of roughly 75,000 a year from fewer errors and less overtime, and payback "in under two years".

**Consistency check.** He runs the check. It returns:

> - The summary says payback is "under two years". Section 4 gives the cost as 180,000 and annual savings as 75,000, which is 2.4 years. If the 12,000 annual licence is deducted from the savings, net savings are 63,000 and payback is about 2.9 years.
> - Section 2 says the trial ran for "two weeks", and Section 5 says "ten working days". These agree, but the wording differs.
> - Section 3 says three alternatives were considered, and the table lists two.

The first of these would have been found by the finance director in the meeting. Omar does the arithmetic himself: 180,000 ÷ 63,000 = 2.86. He corrects the summary to "just under three years" and adds the missing alternative to the table.

**The decision-maker's reading.** He asks for the finance director's three questions. One is: "If the saving across the whole warehouse is half what the trial showed, does this still pay back?" He works it out. At half the saving the payback is too long. So he adds a short section saying so, and proposes a staged payment tied to results from the first month after go-live.

In the meeting the finance director asks exactly that question. Omar turns to the page. The proposal is approved with the staged payment.

## Try it on your own work

1. Pick a report or proposal you need to write. State the reader and the decision in one sentence each.
2. Give the assistant your notes. Ask for an outline and for what a decision-maker would expect that you have not provided.
3. Gather real material for the gaps. Mark what you cannot get.
4. Draft two sections, one at a time, with the [NEEDED] instruction.
5. When you have a full draft, write the summary last, then run the consistency check.
6. Ask for the decision-maker's three questions, and answer one of them in the document.

## Ignore for now

- Formatting and design. Get the argument right first.
- Asking for the whole document at once to "save time". It costs more time in the end.
- Long appendices. Include what the decision needs.

## In the module session

The instructor takes a proposal through the key stages, plants inconsistencies for the group to find with and without the assistant, and has the assistant read it as the decision-maker.

## Check yourself

1. Why does asking for a whole proposal in one request produce a poor result?
2. Why is the summary written last?
3. In the example, what did the consistency check find, and who would have found it otherwise?
