# Scheduled and recurring work

## Outcome

After this lesson you can set up a task that an assistant runs for you on a schedule, design it so that it stays useful, and notice when it has quietly stopped working.

## Why it matters

Some work arrives on a timetable: the Monday summary, the daily check of a few sources, the monthly reminder to chase something. People do it reliably for a while and then stop. An assistant can do it every time without being asked. A scheduled task is a different kind of thing from a chat, though. It runs when you are not there, on a brief you wrote weeks ago, and nobody watches it. A good one saves you time for months. A bad one fills your inbox with noise until you ignore it. A broken one can go unnoticed, and you carry on trusting a report that stopped being true.

## The idea

### What you can schedule

- **Briefings.** "Every weekday at 8:00, summarise what is on my calendar and what I need to prepare."
- **Digests.** "Every Monday, give me the five most relevant developments in [topic] from the past week."
- **Monitoring.** "Check these pages daily. Tell me only if something changes."
- **Recurring preparation.** "On the 25th of each month, draft the status report from the project tracker."

All of these gather something and deliver it to you. That is where scheduling works best.

### Designing a scheduled task

A scheduled task runs with nobody to clarify it. The brief has to be complete without you. Cover six things.

**1. When.** The time and frequency. Choose the least frequent schedule that still does the job.

**2. What, exactly.** A full brief: sources, criteria and limits. Anything you would have explained in a follow-up message has to be in it from the start.

**3. From where.** Name the sources: specific sites, a particular folder, a tracker. "Search the web for news" produces different and worse results each week.

**4. In what form.** A short, fixed format. Set a maximum length. Ask for links, and for the date of every item.

**5. When there is nothing to say.** State this explicitly: "If nothing meets the criteria, say 'Nothing significant this week' and stop." Without that instruction, the assistant will fill the space with something minor. A digest that always contains five items teaches you to ignore it.

**6. Proof that it ran properly.** Ask for a line at the end that shows what was actually checked: "Sources checked: 5 of 5. Period covered: 4 to 10 March." This is how you notice when something has broken.

### How scheduled tasks fail

**Silently.** A connection expires, a website changes, or a limit is reached. The task then runs with part of its input, or does not run at all. Often you are told nothing. The danger is that you go on assuming it works.

**By drifting.** The task still runs, but it no longer fits what you need. The project ended, the competitor was acquired, or the format no longer suits you.

**By becoming noise.** It produces too much, too often, with too little that matters, and you stop reading it. A task you do not read is worth nothing. It can also hide the one week when it has something important.

**By staleness.** It reports old items as new, or repeats last week's.

**By being wrong, unnoticed.** Nobody is reviewing each run. A recurring error becomes something you believe.

### Keeping them healthy

- **Check the first three runs closely.** Treat them as a pilot. Expect to change the brief after each.
- **Keep scheduled tasks to reading and drafting.** A task that runs unattended should not send, pay, delete or publish. If it prepares something that will be sent, it should stop at a draft for you.
- **Give each one a review date.** Ask every month or two whether you still read it, whether it is still right, and whether it is still needed.
- **Keep a list.** Know what you have running. Automations you have forgotten about still run, still read your data and still use up your allowance.
- **Glance at the proof line** every time. If it says "3 of 5", something needs attention.
- **Switch off what you no longer use.**

### When to use something else

If a task needs to run for a whole team, or the business depends on it, it belongs in a tool your IT team manages, with an owner and monitoring. A scheduled task in your personal assistant is a personal aid.

## Worked example

Mariam is a marketing manager at a company that makes project management software for architects. She likes to know what her three main competitors are doing and what the two leading trade publications are saying. She used to check on Monday mornings, when she remembered. She sets up a scheduled task.

**The brief.**

```
Every Monday at 7:30, prepare a competitor and industry brief.

Sources (use only these): the news or blog pages of [Competitor A],
[Competitor B] and [Competitor C], with their web addresses; and the
news sections of [Publication 1] and [Publication 2].

Include only items published in the last 7 days that involve: a
product launch or major feature, a pricing change, a senior hire or
departure, an acquisition or funding, or a significant customer win.

Format: at most 5 items, most important first. For each: one sentence
on what happened, one on why it matters to us, the link, and the
publication date.

If nothing meets the criteria, write "Nothing significant this week."

End with: "Sources checked: X of 5. Period covered: [dates]."
Do not contact anyone or sign up for anything.
```

**Run 1.** The brief arrives with five items. She checks each link.
- Three are real and recent.
- One is a feature announcement from Competitor B dated fourteen months ago. It sits high up on their blog page because the page shows "popular posts".
- One is a general opinion piece from a publication, about remote working. It meets none of her criteria. It looks as though the assistant wanted to reach five.

She amends the brief: "Check the publication date on the article itself. Leave out anything older than 7 days, even if it appears prominently. Do not include general opinion pieces. Fewer than 5 items is fine."

**Run 2.** Three items. Two are right. The third reports a "senior hire at Competitor C", but the article is about a different company with a similar name in another industry. She adds each company's exact name, its web address, and "architecture and construction software" as a description.

**Run 3.** Two items, both correct, and the line "Sources checked: 5 of 5. Period covered: 17 to 23 March." This is the brief she wanted. She puts a note in her calendar to review the task in two months.

**Week 8.** The brief contains one item, from a trade publication. The last line reads: "Sources checked: 2 of 5. Period covered: 21 to 27 April."

It says two of five. She looks into it. The three competitor sites have started showing a pop-up that the assistant cannot get past, so it has been reading only the two publications. That same week, Competitor A announced a price cut of twenty per cent. She heard about it from a sales colleague on Tuesday.

Without the proof line, she would have received a tidy brief with one item and assumed that her competitors had had a quiet week. The task had not crashed. It had gone on producing output that looked plausible while seeing less than half of what it was meant to see.

She changes the sources to each competitor's news feed, which the assistant can read. She adds a rule: "If you cannot read a source, say so at the top of the brief." She runs the task by hand to confirm that it now reads five of five.

**Month 3 review.** She still reads it every Monday. She also finds a second scheduled task, set up for a campaign that ended in January and still running every day, and deletes it.

## In your tool

- **ChatGPT, Claude and Gemini** each let you schedule tasks to run at set times and deliver the result as a notification or a message. Each has a page listing your scheduled tasks, where you can pause, edit or delete them.
- Limits on how many you can have and how often they run depend on your plan. Scheduled runs may start a little after the time you set.

A scheduled task can usually use web search. Whether it can use your connected apps and files varies. Check before you rely on it.

## Try it on your own work

1. Think of something you check or prepare on a regular timetable, or mean to.
2. Write the brief with all six parts, including the rule for "nothing to report" and the proof line.
3. Limit it to reading and drafting.
4. Run it once by hand and check every item.
5. Schedule it. Check the first three runs closely, and amend the brief after each.
6. Put a review date in your calendar. List everything you have running, and switch off anything you no longer read.

## Ignore for now

- Chains in which one automation triggers another.
- Scheduled tasks that send messages to other people.
- Scheduling things in order to look productive. Schedule only what you would otherwise have to do by hand.

## In the module session

The instructor designs a scheduled task live, shows a run that has failed without saying so and asks the group to spot it, and shows three weeks of real runs and what changed after each.

## Check yourself

1. Why must a scheduled task's brief say what to do when there is nothing to report?
2. What is the proof line for, and what did it reveal in the example?
3. Name four ways in which a scheduled task can fail.
