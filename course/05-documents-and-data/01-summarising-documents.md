# Summarising long documents accurately

## Outcome

After this lesson you can get an accurate, useful summary of a long document, and check it quickly enough that you can rely on it.

## Why it matters

Contracts, policies, reports and tender documents arrive faster than anyone can read them. Summarising is one of the things assistants do best. It is quick, and it is usually right, because the assistant is working from text you supplied. The risk is in the word "usually". A summary can drop the one condition that matters, soften a "must" into a "should", or state something that the document does not quite say. Because the rest of the summary is good, you do not notice. This lesson shows how to ask for a summary that serves your purpose, and how to check it in five minutes.

## The idea

**A summary needs a purpose**

"Summarise this" produces a general overview: a little about everything, in proportion to how much space each topic takes up. That is rarely what you need. A sixty-page contract spends forty pages on definitions and standard terms, and two paragraphs on the thing that will cost you money.

Tell the assistant why you are reading:

```
I'm [role], deciding whether to [decision]. Summarise the attached
[document] for that purpose. I need to know:
1. [question]
2. [question]
3. [question]

For each point, give the section or page number. Quote the exact
wording for anything that is an obligation, a deadline, a limit or
an amount. If the document doesn't address one of my questions,
say so.
```

Three parts of this matter:

- **Your questions.** The summary is built around what you need.
- **Section or page numbers.** These make it possible to check.
- **Exact quotes for the things that bind you.** A paraphrase of an obligation is where meaning slips.

**Extract, don't just summarise**

For anything with consequences, ask for extraction as well as summary: "List every date and deadline", "List every amount of money and what it is for", "List everything we are required to do". Extraction is more reliable than summary because the assistant is finding and copying. It is not compressing and rephrasing.

**How summaries go wrong**

Knowing the typical errors tells you where to look.

1. **Dropped conditions.** "The customer may terminate after the initial term with 90 days' notice" becomes "either party may terminate with 90 days' notice".
2. **Softened or hardened language.** "Shall" becomes "should". "May" becomes "will".
3. **Merged points.** Two separate rules are combined into one that is not quite either.
4. **Omissions.** Something important is left out, often an exception or a schedule at the back.
5. **Additions.** A detail appears that is typical of such documents but is not in this one.
6. **Lost in the middle.** In very long documents, material from the middle gets less attention than the start and the end.

**A five-minute check**

You do not need to re-read the document. Do these four things:

- **Spot-check three points.** Choose the three that matter most to your decision. Go to the section cited and read the original. Does it say that, with the same conditions?
- **Ask what was left out.** "What did you leave out of this summary that someone in my position might care about?" This often brings out an exception or a clause that seemed minor.
- **Ask for the surprises.** "Is there anything in this document that is unusual, one-sided or different from what is standard for this kind of document?"
- **Check the numbers and dates** against the extraction list.

If a spot-check fails, treat the whole summary with more suspicion and check further.

**Very long documents**

When a document runs to hundreds of pages, work in parts. Ask for a section-by-section outline first, then for detail on the sections that matter. Asking a focused question about one section gives a better answer than asking the assistant to hold everything at once. Check that the whole file was read: ask "What is the last section of this document?", and confirm that the answer matches.

**Scanned documents and tables**

A scanned PDF is a picture of text. Assistants can usually read it, with more errors than from a text document, particularly in figures, small print and tables. If the numbers matter, check them against the page.

**What a summary is for**

A summary tells you what a document says and where, so that you read the right parts yourself. It does not replace reading the clauses you will sign, and it is not legal advice. For anything binding, use the summary to direct your attention, then read the original wording of what matters.

## Worked example

Kofi is operations manager at a food wholesaler. The company's contract with its logistics provider is up for renewal, and the provider has sent a new agreement of 64 pages. The managing director wants to know by tomorrow whether there is anything to worry about. The company's solicitor will review it later in the week, and Kofi needs to know what to ask.

He uploads the contract into his company's approved assistant and writes:

```
I'm the operations manager at the customer. We are deciding whether
to renew on these terms. Summarise this agreement for that purpose.
I need to know:
1. How and when can either side end the agreement?
2. How can the price change during the term?
3. What service levels are promised, and what happens if they are missed?
4. What are we liable for, and are there limits?

For each point, give the clause number. Quote the exact wording for
any obligation, deadline, limit or amount. If the agreement doesn't
address something, say so.
```

The summary comes back in under a minute, organised under his four questions with clause references. On termination it says: "Either party may terminate with 90 days' written notice (clause 14.2)."

**Spot-check.** Kofi opens clause 14.2. It reads: "Following the Initial Term, the Customer may terminate this Agreement on not less than 90 days' written notice. The Supplier may terminate on not less than 180 days' written notice." The Initial Term is defined in clause 1 as 24 months.

The summary had dropped two things. The customer cannot leave for the first two years, and the notice periods are different for each side. Both matter. He tells the assistant, which corrects the point and apologises. He decides to check the other three points fully.

- **Price (clause 7).** The summary says prices rise annually in line with inflation. The clause says "by the percentage increase in the Consumer Prices Index plus three per cent". The "plus three per cent" was missing. He asks for the exact wording of every sentence in clause 7.
- **Service levels (clause 9 and Schedule 3).** The summary is accurate here. Delivery within the agreed window is promised 96% of the time, with service credits below that.
- **Liability (clause 16).** Accurate, with the cap correctly quoted.

**What was left out.** He asks. The assistant mentions Schedule 5, which lets the supplier add a fuel surcharge "at its reasonable discretion". It had not appeared under "price" because it sits in a schedule and not in clause 7.

**Surprises.** He asks what is unusual or one-sided. The assistant lists the unequal notice periods, the uncapped fuel surcharge, and an automatic renewal for a further 24 months unless notice is given six months before the end. Kofi had missed the last one entirely.

In forty minutes he has a one-page note for the managing director with four concerns, each quoted from the contract with its clause number, and four questions for the solicitor. The first summary was about four-fifths right. The fifth that was wrong included the two points that would have cost the most.

## Try it on your own work

1. Choose a long document you need to understand: a contract, policy, report or specification. Check that it may go into the tool you are using.
2. Write three or four questions you need answered, and your reason for reading.
3. Ask for a purpose-driven summary with section numbers and exact quotes for obligations, deadlines, limits and amounts.
4. Spot-check the three points that matter most against the original.
5. Ask what was left out, and what is unusual or one-sided.
6. Ask for a list of every date and every amount. Compare it with the summary.

## Ignore for now

- Summarising things you could read in two minutes.
- Tools that summarise every document automatically as it arrives. Summarise for a purpose.
- Treating a summary as a replacement for professional review of anything you will sign.

## In the module session

The instructor summarises a real document live, plants the typical errors for the group to find, and explains what happens inside the tool when a document is longer than it can hold at once.

## Check yourself

1. Why does "summarise this" give a poorer result than a summary built around your questions?
2. Name four ways a summary can go wrong.
3. What are the four steps of the five-minute check?
