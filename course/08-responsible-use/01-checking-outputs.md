# Checking outputs before you rely on them

## Outcome

After this lesson you can decide how much checking a piece of AI-assisted work needs, carry out that check efficiently, and avoid the habits that let errors through.

## Why it matters

Everything an assistant produces reads well, whether or not it is right. A correct answer and a wrong one arrive in the same assured tone. Whatever you pass on carries your name, and "the AI wrote it" is no defence when a customer, a manager or a regulator finds the mistake. Checking everything exhaustively would cancel the time you saved, so you need a way to match the check to what is at stake.

## The idea

### Two questions set the level

For any output, ask:

1. **What happens if this is wrong?** Think about who is affected, how badly, and whether it can be put right.
2. **Would I notice?** Can you tell at a glance, or does it look right either way?

The answers put the work into one of three levels.

### Three levels of checking

**Level 1: Glance.**
*Use it when* the work is for you or close colleagues, is easy to correct, and you would spot a mistake by reading it. Examples are a reworded internal message, a list of ideas, or a first outline.
*The check:* read it once, properly. Does it say what you mean?

**Level 2: Check.**
*Use it when* someone else will rely on it, or it goes outside your team, but an error would be an embarrassment and not a disaster. Examples are a summary for your manager, a routine reply to a customer, or an analysis used in a meeting.
*The check:*
- trace every fact, figure, name and date to where it came from;
- recompute any number that matters;
- look for what is missing;
- look for promises or commitments you did not intend to make;
- read it once as the recipient.

**Level 3: Verify.**
*Use it when* money, safety, legal position, someone's job or your organisation's reputation depends on it, or when it cannot be undone. Examples are a technical statement to a customer, a contract term, a published claim, or a decision about a person.
*The check* is everything in Level 2, plus:
- confirm each key claim against an independent, authoritative source. Do not accept the assistant's own citation or its own assurance;
- have a second qualified person review it;
- keep a note of what you checked and against what.

Most work is Level 1 or 2. The skill is in recognising Level 3 when it turns up, and it often turns up looking like a routine request.

### What to look for

Errors gather in predictable places:

- **Specifics.** Numbers, dates, names, references, quotations, clause numbers, units.
- **Sources.** A source may not exist, or may exist and not say what is claimed.
- **Conditions.** An "only if" or "unless" may have been dropped.
- **Calculations and conversions.**
- **Things added.** Look for a detail or commitment that you did not supply.
- **Things left out.**

### Useful techniques

- **Trace to source.** For each claim that matters, find the place it came from and read that place.
- **Recompute.** Do the sum yourself, or have the assistant run the calculation and show its working.
- **Ask for the weak points.** "Which statements here are you least certain of? What should I verify first?" The answer directs your attention. It is not a guarantee.
- **Fresh eyes.** Paste the work into a new chat and ask for a critical review. A new chat is not committed to the earlier one's choices.

### Three traps

**Fluency.** Text that reads well feels correct. Polish tells you nothing about accuracy.

**Growing trust.** After twenty correct outputs you stop checking the twenty-first. The risk on each one has not changed, but your attention has dropped. This is how experienced users get caught.

**Asking the assistant whether it is sure.** It will usually say yes. Its confidence is not evidence.

The first two traps act together. In a field experiment with 758 consultants at a large consulting firm, those using AI did markedly better on tasks that suited the technology. On one task chosen because it lay beyond the AI's ability, the consultants using AI were 19 percentage points less likely to reach the correct answer than those working without it. The output had been plausible, and they accepted it.

### When you find an error

Fix it. Then ask what kind of error it was and whether it could be anywhere else in the same piece. One wrong figure in a table is a reason to check the others.

## Worked example

Lena is a quality engineer at a company that makes pressure-relief valves. On one Tuesday she uses her company's approved assistant for three pieces of work.

**9:15. A message to her team.** She has written a blunt note about a change to the inspection rota and asks for a friendlier version.

*What if it is wrong?* Nothing much. *Would she notice?* Yes. **Level 1.** She reads the result once. The assistant has changed "from Monday" to "starting next week", which means the same thing. She sends it. The check took thirty seconds.

**11:00. A summary for her manager.** She uploads a twelve-page supplier audit report and asks for a one-page summary. Her manager will use it in a supplier review that afternoon.

*What if it is wrong?* Her manager would make a point in a meeting that the report does not support, which would be embarrassing and could be corrected. *Would she notice?* Only by checking. **Level 2.**

She traces each fact to the report.
- The summary says "seven non-conformities, two of them major". The report's table lists nine, two of them major. The assistant had counted from a section that covered only one production line.
- The summary says the supplier "has committed to corrective action within 30 days". The report says 30 days for the major items and 90 for the minor ones. A condition has been lost.
- She looks for anything missing. The report notes that one calibration certificate had expired. The summary does not mention it, and it is exactly what her manager would want to know.

She corrects all three. Then, because the count was wrong, she rechecks every other number in the summary. The check took twelve minutes. The summary would have taken her forty.

**14:30. A reply to a customer.** A customer's engineer has asked whether a valve model is suitable for a system running at 16 bar, and which clause of the applicable standard covers the test requirement. Lena asks the assistant to draft a reply from the product data sheet she provides.

*What if it is wrong?* A customer might install a valve on the strength of her statement. This is a safety matter and a liability matter. *Would she notice?* The draft looks authoritative. **Level 3.**

The draft says the valve is rated to 20 bar and is therefore suitable. It gives the set pressure as "16 bar (323 psi)" and cites a specific clause of the standard for the test requirement.

She verifies each claim independently.
- *The rating.* She opens the data sheet herself. The rating is 20 bar, but only for the stainless steel body. The customer's order is for the bronze body, which is rated to 16 bar. That leaves no margin, and a different recommendation is needed. The assistant had used the first figure it found.
- *The conversion.* She does the calculation. 16 bar × 14.5 = 232 psi. The draft has 323, with two digits transposed.
- *The clause.* She opens her own copy of the standard. The clause cited exists and deals with marking, not testing. The test requirement is in a different section.

There are three errors in a four-sentence reply, and each was stated with complete assurance.

She rewrites the reply herself, with the correct rating for the bronze body, a recommendation of the next model up, the correct conversion and the correct clause. She asks a senior colleague to review it, as company procedure requires for technical statements to customers. In the customer file she records that the rating was checked against the data sheet at its current revision and the clause against the standard, with the date.

That took forty minutes, and the assistant saved her very little. For technical statements to customers she will write the substance herself in future.

The same tool saved real time on two tasks and produced a draft that could have caused a failure on the third. She applied one rule each time: decide the level first, then check to that level.

## Try it on your own work

1. Take the last five things you produced with an assistant's help.
2. For each, answer the two questions and assign a level.
3. Did you check each one to its level? Be honest.
4. Take one that was Level 2 or 3 and check it properly now: trace, recompute, look for what is missing and what was added.
5. Find out whether your organisation requires a second reviewer for any kind of work you do.
6. Write your own three-line rule: what you glance at, what you check, and what you verify.

## Ignore for now

- Tools that claim to detect AI errors automatically.
- Checking low-stakes drafts to Level 3. That wastes the time you saved.
- Waiting for models that do not make mistakes.

## In the module session

The instructor gives the group three outputs to check at three levels against the clock, shows how trust built on a run of correct answers lets an error through, and works on each learner's own three-line rule.

## Check yourself

1. What two questions decide how much checking a piece of work needs?
2. What does Level 3 add to Level 2?
3. Why is "it has been right every time so far" a dangerous reason to skip a check?
