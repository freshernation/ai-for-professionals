# Research with sources you can check

## Outcome

After this lesson you can use an assistant to research a question and come away with findings you can trace to real sources, instead of a confident summary you have to take on trust.

## Why it matters

Research is one of the most useful things an assistant does. It is also where an unchecked answer does the most damage. An assistant can read thirty web pages in the time it takes you to read one, and pull them into a tidy brief. It can also misread a page, lean on a weak source, or state something that no source says. The method in this lesson lets you keep the speed while making sure that what you rely on is real.

## The idea

**Two ways an assistant answers a question**

- **From memory.** It writes from what it absorbed in training. This is fast, often right about well-known things, and has no sources you can check. It may also be out of date.
- **From search.** It looks things up on the web, reads the pages, and writes from them, with links. This is slower, more current, and you can check it.

For anything you will rely on, you want the second. Most assistants search on their own initiative when a question seems to need it, but you should not assume they have. Say so: "Search the web for this and cite your sources."

**Research modes**

ChatGPT, Claude and Gemini each have a deeper research mode. You give it a question, it may ask you one or two things to narrow the scope, then it works for several minutes: searching, reading, searching again as it learns more, and writing a structured report with citations. Use it for questions that deserve a proper brief. For a quick fact, ordinary search is enough.

**A research request that works**

Give it what you would give a human researcher:

```
Research [question].

Context: [why you need it and what decision it feeds].
Focus on: [region, time period, type of organisation].
Prefer: primary sources, official bodies and recent data.
Avoid: vendor marketing and undated blog posts.

For each finding, give the source and the date it was published.
Separate what the sources say from your own interpretation.
Tell me where sources disagree, and what you could not find.
```

The last three lines do the most work. They ask the assistant to show which statements are evidence and which are its own inference. Left alone, it blends the two.

**Checking what comes back**

A citation is not proof. Each one can go wrong in four ways:

1. **The source does not exist.** This is rare when the assistant has really searched, and common when it answers from memory.
2. **The source exists but does not say that.** The assistant misread it, or attached the claim to the wrong link.
3. **The source says it but is weak.** A sales page, an anonymous post, a ten-year-old article.
4. **The source is fine but the claim is stretched.** "One survey found" has become "studies show".

So, for the findings you will actually use:

- **Open the link.** Find the sentence that supports the claim. If you cannot find it, ask: "Quote the exact passage that supports this."
- **Look at who published it and when.**
- **Check the important claims twice.** For a number that will go in front of your boss, find a second independent source.

You do not need to check everything. Check what you will repeat, decide on, or put your name to.

**Useful follow-ups**

- "Which of these findings are you least sure of?"
- "What would someone who disagrees with this conclusion point to?"
- "Is there more recent data than this?"
- "Which of these sources is the most authoritative, and why?"

## Worked example

Mei leads IT at a 300-person professional services firm. Her director has asked whether the firm should move its staff from passwords to passkeys, and wants a recommendation in a week. Mei knows the basics but has not followed the topic closely.

She uses her assistant's research mode:

```
Research whether a 300-person professional services firm should move
staff sign-in from passwords to passkeys in the next 12 months.

Context: I'm the IT lead and need to make a recommendation to our
director. We use Microsoft 365 and about 40 other business apps.
Focus on: organisations of 100 to 1,000 people, guidance from the
last two years.
Prefer: national cyber security agencies, standards bodies, and
documentation from the major platform vendors.
Avoid: marketing from companies that sell sign-in products.

For each finding, give the source and its date. Separate what the
sources say from your own interpretation. Tell me where sources
disagree and what you could not find.
```

The assistant asks one question, about whether staff use company or personal phones, then works for a few minutes. The report has five findings, each with links, a section headed "Where sources differ", and a short list of things it could not establish, including the cost of support during the changeover.

Mei checks the three findings she intends to use.

- **The first** cites a national cyber security agency. She opens it, finds the recommendation in the second section, and notes the date. It holds up.
- **The second** says that most business applications now support passkeys, and cites an industry body's page. She opens it. The page lists which applications support them and gives no overall proportion. The word "most" was the assistant's. She asks: "Quote the passage that supports 'most'." It replies that the page does not give a proportion and corrects the finding. She decides to check her own forty apps against the list instead.
- **The third**, a figure for reduced help-desk calls, comes from a vendor's case study. That is a weak source for a number. She keeps the point as "vendors report fewer password resets" and leaves the figure out.

Her recommendation rests on one strong source, one fact she will verify herself, and one claim downgraded to its true strength. It took her forty minutes. Without the assistant it would have taken most of a day. Without the checking, she would have told her director that "most apps support it" and quoted a sales figure as evidence.

## In your tool

All three assistants search the web and have a deeper research mode. What each is called, where the switch is, and how many research runs your plan includes all change often. Look for a "research" or "deep research" option near the message box, or check the provider's help pages. Free plans usually allow only a few research runs.

## Try it on your own work

1. Choose a real question from your work that you would otherwise spend an hour searching for.
2. Write a research request using the template: question, context, focus, preferred and avoided sources, and the three closing lines.
3. Run it, in a research mode if you have one.
4. Pick the three findings you would actually use. Open each source and find the supporting passage.
5. Note which of the four problems you found, if any.
6. Ask one follow-up from the list above.

## Ignore for now

- Specialist academic search tools. Learn the general method first.
- Building your own collection of sources for the assistant to search. That comes later in the course.
- Trying to verify every sentence. Check what you will rely on.

## In the module session

The instructor runs a research task live from start to finish, checks its citations with the group to find each of the four problems, and explains how research modes work and where they fail.

## Check yourself

1. What is the difference between an answer from memory and an answer from search, and how do you make sure you get the second?
2. Name the four ways a citation can let you down.
3. In the example, what was wrong with "most business applications", and how did Mei find out?
