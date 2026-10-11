# Asking questions across several files

## Outcome

After this lesson you can give an assistant a set of documents and get reliable answers that draw on all of them: comparisons, contradictions and gaps, each traced to the file it came from.

## Why it matters

Much professional work means holding several documents in your head at once. You compare three supplier proposals against your requirements, check whether a new policy conflicts with two existing ones, or work out what five reports say collectively about one question. It is slow, and people are bad at it, because by the fourth document you have forgotten the detail of the first. An assistant can read all of them together and lay the answers side by side. The risk is that it mixes them up, misses the file where the answer was, or fills a gap in one document with something from another.

## The idea

**Set the files up well**

A little preparation prevents most confusion.

- **Name files clearly.** "Vendor-A-proposal.pdf" is better than "Document (3) final v2.pdf". The assistant uses the names to keep things apart, and so will you when you check.
- **Say what each file is.** One line each: "File 1 is our requirements. Files 2 to 4 are the three proposals."
- **Keep the set small and relevant.** Five documents that matter work better than twenty that might.
- **Use a project or notebook for a set you will return to.** Load the files once and ask as many questions as you need.

**Three kinds of question**

*1. Compare.*
The most common, and the one where a table helps.

```
Compare the three proposals against our requirements document.
Make a table: one row per requirement, one column per vendor.
In each cell, say whether the requirement is met, partly met or not
met, with the page number. If a proposal doesn't mention it, write
"not stated". Don't infer.
```

*2. Find conflicts.*
"Do any of these documents contradict each other? List each contradiction with the file and section on both sides."

*3. Synthesise.*
"What do these five reports collectively say about [question]? Where do they agree, where do they differ, and which report is each point from?"

**The instruction that matters most: "not stated"**

When you ask for a table, the assistant wants to fill every cell. If Vendor C's proposal says nothing about data backup, the assistant may fill the gap with what such products usually do, or with what Vendor B said. Telling it to write "not stated" and not to infer gives it a way to leave a cell empty. A "not stated" cell tells you what to go and ask.

**Always ask which file**

Every answer drawn from several documents should say where each part came from: the file and the page or section. Without that you cannot check it, and you cannot tell a fact in the documents from a blend of them. If the assistant gives an answer without sources, ask: "Which file and page is each of those from?"

**How multi-file answers go wrong**

1. **Cross-contamination.** A detail from one document is attributed to another.
2. **Gap-filling.** A missing answer is supplied from general knowledge or from a different file.
3. **Missed passages.** With many or long files, the tool may search for relevant passages instead of reading everything, and can miss one. The answer is in the file, but the assistant says it is not, or overlooks it.
4. **Unlike compared with unlike.** Prices quoted on different bases, per user against per site or with and without tax, are placed side by side as if they were comparable.
5. **Appendices and small print.** Material at the back of a document is under-read.

**How to check**

- **Check two cells per document.** Go to the page cited. Is it there, and does it say that?
- **Chase the "not stated" cells that matter.** Search the document yourself for the key term. Sometimes it is there under another name.
- **Ask one file at a time for the important points.** "Looking only at Vendor B's proposal, what does it say about pricing? Quote it." A question about one file is more reliable than a question about five. If the two answers differ, trust the single-file one and investigate.
- **Check that the numbers are on the same basis** before you compare them.

**Start with one, then compare**

For anything important, a dependable sequence is this: first ask the same set of questions of each document separately, then ask for the comparison. The separate passes make sure each file was actually read, and the comparison then rests on firmer ground.

## Worked example

Leila is IT lead at an architecture practice of 120 people. The practice is replacing its helpdesk software, and three vendors have submitted proposals of between 22 and 41 pages. She also has her own four-page requirements document. The partners want a recommendation on Friday.

She creates a project in the company's approved assistant, uploads the four files with clear names, and writes:

```
File "Requirements" is what we need. The other three files are vendor
proposals. Compare the proposals against the requirements.

Make a table: one row per requirement, one column per vendor. In each
cell: met, partly met or not met, with a short reason and the page
number. If a proposal doesn't mention something, write "not stated".
Don't infer from what is typical.

Then give a separate table of costs for each vendor: every charge
mentioned anywhere in the proposal, including appendices, with the
page number and the basis (per user, per month, one-off).
```

The requirements table has fourteen rows. Most cells are filled, each with a page number. Three say "not stated": Vendor C on where data is stored, Vendor A on single sign-on, and Vendor B on the notice period for cancelling.

**Checking cells.** She checks two cells per vendor against the cited pages. Five are right. The sixth says Vendor A "meets" the requirement for a mobile app, citing page 12. Page 12 says a mobile app is "on our roadmap for next year". She corrects the cell to "not met" and asks the assistant to re-check every "met" for Vendor A against the exact wording. One more is downgraded to "partly met".

**Chasing "not stated".** She searches Vendor A's proposal for "single sign-on" and finds nothing. She then tries "SSO" and finds it on page 19. The assistant had missed the abbreviation. She tells it, and the cell is updated. The other two gaps really are absent from the proposals, and she emails both vendors.

**Costs.** The cost table shows the monthly price for each vendor. Vendor B looks cheapest. One row, however, was found in an appendix on page 38: a one-off "onboarding and data migration fee" of 9,500, which Vendor B's pricing page does not mention. Vendor A's price turns out to be per technician, and the other two are per employee. With six technicians and 120 employees, these are very different numbers.

She asks for the costs to be put on the same basis:

```
Using only the figures in the cost table, calculate the total cost
over three years for each vendor, for 120 employees and 6 technicians,
including one-off fees. Use your analysis tool and show the working.
```

She checks the arithmetic for one vendor by hand. On a three-year basis Vendor B is no longer the cheapest.

**One file at a time.** Before she writes her recommendation, she asks about her preferred vendor alone: "Looking only at Vendor A's proposal, list anything that limits or qualifies what they are offering. Quote each." This finds a cap on the number of support tickets per month, which she had not seen in the table.

On Friday her recommendation includes a comparison table in which every cell has a page reference, a cost comparison on a common basis, and a list of four questions still outstanding with vendors. One partner asks where the 9,500 came from, and she gives the page number.

## In your tool

- **ChatGPT and Claude:** attach several files to one chat, or load them into a project so that every chat in the project can use them.
- **Gemini:** attach files to a chat, or use NotebookLM, which is designed for questions across a set of sources and links each answer to the passage.

Limits on the number and size of files vary by tool and plan. If the set is large, the tool may search the files instead of reading every page, which is one reason to check the cells that matter.

## Try it on your own work

1. Choose two to five related documents you need to compare or reconcile. Check that they may go into your tool.
2. Rename them clearly. Tell the assistant what each one is.
3. Ask a comparison question as a table, with page numbers and "not stated" for gaps.
4. Check two cells per document against the source.
5. For one "not stated" that matters, search the document yourself under different terms.
6. Ask one important question of a single file on its own, and compare the answer with the table.

## Ignore for now

- Loading every document you own into one place. Small, purposeful sets work better.
- Building a searchable archive for your whole team. That is a project for IT.
- Comparing documents you have not at least skimmed. You need enough familiarity to notice a strange answer.

## In the module session

The instructor compares a set of documents live with a planted trap in an appendix, shows how the same question does when asked across five files and of one, and explains how these tools decide which passages to read.

## Check yourself

1. Why tell the assistant to write "not stated" and not to infer?
2. Name three ways an answer drawn from several files can go wrong.
3. Why is a question about one file more reliable than a question about five?
