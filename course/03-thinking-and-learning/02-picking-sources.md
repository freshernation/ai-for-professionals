# Picking the few sources worth your time

## Outcome

After this lesson you can choose a handful of trustworthy sources on a new topic, and set your assistant up to answer from those sources instead of from the open internet.

## Why it matters

On any topic there are a few sources that deserve your attention and thousands that do not. The hard part of learning or researching something new is rarely a shortage of information. It is knowing which three or four things to read. Choosing is a separate skill from reading, and most of us were never taught it. An assistant can help you choose. Once you have chosen, it can work from your selection alone, which makes its answers far more reliable.

## The idea

**Step 1: Map the territory before you pick**

When a topic is new, you do not yet know what kinds of source exist. Ask the assistant to lay out the field first:

```
I need to get up to speed on [topic] for [purpose]. I'm starting from
[what you already know].

Search for what's available and give me a map: the main kinds of
source on this topic, and for each kind, the one or two best examples
with links. Include official or primary sources, a good overview for
a newcomer, and the most respected expert voices.

Then tell me which three or four I should actually read, in what
order, which are too advanced for now, and what I can safely ignore.
```

This asks the assistant to do what a good librarian does. A librarian does not hand you everything. They tell you where to start and what to leave.

**Step 2: Know the kinds of source**

Sources fall roughly into four kinds, and each needs a different level of trust.

| Kind | Examples | Use it for |
|---|---|---|
| Primary | The law itself, the official statistics, the original study, the company's filed accounts | What is actually true or required |
| Expert synthesis | A regulator's guidance, a textbook, a review by a recognised authority | Understanding and overview |
| Commentary | News articles, opinion pieces, newsletters, podcasts | What people think it means |
| Interested parties | Vendor white papers, consultancy marketing, lobby groups | Their point of view, read as such |

A good set usually has at least one primary source and one expert synthesis. Interested parties often write the clearest explanations, and that is exactly why you should notice who is paying for the page.

**Step 3: Check a source by leaving it**

You cannot judge a source by how it looks. A professional design, a serious-sounding name and a list of references are easy to produce. In a 2017 Stanford study, professional fact-checkers judged unfamiliar websites faster and more accurately than historians and university students. The difference lay in what they did. The others stayed on the page and studied it. The fact-checkers left it almost at once and searched for what other sites said about the organisation behind it.

So spend one minute on three questions, answered away from the page itself:

- **Who is behind this?** Search the organisation's name. What do others say it is?
- **What do other reliable sources say about the same claim?**
- **Where did this claim originally come from?** Follow it back to the first source.

Your assistant can do this for you: "Who publishes this site, who funds them, and how are they regarded? Search for independent descriptions and ignore their own About page."

**Step 4: Make the assistant work from your sources**

Once you have your three or four, give them to the assistant and tell it to stay inside them:

```
Answer only from the documents I've attached. For each point, tell me
which document and section it comes from. If the documents don't
cover something, say so. Don't fill the gap from general knowledge.
```

This changes the quality of the answers. The assistant is no longer drawing on everything it has absorbed. It is reading the material you chose and reporting what that material says, and you can check each point against a page.

Three to five sources is enough to get oriented. A few good ones read properly will serve you better than many skimmed.

## Worked example

Hana is an HR director at a manufacturing company with sites in three European countries. New pay transparency rules are coming into force and the board wants a briefing. A search turns up hundreds of articles, most from law firms and HR software companies, all slightly different and many of them urgent in tone.

She asks her assistant for a map, using the prompt above and adding: "I know employment law in general terms but have not followed this. We operate in Germany, Poland and Ireland."

The assistant searches and returns a map: the directive itself; the European Commission's explanatory pages; national implementation pages for each of her three countries; two law-firm guides it describes as thorough; and a set of HR-vendor articles which, it notes, are written to sell pay-analysis software. It recommends four to read: the Commission's summary first, then one detailed law-firm guide, then the directive's key articles, then the national page for the country with the nearest deadline. It suggests leaving the vendor articles and the academic commentary for now.

Hana does not know the recommended law firm, so she asks: "Who is this firm, and how is it regarded in employment law? Search for independent sources." The assistant finds independent legal directory rankings that place the firm among the leading employment practices. That is good enough for a secondary source.

She downloads the four documents and loads them into a notebook tool. Then she asks:

```
Answer only from these four sources and cite the document and section
each time. What must an employer of our size do, and by when? Where
do the sources differ or leave something unclear?
```

The answer lists the obligations with a reference for each. It also flags that the law-firm guide gives a date for one country's implementation that the official national page does not confirm. Hana checks the national page, finds the legislation is still in draft, and marks that date as provisional in her briefing.

Had she asked a bare question such as "what do the pay transparency rules require?", she would have received a fluent general answer of unknown origin. What she has now is an answer she can trace line by line to documents she chose, with the one uncertain point visible.

## In your tool

- **Gemini:** Google's NotebookLM is built for this. You load sources into a notebook and it answers from them with citations to the passage. It can also turn the set into a spoken overview.
- **ChatGPT and Claude:** a project holds a set of files that every chat inside it can draw on. You can also attach files to a single chat.

Limits on how many sources you can add, and how large, depend on your plan.

## Try it on your own work

1. Pick a topic you need to understand better for your job.
2. Ask for a map with the prompt in step 1.
3. For one recommended source you do not recognise, check it by leaving it: who is behind it, and what do others say?
4. Choose three or four sources. Make sure at least one is primary.
5. Load them into a chat, project or notebook. Ask a real question with the "answer only from these" instruction.
6. Check two of the citations against the documents.

## Ignore for now

- Reading everything. The point of this lesson is to give yourself permission not to.
- Formal systems for rating evidence quality.
## In the module session

The instructor builds a source set live on a topic chosen by the group, shows how identical questions get different answers with and without chosen sources, and explains how these tools find the passage they quote.

## Check yourself

1. What are the four kinds of source, and which do you need at least one of?
2. What did the fact-checkers in the Stanford study do differently?
3. What does the instruction "answer only from the documents I've attached" change?
