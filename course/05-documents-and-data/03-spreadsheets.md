# Spreadsheets: formulas, cleanup and analysis

## Outcome

After this lesson you can use an assistant to write and explain formulas, clean up messy data, and analyse a spreadsheet, and you know how to confirm that the numbers are right.

## Why it matters

Almost every job involves a spreadsheet, and most people use a small fraction of what spreadsheets can do. An assistant changes this more than almost anything else in this course. You describe what you want in plain language and it writes the formula, tidies the file or runs the analysis. Spreadsheet work is also where a confident wrong answer is most dangerous, because a number looks like a fact. So this lesson gives as much attention to checking as to doing.

## The idea

There are three levels of help. Each needs a different kind of check.

### Level 1: Formulas

Describe what you want and where your data is.

```
In Google Sheets, column A has order dates, column B has the region,
column C has the order value. Write a formula that totals the order
value for the "North" region in March 2026. Explain how it works.
```

Say which spreadsheet program you use, because the functions differ, and give the column letters.

You can also paste a formula you inherited and ask: "Explain what this does, step by step, and what could make it give a wrong answer."

**Check:** try the formula on three or four rows where you can work out the answer by hand. Include an awkward case, such as a blank cell, a zero, or a date at the edge of the range.

### Level 2: Cleaning

Real data is messy. The same thing is spelled five ways, dates come in mixed formats, there are stray spaces, duplicates and merged cells. Cleaning is tedious, and assistants are good at it.

Upload the file and start by asking the assistant to look:

```
Look at this file before doing anything. Tell me: how many rows and
columns, what each column contains, and any problems you can see:
inconsistent spellings, mixed formats, blanks, duplicates, values
that look wrong.
```

Then ask for specific fixes, and a record of them:

```
Fix these: [list]. Don't delete any rows without telling me. Give me
the cleaned file, and a list of every change you made with the number
of rows affected.
```

**Check:** the row count before and after. Read the list of changes. Open the cleaned file and look at twenty rows.

### Level 3: Analysis

With a file uploaded, you can ask questions in plain language: "What were sales by region by month?", "Which ten customers account for the most revenue?", "Is there a relationship between discount and order size?"

Behind the scenes, a capable assistant writes a small program, runs it on your file and reports the result. This matters. A number that comes from running a calculation is exact. A number the assistant simply "says" without running anything is a guess, and may be wrong.

So look for the sign that it actually computed. Most tools show an "analysing" step, or let you open the code. If you are not sure, ask: "Did you calculate that by running code on the file, or estimate it? Show the calculation."

**Check:** this is the important one.

1. **Confirm it read the whole file.** "How many rows did you analyse?" The number should match yours.
2. **Check one number by hand.** Pick one figure from the result. Filter or sum in the spreadsheet yourself and compare.
3. **Check the totals add up.** If it gives sales by region, do the regions sum to the overall total?
4. **Ask what it assumed.** "What did you do with blank cells, duplicates and anything that didn't fit?" The answer often reveals a decision you would have made differently.
5. **Ask whether it looks plausible.** You know your business. A figure that surprises you is either an insight or an error. Find out which before you repeat it.

**What goes wrong**

- **Part of the file is missed.** A second sheet, rows beyond a limit, or a header row read as data.
- **Silent choices.** It drops rows with blanks, or counts duplicates twice, without saying so.
- **Wrong column.** It uses "order date" when you meant "ship date".
- **Categories not merged.** "Trade show" and "Events" are the same thing to you and two things to the assistant.
- **A stated number that was never calculated.**

**What may go in**

Spreadsheets often hold customer names, salaries and sales figures. Apply your usual rules. If the file cannot go into your tool, you can still get formula help by describing the columns.

## Worked example

Camille is a marketing analyst at a company that sells accounting software to small businesses. She has an export of last quarter's leads from the customer system: 2,400 rows, with the lead's source, the date and the campaign. She also has a separate note of what was spent on each channel. The marketing director wants cost per lead by channel by tomorrow. The file contains no personal data beyond a lead number, and company policy allows it in the approved assistant.

**Look first.** She uploads the file and asks the assistant to describe it before doing anything.

It reports 2,400 rows and five columns. The "Source" column has eleven distinct values where there should be four: "LinkedIn", "linkedin", "Linked In", "LinkedIn " with a trailing space, "Search", "Google search", "Email", "email", "Events", "Event" and "Trade show". Dates are in two formats. There appear to be 88 duplicate lead numbers.

**Clean.** She writes:

```
Fix these: standardise Source to four values (LinkedIn, Search,
Email, Events), where "Google search" is Search and "Event" is Events.
Put all dates in one format. Remove duplicate lead numbers, keeping
the earliest. Don't delete anything else. Give me the cleaned file
and a list of every change with the number of rows affected.
```

The change list says 88 duplicates were removed, leaving 2,312 rows, and gives the number of rows relabelled for each spelling. She checks: 2,400 − 88 = 2,312.

**Analyse.** She gives the spend per channel and asks for leads and cost per lead by channel, calculated with the analysis tool. The result:

| Source | Leads | Spend | Cost per lead |
|---|---|---|---|
| LinkedIn | 480 | 12,000 | 25.00 |
| Search | 750 | 9,000 | 12.00 |
| Email | 782 | 2,000 | 2.56 |
| Events | 288 | 15,000 | 52.08 |
| Trade show | 12 | — | — |

**Check.** She runs through the list.

- *Whole file?* She asks how many rows were analysed. 2,312. Good.
- *Totals?* 480 + 750 + 782 + 288 + 12 = 2,312. Good.
- *Plausible?* There is a fifth row. "Trade show" was in the original list of eleven values, and she had forgotten to include it in her cleaning instruction. The assistant had left it alone, as told. Trade shows are events. She asks for it to be merged: Events becomes 300 leads, and cost per lead becomes 15,000 ÷ 300 = 50.00.
- *One number by hand.* She opens the cleaned file, filters Source to "Search", and counts 750 rows. It matches.
- *Assumptions.* She asks what was done with blanks. The assistant says 14 rows had no date and were kept, since the analysis did not depend on date. That is fine for this question, and it would matter for a monthly breakdown.

**Formula.** The director will want this every quarter. Camille asks:

```
I'm using Excel. The cleaned data is on a sheet called Leads, with
Source in column B. On a second sheet I have the four sources in
A2:A5 and spend in B2:B5. Write formulas for C2 (number of leads)
and D2 (cost per lead) that I can copy down. Explain them.
```

She gets a COUNTIF formula for the count and a division for the cost, with an explanation. She tests them, and the counts match the table.

The whole job took thirty-five minutes. Had she skipped the checks, the director would have received a table with a stray fifth row and an Events figure that was four per cent too high.

## In your tool

- **ChatGPT, Claude and Gemini** all accept spreadsheet files and can run calculations on them. Check that the analysis or code-execution feature is on for your account.
- **Assistants inside the spreadsheet:** Microsoft Copilot in Excel and Gemini in Google Sheets work directly in the file, on eligible plans. ChatGPT and Claude each offer an add-in for Excel.

Very large files may exceed upload limits. If so, analyse a filtered extract.

## Try it on your own work

1. Take a formula you use and do not fully understand. Ask for a step-by-step explanation and what could make it wrong.
2. Describe a calculation you need in plain language, with your column letters and spreadsheet program. Test the formula on four rows, including an awkward one.
3. Take a messy file that may go into your tool. Ask the assistant to describe it before changing anything.
4. Ask for specific fixes with a list of changes. Check the row count.
5. Ask one analysis question. Confirm the rows analysed, check one number by hand, and check the totals.
6. Ask what was assumed about blanks and duplicates.

## Ignore for now

- Macros, scripts and programming. Formulas and uploaded analysis cover most needs.
- Statistical tests and forecasting models. Get counts, totals and averages right first.

## In the module session

The instructor cleans and analyses a messy file live, shows the difference between a calculated number and a stated one, and plants errors in the data for the group to catch with the five checks.

## Check yourself

1. What is the difference between a number the assistant calculated and one it stated, and how can you tell which you have?
2. What are the five checks for an analysis?
3. In the example, how did the fifth row come about, and which check caught it?
