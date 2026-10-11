# Have the AI interview you first

## Outcome

After this lesson you can turn a task round so that the assistant asks you the questions, draws out what it needs, and only then produces the work.

## Why it matters

Giving good context depends on knowing what context is needed. For a familiar task you do know. For an unfamiliar one, such as a kind of document you have never written or a plan in an area that is new to you, you don't know what you don't know. You leave things out because it never occurred to you that they mattered. The assistant, having seen a great many such tasks, usually does know what matters. So let it ask.

## The idea

**Reverse the direction**

The usual flow is that you explain and the assistant produces. The interview flow adds a step:

1. You state the task and ask to be interviewed.
2. The assistant asks questions. You answer.
3. The assistant produces the work from your answers.

The single instruction that makes this happen is some version of:

> Before you write anything, interview me to get what you need.

**Two additions that make it work properly**

*Ask one question at a time.*
Left alone, an assistant will hand you a list of ten questions at once. Faced with that, most people answer three properly and skim the rest. Asking for one question at a time turns it into a conversation. You give each answer real thought, and the assistant can shape its next question around what you just said, which is what a good interviewer does.

*Say when to stop.*
Give it a limit or a finishing line, otherwise it may keep asking: "Ask up to six questions", or "Stop when you have enough to write a first draft, and tell me what you are still unsure about."

A complete version:

```
I need to [task]. Before you write anything, interview me to get what
you need. Ask one question at a time and wait for my answer. Ask no
more than six questions. Then produce the draft, and list any
assumptions you had to make.
```

**Why it works**

- **It finds the gaps you could not see.** The questions show you what an expert would want to know.
- **It is easier than writing a briefing.** Answering questions takes less effort than composing a complete explanation from nothing. Voice input makes it easier still.
- **The answers are yours.** The result is built from your facts and judgements, so it is specific to you and more accurate.
- **The questions are useful in themselves.** A question you cannot answer has often found the weak point in your plan.

**Point the interview at something**

You can tell the assistant what to dig into:

- "Ask about the audience and what they already believe."
- "Find the weak points in my plan."
- "Establish what I already know, so you don't explain things I've mastered."
- "Work out what I actually want here. I'm not sure myself."

The last of these is more useful than it sounds. When a request is vague because your thinking is vague, an interview is often the fastest way to sharpen it.

**When to use it, and when not**

Use it when the task is new to you, when it is important enough to get right, when you are not sure what you want, or when the result has to be personal to your situation.

Skip it for quick, familiar tasks where you already know exactly what to supply. For those, an interview only adds delay.

**If you can't answer a question**

Say so. "I don't know" and "that hasn't been decided" are useful answers. The assistant can then propose a sensible default and mark it as an assumption, or you can go and find out. Either is better than a guess buried in a finished document.

## Worked example

Kwame is an HR manager at a company of 200. He has been asked to design an onboarding plan for a new group of eight customer support staff starting next month. He has run onboarding before, but never designed a plan from nothing.

He starts with the interview prompt:

```
I need to design a two-week onboarding plan for eight new customer
support staff. Before you write anything, interview me to get what
you need. Ask one question at a time and wait for my answer. Ask no
more than seven questions. Then draft the plan and list any
assumptions you made.
```

The conversation goes like this, in shortened form:

> **Assistant:** What should a new starter be able to do unaided by the end of week two?
>
> **Kwame:** Handle standard email tickets on their own. Not phone calls yet.
>
> **Assistant:** What makes a ticket "standard", and roughly what share of tickets are?
>
> **Kwame:** Billing questions, password resets, delivery status. Maybe 60%.
>
> **Assistant:** Who will be available to train and shadow them, and for how many hours a day?
>
> **Kwame:** Two senior agents. Realistically two hours each per day; they still have their own queues.
>
> **Assistant:** How have previous starters struggled in their first month?
>
> **Kwame:** Too much product training up front. They forget it. And they're nervous about their first real ticket.
>
> **Assistant:** How will you know on day ten whether someone is ready?
>
> **Kwame:** I don't have a clear answer to that.

That fifth question exposes a gap. Kwame had no test of readiness. The assistant goes on to ask about systems access and about the eight starters' previous experience, then drafts a plan.

The plan reflects his answers. It has the starters replying to real standard tickets from day three, with a senior agent reviewing each one before it is sent. Product training is spread across the two weeks, not loaded into the first days. The seniors' time is capped at two hours a day. It also proposes a readiness check: ten tickets handled with no corrections needed. The assistant lists three assumptions, including that system access will be ready on day one.

Kwame checks that assumption with IT and finds that access takes three working days to arrange. He would not have found that out until the first morning. He adjusts the plan and has a finished draft in twenty minutes.

## Try it on your own work

1. Pick a task that is new to you or matters more than usual: a plan, a proposal, a difficult message, a decision.
2. Use the interview prompt above, setting your own limit on the number of questions.
3. Answer one question at a time, honestly. Say "I don't know" where that is true.
4. Note any question you could not answer. That is something to go and find out.
5. Read the list of assumptions in the result and check the one that matters most.

## Ignore for now

- Scripting the questions yourself. The point is that the assistant chooses them.
- Very long interviews. Six to eight questions is enough for most tasks.
- Using this for everything. For routine tasks, give the context directly.

## In the module session

The instructor runs a live interview on a task from the group, shows how to steer an interview that is asking the wrong questions, and demonstrates how to turn a good interview into a reusable prompt for a task you repeat.

## Check yourself

1. Why ask for one question at a time instead of a list?
2. In the example, which question was most valuable, and why?
3. When would you not bother with an interview?
