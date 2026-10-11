# Giving context: goal, audience, constraints

## Outcome

After this lesson you can write a request that tells the assistant what you are trying to achieve, who it is for and what limits apply, in about five lines.

## Why it matters

Knowing that the assistant needs context is one thing. Knowing which context to give, without writing an essay every time, is the skill. Three kinds of context do most of the work: the goal, the audience and the constraints. Get these into a request and the first draft is usually close. Leave one out and you can predict how the result will go wrong.

## The idea

Think of the task as the *what*. The three pieces of context tell the assistant *why*, *for whom* and *within what limits*.

**1. Goal: what are you trying to achieve?**

The task is the thing you want produced: an email, a summary, a plan. The goal is what you want to happen as a result. They are different, and the goal changes the output more than people expect.

- Task: "Write an email declining the supplier's proposal."
- Goal A: "…and I want to keep the door open because we may use them next year."
- Goal B: "…and I want them to stop following up."

Same task, two very different emails. Without the goal, the assistant picks a middle path that serves neither.

A quick way to find your goal: finish the sentence *"This will have worked if…"*.

**2. Audience: who is it for?**

The same content should be written differently for a board member, a new joiner and a customer. Tell the assistant:

- **Who they are.** Role and relationship to you.
- **What they already know.** This sets how much to explain.
- **What they care about.** This sets what to lead with.
- **How they will read it.** A phone between meetings, or a printed pack studied closely.

One sentence is often enough: "The reader is our operations director, who knows the project well, is short of time and mainly cares about the delivery date."

**3. Constraints: what are the limits?**

Constraints stop the assistant doing the reasonable-sounding thing that is wrong for you.

- **Length.** "Under 150 words." "One page."
- **Format.** "A table with three columns." "Plain paragraphs, no bullet points."
- **Tone.** "Direct and warm." "Formal, as for a regulator."
- **Must include.** "Mention the 14 March deadline."
- **Must not include.** "Don't promise a refund." "No jargon." "Don't invent figures; use only the numbers I've given."

The "must not" list is the most neglected and often the most valuable. If you have ever received a draft that offered something you could not give, a missing constraint was the cause.

**Putting it together**

A request with all the parts reads like this:

```
[Task] Write…
[Material] Here is the information: …
[Goal] This will have worked if…
[Audience] The reader is…
[Constraints] Keep it…, don't…
```

You do not need the labels, and the order is not sacred. Write it as you would explain it to a colleague. What matters is that the three pieces are present.

**What goes wrong when one is missing**

| Missing | What you get |
|---|---|
| Goal | Correct but aimless. It covers the topic without doing the job. |
| Audience | Wrong level. It explains what the reader knows, or assumes what they don't. |
| Constraints | Too long, wrong format, or it includes something you can't say. |

When a result disappoints, check it against this table. You can usually name the missing piece in seconds and add it.

## Worked example

Rafael is a finance business partner. The marketing department is 18% over budget for the quarter, and he needs to explain why to its managers before the monthly review.

**First attempt**

```
Explain this budget variance.

Marketing Q3: budget 420,000, actual 495,600.
Events: budget 90,000, actual 151,000 (trade show moved from Q4 to Q3).
Agency fees: budget 120,000, actual 138,000 (rebrand overran by 3 weeks).
Paid media: budget 150,000, actual 147,600.
Other: budget 60,000, actual 59,000.
```

He gets an accurate, formal variance commentary: "Marketing expenditure exceeded budget by 75,600 (18.0%), driven principally by adverse variances in Events and Agency Fees…". It is correct, and it reads as though written for an auditor.

Rafael checks the table. The goal is missing, so the commentary describes the variance without leading anywhere. The audience is missing, so it is pitched at accountants. The constraints are missing, so it is long and full of finance terms.

**Second attempt**

He keeps the figures and adds:

```
Goal: I want the marketing managers to understand that most of the
overspend is timing, not waste, and to agree one action on agency
fees before the monthly review.

Audience: four marketing managers. They are not finance people. They
are a bit defensive about this and expect to be blamed.

Constraints: under 180 words. Plain language: no "adverse variance",
no "phasing". Lead with the overall picture, then the two causes.
Be factual, not accusing. End with one question for them to answer
before the review. Use only the figures I've given.
```

The new version opens: "Marketing spent 75,600 more than planned this quarter. Most of that is timing: the trade show moved forward from Q4, so about 61,000 of spend arrived early and Q4 will be lower by the same amount." It then deals with the 18,000 agency overrun as the one item that is a true overspend, and closes by asking how the team wants to handle agency scope changes in future.

Rafael checks the arithmetic himself (61,000 on events, 18,000 on agency fees, small underspends elsewhere, 75,600 in total) and sends it.

## Try it on your own work

1. Choose something you need to write or prepare this week.
2. Write the task in one line.
3. Add the goal by finishing: "This will have worked if…".
4. Add one sentence on the audience: who, what they know, what they care about.
5. Add at least three constraints, including one "must not".
6. Run it. If the result is off, use the table to name what was missing, add it, and run it again.

## Ignore for now

- Long role-play openings ("You are a world-class expert with 30 years of experience…"). A clear goal and audience do more.
- Formatting your request with special symbols or tags. Plain sentences work.
- Trying to anticipate every possible constraint in advance. Add them when the first draft shows you what you forgot.

## In the module session

The instructor shows what each piece of context changes by adding goal, audience and constraints one at a time to the same task, and demonstrates how to store context you reuse, so that you do not retype it in every chat.

## Check yourself

1. What is the difference between a task and a goal? Give an example from your own work.
2. A draft comes back accurate but pitched at the wrong level. Which piece of context was missing?
3. Why is a "must not include" constraint often the most valuable one?
