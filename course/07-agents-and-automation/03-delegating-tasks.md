# Delegating a multi-step task

## Outcome

After this lesson you can hand an agent a task of many steps with a brief that sets its limits, test it on a small sample, supervise the full run, and review the result properly.

## Why it matters

Giving an agent a long task is closer to delegating to a person than to asking a question. The brief was vague, so you got something other than what you wanted. You did not say where the limits were, so the person went past them. You did not check until the end, and by then it was too late. Agents fail in the same ways. They are faster, though, and they do not stop to ask when something seems odd. The skill in this lesson is delegation: a clear brief, a small trial, and a real review.

## The idea

### The delegation brief

A brief for a multi-step task has seven parts.

1. **Goal.** State the outcome and what it is for.
2. **What done looks like.** How will both of you know it is finished and correct?
3. **Inputs.** Say where the material is, and which sources to use and which to leave alone.
4. **Method, where it matters.** Include any rule that must be followed. Leave the rest to the agent.
5. **Limits.** State what it must not do, and be explicit: "Do not send anything. Do not delete or move files. Do not change the original spreadsheet."
6. **Checkpoints.** Say where it must stop and ask you: "Show me the plan before you start. Stop and ask if you find more than ten discrepancies."
7. **The report.** Tell it what to say at the end: what it did, what it could not do, what it assumed, and what you should check.

Parts 5, 6 and 7 are the ones people leave out, and the ones that matter most with an agent. An agent that has been told only the goal will find some way to reach it.

### Ask for the plan first

Before any long task, have the agent set out how it intends to go about it: "Give me your plan as numbered steps before you do anything. Wait for my approval."

Reading the plan takes a minute, and it shows up misunderstandings that would otherwise appear only in the output. If the plan is wrong, correct the brief. If it is right, approve it.

### Test small

Never run a new task on everything first. Run it on a small sample, three items out of three hundred, and review that sample closely. You will nearly always find something to change: a case the brief did not cover, a rule the agent read differently, an output that is not what you pictured.

A pilot costs minutes. A full run with a flaw in it costs the whole run, plus the time it takes you to discover the flaw.

### Supervise the run

- **Watch the start.** The first few minutes show whether the agent is on the right track.
- **Know how to stop it.** Find the stop button before you need it.
- **Check in on long runs.** If a task takes half an hour, look at it after ten minutes.
- **Stop when it goes wrong.** An agent that has gone off course seldom finds its own way back.

### Review the result

An agent's report is its own account of its work. It is a place to start your review. It does not replace one.

1. **Read the report.** In particular, read what it could not do and what it assumed.
2. **Reconcile the counts.** If there were forty items, does the result account for all forty?
3. **Check every exception.** Anything the agent flagged as a problem needs your judgement.
4. **Spot-check the unremarkable.** Choose a few items it reported as fine and verify them yourself. If one is wrong, check more.
5. **Check nothing else changed.** Are the original files untouched? Was anything created, moved or sent that you did not ask for?

### Then make it repeatable

When a task has run well, save the brief with what you learned folded in. Next time you start with a brief you have already tested.

### What to keep for yourself

Delegate the gathering, the matching, the sorting and the drafting. Keep the judgement: what a discrepancy means, what to say to a supplier, and anything that commits you or your organisation.

## Worked example

Ibrahim is an accounts payable accountant at a building supplies distributor. At each month-end he reconciles supplier statements against the company's ledger. There are forty suppliers, and each sends a statement as a PDF. For each one he compares the invoices listed with what the ledger shows, notes the differences, and emails the supplier about anything unexplained. It takes two days.

His company has approved an assistant with an agent mode that can work on files in a folder. The statements and a ledger export are not customer data, and company policy allows them in the tool.

**The brief.**

```
Goal: reconcile this month's supplier statements against our ledger,
so I can query suppliers about real discrepancies.

Inputs: 40 supplier statements (PDFs) in the folder "Statements-Sept".
The ledger export is "AP-ledger-Sept.xlsx". Use only these.

Method: for each supplier, match each invoice on the statement to the
ledger by invoice number and amount. An item is a discrepancy if it is
on the statement and not in the ledger, in the ledger and not on the
statement, or the amounts differ.

Done: a spreadsheet with one row per supplier (matched / discrepancies /
could not process) and a second sheet listing every discrepancy with
supplier, invoice number, both amounts and the page of the statement.

Limits: do not change or move any file in the folder. Do not send
anything to anyone. Save your output as a new file.

Checkpoints: show me your plan first. Then do only the first three
suppliers and stop.

Report: what you did, what you could not process and why, anything
you assumed.
```

**The plan.** The agent lists six steps. Step 3 says "extract invoice lines from each statement". Ibrahim asks, "How will you treat credit notes?" The agent replies that it will treat every line as an invoice. That is wrong. A credit note reduces what is owed. He adds a rule: "Lines marked as credit notes or with negative amounts are credits. Match them to credit entries in the ledger."

Without it, every supplier with a credit note would have shown a false discrepancy.

**The pilot.** The agent processes three suppliers and stops. Ibrahim checks all three by hand.
- Two are right.
- In the third, the agent reports a discrepancy for invoice "INV-00482", which the ledger holds as "482". They are the same invoice in two formats. He adds: "Ignore prefixes and leading zeros when matching invoice numbers."

He runs the three again. All three are now correct.

**The full run.** He starts it and watches the first few minutes. It finishes in twenty-five.

**The review.**

*The report* says: 34 suppliers fully matched, 5 with discrepancies, 1 could not be processed, because the statement is a poor scan with unreadable amounts. One assumption is listed: where a statement showed a payment the ledger did not yet show, it was treated as a timing difference and noted, not flagged.

*Counts:* 34 + 5 + 1 = 40. Every supplier is accounted for.

*Exceptions:* he examines all five.
- Three are real: invoices on the statement that the company never received.
- One is a supplier that has invoiced twice for the same delivery.
- One is no discrepancy at all. The ledger shows a payment made on the 29th that the supplier's statement, dated the 28th, could not include. The agent's timing rule covered payments missing from the ledger and did not cover this reverse case. Ibrahim takes it off the list.

*Spot-check:* he picks four of the 34 "matched" suppliers and checks them fully. All four are right.

*The unprocessed one:* he reconciles that supplier by hand.

*Nothing else changed:* the folder still contains forty PDFs and the ledger with their original dates, plus one new output file.

**The judgement.** He asks the agent to draft a query email for each of the four real discrepancies and to save them as drafts without sending them. He reads each one, softens the wording to the supplier who double-invoiced, since it is a long-standing relationship and probably an honest mistake, and sends all four himself.

The reconciliation took three hours in place of two days. He saves the brief, now including the rules on credit notes, invoice number formats and timing in both directions, as "Month-end supplier reconciliation". Each of those three rules came from something the plan, the pilot or the review showed him. None of them was in his first draft.

## Try it on your own work

1. Choose a repetitive task of many steps that you are allowed to run through your tool.
2. Write a brief with all seven parts. Take most care over the limits, the checkpoints and the report.
3. Ask for the plan. Ask one question about how it will treat an awkward case.
4. Run a pilot on three items. Check all three by hand, and amend the brief.
5. Run the full task. Watch the start.
6. Review it: the report, the counts, every exception, a spot-check of the unremarkable, and whether anything else changed.
7. Save the improved brief.

## Ignore for now

- Tasks in which the agent sends, pays, deletes or publishes.
- Long unattended runs with no checkpoint.

## In the module session

The instructor delegates a multi-step task live from brief to review, with the group questioning the plan, auditing the pilot and reconciling the final counts.

## Check yourself

1. Which three parts of the brief are most often left out, and why do they matter with an agent?
2. What does a pilot on three items protect you from?
3. What are the five steps of reviewing an agent's result?
