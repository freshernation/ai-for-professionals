# From chat to agent: what changes

## Outcome

After this lesson you can explain what makes an AI agent different from a chat assistant, recognise the kinds available, and choose a safe first task to hand to one.

## Why it matters

In a chat you ask and it answers, and you carry out the steps in between. An agent is given a goal and works towards it itself. It searches, opens files, clicks through websites, checks what it found and decides what to do next. It may work for many minutes before it comes back with a result. This is a real change in what you can delegate. It also changes your position. You are now supervising work you did not watch being done, by something that can take actions.

## The idea

### What an agent is

An agent has three parts:

1. **A goal.** You give it an outcome to reach, where a chat would be given one question.
2. **Tools.** These are the things it can do beyond writing text. It might search the web, read and create files, run calculations, operate a web browser, or use your email and calendar.
3. **A loop.** It plans a step, takes it, looks at the result, and decides on the next step. It repeats this until it judges the goal met, gets stuck, or is stopped.

In chat, you supply the loop. You read each answer and decide what to ask next. An agent runs that cycle itself.

### The kinds you will meet

- **Research agents.** They search and read many sources over several minutes and write a report with citations. They only read.
- **Workspace agents.** They work with files in a folder or on your computer. They read documents, build spreadsheets and produce finished files.
- **Browser agents.** They operate a web browser as you would, clicking, typing and filling in forms. They can use websites that have no other way in.
- **Connected agents.** They act inside your work apps through connections you approve, such as email, calendar, documents and task tools.

Many products combine several of these. The names and packaging change often. The three parts stay the same.

### What changes for you

**You delegate outcomes.** In a chat you might ask five questions in turn. To an agent you say what you want at the end and what the limits are. The quality of that brief matters more than any single prompt did.

**Small errors add up.** In a chat, you catch a mistake before the next step. An agent that misreads something in step two builds steps three to twenty on top of it. A long task that is right at each step nineteen times in twenty can still end in the wrong place.

**It can take actions.** A wrong answer in chat is a wrong paragraph, and you can ignore it. A wrong action may be a sent email, a changed file or a submitted form, and some of these cannot be undone.

**You see less.** Twenty steps happen while you do something else. You get a result and a summary. The summary is the agent's own account of what it did, and it can be incomplete or wrong.

**It reads things you have not read.** An agent browsing the web or reading your inbox takes in whatever is there. That can include text written to mislead it.

### What agents are good and bad at

They are good at:

- gathering and organising information from many places;
- repetitive multi-step work where each step is simple;
- first passes that you will review, such as a table of prospects or a sorted folder;
- tasks where you can check the result more easily than you could produce it.

They are poor at:

- anything that needs judgement about people or about your organisation's unwritten rules;
- long tasks with no checkpoints, where an early error ruins everything after it;
- tasks whose result you cannot check;
- websites and systems designed to keep automated visitors out.

### Choosing a first task

Start where a mistake costs nothing. A good first task has three properties:

- **Read-only.** The agent gathers and organises. It does not send, change or buy anything.
- **Checkable.** You can verify a sample of the result in a few minutes.
- **Real.** It is something you would otherwise have done by hand.

Watch it work the first time. Most agents show their steps as they go, and all of them can be stopped. If one heads in the wrong direction, stop it and correct the brief. Do not wait to see how it turns out.

## Worked example

Kai leads a small sales development team at a company that sells maintenance software to hotels. Each month he is given a list of about fifteen hotel groups to approach. For each one he needs the basics: where it is based, roughly how many hotels it runs, any recent news that affects buying, and which role is most likely to own maintenance. Doing it by hand takes most of a day.

**In chat.** He has used his assistant for this before, one company at a time. He asks, reads, copies the answer into a spreadsheet, and moves on to the next. It is faster than doing it unaided, but he is still the one running the loop fifteen times.

**With an agent.** He gives the whole job to his assistant's agent mode:

```
I have a list of 15 hotel groups (below). For each one, find:
- head office city and country;
- approximate number of hotels they operate;
- one piece of news from the last 12 months relevant to someone
  selling them maintenance software (expansion, renovation,
  acquisition, new leadership);
- the job title most likely to be responsible for property maintenance.

Use each company's own website and reputable news sources. Give me a
table with one row per company and a source link for every fact, with
the date of any news item. If you can't find something, write
"not found". Don't guess. Don't contact anyone or fill in any forms.

[list]
```

The task is read-only, he can check it, and he really needs it.

He watches the first few minutes. The agent lists its plan, then begins to search, opening each company's website and then news pages. It is doing what he asked, so he leaves it. Twelve minutes later he has a table of fifteen rows with links.

**Review.** He does not take the table on trust. He checks five rows in full and skims the rest.

- Four of the five are right, and every link supports its fact.
- In the fifth, the head office and hotel count belong to a different company with a very similar name, in another country. Because the agent mixed them up at the first step, everything in that row came from the wrong company. He would have written to a contact about hotels they do not own.
- Skimming the rest, he notices a news item dated three years ago offered as recent. The date column shows it straight away, which is why he asked for dates.
- Two cells say "not found". He would sooner have that than an invention.

He asks the agent to redo the row with the mixed-up name, giving the company's website address so it cannot go wrong, and to replace the old news item. Three minutes later the table is fixed.

The work took twenty-five minutes of his attention in place of a day. The research was no cleverer than before. What changed is that the agent ran fifteen cycles while he did other work. The risk changed with it. In chat, the mix-up would have caught his eye as soon as he read that answer. Here it sat in row nine of a table that looked finished, and he found it only because he checked.

Next month he will put each company's website in the list from the start.

## In your tool

- **ChatGPT, Claude and Gemini** each offer research modes and agent features that carry out multi-step tasks, and each offers some way of operating a browser or working with your files.
- The names, and the plans that include them, change often. Agent features are mostly on paid plans, and organisations frequently switch them off until they have been reviewed.

Check what your employer has approved before you use an agent on work material.

## Try it on your own work

1. Think of a task you do by repeating the same steps many times: looking things up, collecting details, filling in a table.
2. Check it against the three properties: read-only, checkable and real.
3. Write a brief that states the outcome, the sources to use, the format, what to do when something cannot be found, and what the agent must not do.
4. Run it. Watch the first few minutes.
5. Check a sample of the result in full. Note any error that carried through several steps.
6. Write down what you would add to the brief next time.

## Ignore for now

- Agents that act in your accounts. Start with tasks that only read.
- Building your own agents or chains of agents.
- Claims that agents can run a business unattended.

## In the module session

The instructor runs an agent live on a research task, with the group watching its steps and auditing its output, and explains what happens inside the loop and why errors compound.

## Check yourself

1. What are the three parts of an agent?
2. Why can a small error early in an agent's task matter more than the same error in a chat?
3. What three properties make a good first task for an agent?
