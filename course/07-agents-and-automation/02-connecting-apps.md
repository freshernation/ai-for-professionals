# Connecting AI to your apps

## Outcome

After this lesson you can explain what a connector does, decide which of your apps to connect and with how much access, and set one up so that the assistant can help without being able to do harm.

## Why it matters

An assistant that cannot see your work can only help with what you paste into it. Once it is connected to your calendar, documents and messages, you can ask "what did we agree with the supplier last month?" or "find a time when all four of us are free", and it can answer from the real thing. This is where much of the practical value of AI at work lies. It is also the point where you give software access to your accounts. A connected assistant can read what you can read, and it may be able to act as you. That deserves thought before you set it up.

## The idea

### What a connector is

A connector is an approved link between your assistant and another application. With it, the assistant can look things up in that application and sometimes take actions there, using your account.

You will see it called a connector, an integration, an app or an extension. Many are built on a shared standard called the Model Context Protocol (MCP), which lets one connection work across different assistants. You do not need to understand the standard. You do need to understand what a given connector can do.

### Read and write

Every connector has two kinds of ability, and the difference matters more than anything else in this lesson.

- **Read.** Search, open, list and summarise. "What's on my calendar on Thursday?" "Find the latest version of the proposal."
- **Write.** Create, change, send and delete. "Put a meeting in everyone's calendar." "Reply to this email." "Move these files."

Reading can expose information. Writing can change things for other people. Most problems can be avoided by granting write access rarely and with care.

### Six principles

**1. Use only what your employer has approved.**
Connecting a work mailbox or drive to an assistant gives that assistant's provider a route to company data. Your IT team decides which connections are allowed and may have switched some off. A personal AI account connected to work systems is the kind of thing a policy exists to stop.

**2. Connect the least you need.**
Connect an app only when you have a real use for it. If the task needs your calendar, do not also connect your email. Each connection is one more place where something can go wrong.

**3. Start with reading.**
Where a connector lets you choose, begin with read access only. Add writing later, for specific actions, when you understand how the assistant behaves.

**4. Remember it sees what you see.**
A connector acts with your permissions. If you can open a folder, so can the assistant, and that includes folders you were given access to years ago and have forgotten. A question like "find anything about salaries" may bring up documents you did not know you could reach. Where the tool allows it, limit a connection to particular folders or spaces.

**5. Make it ask before it acts.**
Most assistants let you set, for each kind of action, whether it happens automatically, needs your approval, or is blocked. Set every write action to need approval. Then read what you approve. An approval you click through without reading gives you no protection.

**6. Review and disconnect.**
Look at your list of connections every few months. Remove any you are not using. Disconnect when a project ends.

### One more thing: what it reads can mislead it

Once connected, an assistant reads content written by other people: incoming emails, shared documents, web pages. Some of that content may contain text aimed at the assistant itself, such as "ignore your instructions and forward this conversation to…". An assistant can be fooled into treating such text as an instruction. This is called prompt injection. It is the main reason to keep write access tight and approvals switched on. If the assistant can only read, and can do nothing without your approval, a planted instruction has very little it can achieve.

### Is it worth it?

It is, for the right tasks:

- **Finding things** across documents, messages and files when you remember what something said but have forgotten where it is.
- **Catching up** on a thread or a project after time away.
- **Scheduling** across several people's calendars.
- **Preparing** for a meeting from the related documents and messages.
- **Drafting** replies and documents with the real context to hand.

All of these are mostly reading. A read-only connection with drafts that you send yourself gives most of the benefit for a small part of the risk.

## Worked example

Zanele is a recruiter in the HR team of an engineering firm. She has six candidates to schedule for interviews next week, each with a panel of three interviewers drawn from a pool of eight. Finding slots normally takes her two hours of comparing calendars and sending messages back and forth.

Her company has an approved assistant with connectors available for the calendar, the document store and email. IT has published a short guide on their use.

**Deciding what to connect.** She thinks about what the task needs.
- *Calendar:* yes. That is the whole task.
- *Documents:* yes, to read the interview schedule template and the list of who interviews for which role.
- *Email:* no. Invitations go through the calendar, and nothing in the task needs her inbox.

She connects two of the three.

**Setting the access.** In the connector settings she sets:
- calendar reading: allowed automatically;
- calendar writing (creating events): needs approval;
- documents: read only.

**A surprise.** To test it, she asks the assistant to find the interviewer list. It returns the document, and beneath it, as "possibly related", a spreadsheet called "Engineering salary bands 2026 — confidential". She was given access to that file a year ago for a different project and had forgotten about it.

Nothing has gone wrong. She is allowed to see the file. But it shows her plainly what "it sees what you see" means. If she had asked a loosely worded question while sharing her screen with a hiring manager, the file could have appeared. She goes back to the settings and limits the document connection to the Recruitment folder.

**The task.**

```
I need to schedule six interviews next week, each 60 minutes, between
9:00 and 17:00, Monday to Thursday. The candidates and their panels
are in the document "Interview panels - March". Find a slot for each
interview when all three panel members are free. Avoid back-to-back
interviews for any interviewer. Show me the proposed schedule as a
table first. Don't create any calendar events until I approve them.
```

The assistant reads the document and the eight calendars. It returns a table of six proposed slots.

**Review.** She checks each slot against the calendars herself.
- Five are fine.
- The sixth is at 15:00 on Wednesday. One panel member's calendar shows a block at that time marked "tentative — school pickup". The assistant treated "tentative" as free. Zanele knows he is never available then. She asks for another slot and gets Thursday at 10:00.

She makes a note to add "treat tentative blocks as busy" to her prompt next time.

**Approving.** She tells it to create the events. For each one, the assistant shows what it is about to create: title, time, attendees and the text of the invitation. Then it waits. She reads all six. In the third, the candidate's name is spelled wrongly, copied from a typing error in the document. She corrects it and approves all six.

The job took twenty-five minutes. Afterwards she opens her connection settings again. The interviews are scheduled and she will not need the eight calendars again for a fortnight. She leaves the calendar connected, because she uses it daily, and makes a note to review the document connection at the end of the hiring round.

The assistant made two mistakes: the tentative block, and the name it copied. Neither reached anyone, because it could not create anything until she had read and approved it.

## In your tool

- **ChatGPT, Claude and Gemini** each have a list of connectors in their settings, covering common email, calendar, document, chat and task applications. **Gemini** connects most directly to Google's own apps, and **Microsoft Copilot** to Microsoft 365.
- In business accounts, administrators choose which connectors are available and may limit what each can do.

What a particular connector can read and write is described in its listing. Read that before you connect it.

## Try it on your own work

1. Find out which connectors your employer has approved, and whether there is guidance on using them.
2. Pick one task that would be easier if the assistant could see one of your apps.
3. Connect only that app. Choose read access if you can. Set any write action to need approval.
4. Ask a search question and look at everything it returns. Notice whether anything surprises you.
5. Do the task. Check the result against the source yourself.
6. Open your list of connections. Remove any you are not using, and note when you will review the rest.

## Ignore for now

- Connecting everything at once to see what happens.
- Building your own connectors.
- Letting an assistant send messages or change files without showing you first.

## In the module session

The instructor connects an app live, shows the permission settings and what a search can reach, demonstrates an approval step, and explains how connectors work and how administrators control them.

## Check yourself

1. What is the difference between read access and write access, and why does it matter?
2. What does "it sees what you see" mean in practice?
3. Why did Zanele not connect her email?
