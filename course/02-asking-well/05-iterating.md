# Iterating: improving an answer and improving your prompt

## Outcome

After this lesson you can turn a mediocre first answer into a good one in a few targeted steps, and turn a prompt that worked into one you can reuse.

## Why it matters

A first answer is seldom the best the assistant can do. It is only the best it could do with what you said. People who get strong results are not writing perfect prompts. They read the first answer critically, say exactly what is wrong, and repeat. Then, for a task they will do again, they take what they learned and fold it back into the prompt, so that next time the first answer is already good. There are two loops here, improving the answer and improving the prompt, and each needs slightly different moves.

## The idea

### Loop 1: improving the answer

**Diagnose before you respond.** Read the draft and name the problem. Most problems are one of five kinds, and each has a direct fix.

| Problem | What to say |
|---|---|
| Wrong content: it missed the point or included the wrong things | "The main point should be X. Remove the section on Y." |
| Wrong level: too basic or too advanced | "The reader already knows A and B. Don't explain them." |
| Wrong shape: too long, wrong format | "Cut to 100 words. Three short paragraphs, no list." |
| Wrong voice: too stiff, too gushing | "More direct. Remove the adjectives. Write it as I'd say it aloud." |
| Vague: general where you need specific | "Replace the general claims with the actual figures I gave." |

**Be specific in feedback.** "Make it better" gives the assistant nothing to work with, so it changes things at random. "The second paragraph buries the deadline; move it to the first line" gets exactly that.

**Change one or two things at a time.** If you ask for six changes at once, some will be missed or will pull against each other. Two rounds of clear changes beat one tangled round.

**Ask for options.** When you cannot say what you want, ask to see choices: "Give me three versions of the opening line, each with a different angle." It is easier to recognise the right one than to describe it.

**Ask it to criticise its own draft.** "What are the three weakest points of this draft? Then fix them." This often surfaces problems you sensed but could not name.

**Know when to start again.** If the conversation has gone down a wrong path, or you have corrected the same thing twice and it keeps coming back, more feedback will not help. Open a new chat and write a better opening request, using what you now know. You can also go back and edit your original message, which most assistants allow, and try again from that point.

**Know when to stop.** When each round is only swapping one acceptable phrase for another, you are finished. Take the draft and do the last edits by hand.

### Loop 2: improving the prompt

For a one-off task, the answer is all you need. For a task you will repeat, such as a weekly report, a kind of customer reply or a standard analysis, the valuable thing is a prompt that gets it right first time.

**Fold your corrections back in.** Look at the feedback you gave during the conversation. Each correction is something the original prompt failed to say. If you had to say "shorter" and "don't mention pricing", then the improved prompt includes "under 120 words" and "don't mention pricing".

**Have the assistant write the improved prompt.** At the end of a conversation that went well, ask:

```
Based on this whole conversation, write the prompt I should have given
you at the start to get this final result first time. Make it reusable:
put [square brackets] where the details will change each time.
```

The result is a template built from your own corrections.

**Test it.** Open a new chat, paste the improved prompt with fresh details, and see whether the first answer is good. If it is not, note what you had to correct and add that too. After two or three uses, a prompt usually settles.

**Keep a small library.** Save prompts that work in a notes file, with a line on what each is for. Five to ten well-tested prompts for your recurring tasks will save you more time than any other habit in this course.

**The wording is not sacred.** Expect to adjust a saved prompt as your needs and the tools change. What lasts is your understanding of what the task requires.

## Worked example

Farah is an operations manager at a food distribution company. Every Friday she writes an update for the leadership team from her notes, and it takes her forty minutes. She decides to build a prompt for it.

**First request**

```
Turn these notes into a weekly operations update for the leadership
team. [notes pasted]
```

The draft is 450 words, opens with "This week saw a number of developments across operations", and lists everything in the order she happened to note it.

**Loop 1.** She diagnoses the draft: wrong shape, because it is too long, and wrong content, because the one serious issue (a refrigeration failure at the northern depot) sits in the fourth paragraph.

```
Two changes. Lead with the refrigeration failure: what happened, cost,
and what we've done. Then cut the whole thing to under 200 words.
```

That is better. Next round:

```
Good. Now group the rest under three headings: On track, Needs
attention, Decisions needed from you. Drop anything that needs no
action and has no risk.
```

Now it is the update she would have written. One more round: "Remove the opening sentence; start with the first heading." She is done after three rounds and five minutes.

**Loop 2.** She asks:

```
Based on this whole conversation, write the prompt I should have given
you at the start to get this final result first time. Make it reusable
with [square brackets] for what changes each week.
```

She gets back:

```
Turn the notes below into a weekly operations update for the
leadership team.

- Start with the single most serious issue of the week: what happened,
  the cost or impact, and what has been done.
- Then use three headings: On track, Needs attention, Decisions
  needed from you.
- Leave out anything that needs no action and carries no risk.
- Under 200 words. No introductory sentence. Plain, direct language.
- Use only facts from the notes. If something is unclear, list it at
  the end as a question for me instead of guessing.

Notes: [paste this week's notes]
```

The last instruction was the assistant's own addition, and she keeps it. The following Friday she pastes the template and her notes into a new chat. The first draft needs one small edit. The update now takes her eight minutes.

## Try it on your own work

1. Choose a task you do regularly.
2. Make a simple first request and read the result critically.
3. Diagnose it using the five problem types. Give specific feedback, one or two changes per round, until you are satisfied.
4. Ask the assistant to write the prompt that would have produced that result first time, with brackets for the changing parts.
5. Test that prompt in a new chat with different details.
6. Save it in your notes file with a one-line description.

## Ignore for now

- Prompt marketplaces and collections of "best prompts". A prompt built from your own corrections fits your work better.
- Automated prompt-optimisation tools.
- Chasing perfection. A prompt that gets you 90% of the way on the first try is finished.

## In the module session

The instructor iterates on a poor draft live, shows the same task handled by correcting within the chat and by restarting with a better prompt, and reviews the reusable prompts you built for your milestone.

## Check yourself

1. Name the five kinds of problem a first draft can have.
2. Why is "make it better" poor feedback?
3. What is the difference between improving an answer and improving a prompt, and when is the second worth doing?
