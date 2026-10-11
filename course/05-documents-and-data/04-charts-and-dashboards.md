# Charts and simple dashboards

## Outcome

After this lesson you can turn data into a chart that makes one point clearly, build a simple dashboard for a question you are asked repeatedly, and check that what the picture shows is true.

## Why it matters

A good chart does in three seconds what a table takes a minute to do. Most people seldom make charts, because choosing the right kind and getting the software to cooperate is fiddly. Assistants remove nearly all of that. The work that remains is the work that always mattered: deciding what the chart is for, and making sure it does not mislead. A picture persuades more strongly than a table, so a wrong one does more harm.

## The idea

**Start with the point**

A chart should answer one question. Before asking for one, finish this sentence: *"This chart shows that …"*. If you cannot, you are not ready for a chart. Ask the assistant to explore first: "Look at this data and tell me the three most notable things in it." Then choose what is worth showing.

**Ask for the chart by its purpose**

```
Using the attached data, make a chart that shows [the point].
The audience is [who]. Suggest the best type of chart and tell me why.
Give it a title that states the finding. Label the values directly.
Use one colour, with a second only to highlight [the thing that
matters].
```

The usual matches are these:

| You want to show | Use |
|---|---|
| A comparison between categories | Bars |
| A change over time | A line |
| Parts of a whole (few parts) | Stacked bar, or a simple table |
| A relationship between two measures | A scatter plot |
| A single important figure | The number, large, with a comparison |

**What makes a chart clear**

- **The title states the finding.** "Sales team turnover is 40%, far above every other department" is a title. "Turnover by department" is only a label.
- **One point per chart.** If you have two points, make two charts.
- **Direct labels** on bars or lines, so that the reader does not have to look back and forth to a legend.
- **Colour with a purpose.** Grey for context, one colour for what matters.

**How charts mislead**

These errors appear in AI-made charts just as they do in human ones. Often nobody intended them.

1. **Counts where rates are needed.** A department with 120 people will have more leavers than one with 40. The count shows which is bigger. The rate shows which has the problem.
2. **A cut-off axis.** A bar chart whose axis starts at 90 instead of zero makes a small difference look huge.
3. **Uneven time periods.** A part-year compared with full years.
4. **Averages that hide the spread.** An average satisfaction score of 7 could mean that everyone gave 7, or that half gave 10 and half gave 4.
5. **Too little data.** A dramatic percentage change based on five cases.
6. **Wrong values.** The chart simply does not match the data, because the wrong column was used or rows were dropped.
7. **Suggested causes.** Two lines that rise together invite the conclusion that one causes the other.

**Checking a chart**

- **Read two values off the chart and find them in your data.** Do they match?
- **Check the axis.** Does it start at zero for bars? Are the units right?
- **Ask what is behind each figure.** "How many records is each bar based on?"
- **Ask the assistant to criticise it.** "How could this chart mislead someone? What would a sceptic say?"
- **Ask whether it should be a rate.** "Should this be shown as a percentage of the total and not as a count?"

**From chart to dashboard**

A dashboard is a small set of charts that answer the questions you are asked repeatedly, kept in one place. For a simple one:

1. **List the questions it must answer.** Three to five. Limit it to what someone looks at monthly and acts on.
2. **Choose one chart or number for each question.**
3. **Put the most important at the top left.**
4. **Decide how it will be refreshed.**

You can build one in three ways:

- **In your spreadsheet.** Ask the assistant for step-by-step instructions to create the charts on a summary sheet. This is the simplest to maintain, because the charts update when the data does.
- **As an interactive page.** Assistants can build a small web page with charts from your file, with filters you can click. The page is a snapshot of the data you gave it.
- **In your organisation's reporting tool,** if it has one.

Apply the same checks to every chart on it, and write down the definitions: what counts as a "leaver" or a "late delivery". Most arguments about dashboards are really arguments about definitions.

## Worked example

Yuki is an HR analyst at a software company of 360 people. The leadership team has asked whether there is a turnover problem. She has a spreadsheet of everyone who left in the last twelve months, with department and leaving date, and a headcount table by department. The file has employee numbers but no names, and may go into the company's approved assistant.

**Explore.** She uploads both sheets and asks for a chart of leavers by department.

The assistant produces a bar chart of the number of leavers: Support 30, Sales 16, Engineering 7, Operations 3. The title reads "Leavers by department, last 12 months". Support's bar is nearly twice the height of any other.

**Check.** Yuki reads two values off the chart and finds them in her data. Support 30 is right. Sales 16 is right. So the chart is accurate. Then she asks:

```
How could this chart mislead someone? Should this be a rate instead
of a count?
```

The assistant replies that the chart shows counts, and that the departments are very different in size. Support has 120 people and Sales has 40. Shown as a share of headcount, the picture changes. It recalculates with the analysis tool:

| Department | Headcount | Leavers | Turnover |
|---|---|---|---|
| Sales | 40 | 16 | 40% |
| Support | 120 | 30 | 25% |
| Engineering | 140 | 7 | 5% |
| Operations | 60 | 3 | 5% |
| **Company** | **360** | **56** | **15.6%** |

She checks the arithmetic for Sales herself: 16 ÷ 40 = 0.40. She also checks that the leavers sum to 56 and the headcount to 360.

The real outlier is Sales, where two in five people left within a year.

**The chart.** She asks:

```
Make a bar chart of turnover rate by department, sorted highest to
lowest. Start the axis at zero. Label each bar with the percentage
and the number of leavers in brackets. Grey bars, with Sales in a
single highlight colour. Add a line for the company average. Title
it with the finding.
```

The chart comes back titled "Sales turnover is 40%, more than twice the company average". Each bar is labelled, for example "40% (16 of 40)". The numbers behind each percentage matter: Operations' 5% rests on three people.

**Asking for criticism again.** The assistant notes that a twelve-month figure hides when people left, and that the rate uses current headcount where it could use the average over the year. Yuki checks the dates. Eleven of the sixteen Sales leavers went in the three months after a change to the commission plan. She adds a second chart, a line of Sales leavers by month, with the commission change marked. She words the title with care: "Most Sales departures followed the commission change in March". The title says they followed it. It does not say the change caused them. She does not have the evidence for cause, and says so in her notes.

**The dashboard.** Leadership will want this every quarter. She lists four questions: overall turnover against last year; turnover by department; leavers by length of service; and time to fill vacancies. She asks the assistant to help her build a summary sheet with four charts driven by formulas, so that it updates when she adds new rows. She writes the definitions at the top: "leaver" means anyone who left in the period, and the rate is leavers divided by current headcount.

She presents two charts. The discussion is about Sales and the commission plan, which is where it needed to be.

## In your tool

- **ChatGPT, Claude and Gemini** can each make charts from an uploaded file, and can build an interactive page with several charts.
- **Copilot in Excel and Gemini in Google Sheets** create charts inside the spreadsheet on eligible plans.

## Try it on your own work

1. Take a set of data you report on. Check that it may go into your tool.
2. Ask the assistant for the three most notable things in it.
3. Choose one. Finish the sentence "This chart shows that…".
4. Ask for the chart by its purpose, with a title that states the finding and direct labels.
5. Check two values against the data. Ask how the chart could mislead, and whether it should be a rate.
6. List three questions you are asked every month. Sketch which chart would answer each.

## Ignore for now

- Advanced chart types. Bars and lines cover most needs.
- Large dashboards with dozens of measures. Nobody reads them.

## In the module session

The instructor builds a chart live from a learner's question, shows the same data telling two different stories as counts and as rates, and shows how a chart can be made to mislead, with the group checking each chart against the data.

## Check yourself

1. What should a chart's title do?
2. Name four ways in which a chart can mislead.
3. In the example, the first chart was accurate. Why was it still the wrong chart?
