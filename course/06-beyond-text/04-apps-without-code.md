# Small apps and tools without code

## Outcome

After this lesson you can describe a small working tool, such as a calculator, a checklist or a tracker, have an assistant build it, test it properly, and judge when it is safe to share.

## Why it matters

Every workplace runs on small tools that nobody ever built: a calculation someone does on paper, a checklist kept in someone's head. A proper tool was never worth a developer's time. Now you can describe what you want in plain language and have a working, clickable tool in a few minutes, without writing code. A tool that looks finished can still be wrong, though. The skill is in the describing, the testing and the judging.

## The idea

### What you can build

- **Calculators:** a quote, a commission, a discount, a loading plan, a break-even point.
- **Checklists and guided steps:** an opening routine, a handover, an inspection.
- **Converters:** units, time zones, text into a standard format.
- **Simple trackers and forms.**

### How it works

You describe the tool to your assistant. It writes the code and shows you the working tool in a panel beside the chat. You can use it at once, and you ask for changes in plain language.

### Describing a tool

Cover five things:

1. **Who uses it, and when.** "A shift supervisor at a loading dock, on a tablet, wearing gloves."
2. **What goes in.** Each input, with its unit and sensible limits.
3. **What comes out.** The result, and how it should be shown.
4. **The rules.** Exactly how the result is worked out. This is the part that matters most and the part most often left vague.
5. **How it should look and behave.** Large buttons, a clear result, what happens when the input is invalid.

Give the rules as you would explain them to a new colleague, and include one example with the answer worked out.

### Build in small steps

Ask for the simplest version first, try it, then add one thing at a time. If you ask for everything at once, you cannot tell which part is wrong.

### Test it properly

A tool that runs can still be wrong. The assistant may have interpreted a rule differently from you, and the result will still look confident on screen.

- **Test with cases where you already know the answer.** Work out three or four by hand first.
- **Test the awkward cases.** Zero, a very large number, a blank box, a decimal, a value exactly on a limit.
- **Test the unusual but real cases.** The heavy item, the part-time employee, the order that crosses midnight. These are where a rule that sounded complete turns out to have gaps.
- **Try to break it.** Type letters where numbers belong. Does it fail clearly, or does it show a wrong answer?
- **Have someone else use it** without your explanation. Watch where they hesitate.

When a test fails, tell the assistant exactly what you entered, what you got and what you expected. Then run every test again, because a fix can break something that was working.

### Know its limits before you share it

Four questions decide whether a tool is safe to use beyond your own desk.

**1. Where does the data go?**
Many tools built this way keep nothing, and the entries are gone when you close the page. Others save data in your browser or with the provider. Ask the assistant where the data is stored and who can see it.

**2. Who can open it?**
A shared tool often lives at a public web address, and anyone with the link can open it.

**3. What data will people type into it?**
If the answer includes personal details, customer information, health data, pay or anything confidential, do not share a tool you built this way without your IT or security team. Researchers have repeatedly found quickly built AI apps on the public internet exposing their users' data, usually because nobody had set up proper sign-in or access rules.

**4. What happens if it is wrong, or disappears?**
If a wrong result could cause harm or cost money, the tool needs a proper review and someone to keep it working.

**A simple rule**

- **For you alone, with nothing confidential in it:** build and use freely.
- **For your team, with no personal or confidential data, low stakes:** share it, tell people it is a home-made tool, and say how to check its answers. If a wrong answer could affect safety, have a responsible person approve your tests first.
- **Anything that stores other people's data, handles money, or that many people will depend on:** treat what you built as a prototype. Take it to IT.

## Worked example

Hamza is a shift supervisor at a warehouse that ships catering supplies. Several times a day, someone has to work out how many pallets an order needs. The rule is that a pallet holds at most 48 boxes and at most 800 kg. People work it out on paper and sometimes get it wrong, which means a second lorry trip. He decides to build a calculator.

**The description.**

```
Build a simple pallet calculator for warehouse staff to use on a
tablet with gloves on.

Inputs: number of boxes (whole number, 1 to 2,000) and weight of one
box in kg (0.5 to 800).
Output: the number of pallets needed, shown very large, with a line
underneath explaining which limit decided it.

Rules: a pallet holds at most 48 boxes and at most 800 kg. Boxes
cannot be split between pallets. All boxes in an order are the same.
Example: 130 boxes of 18 kg each needs 3 pallets.

Large buttons and text. If an input is missing or out of range, show
a clear message instead of a result.
```

A working calculator appears. He types in 130 and 18, and it shows **3 pallets**. It looks finished.

**Testing.** Before building, Hamza had worked four cases out by hand.

| Boxes | Weight each | His answer | Why |
|---|---|---|---|
| 130 | 18 kg | 3 | 44 boxes fit by weight (792 kg); 130 ÷ 44 rounds up to 3 |
| 48 | 10 kg | 1 | exactly at the box limit |
| 49 | 10 kg | 2 | one over the box limit |
| 10 | 450 kg | 10 | only one drum fits per pallet |

The first three pass. For the fourth, the tool says **6 pallets**.

Hamza can see what happened. The tool divided the total weight, 4,500 kg, by 800 and rounded up. But a 450 kg drum cannot be split, and two would weigh 900 kg, so each pallet takes one. Six pallets would be overloaded, which is a safety problem.

He tells the assistant exactly what he found:

```
With 10 boxes of 450 kg, you show 6 pallets. The right answer is 10.
You are dividing total weight by 800, but boxes can't be split. Work
out how many whole boxes fit on one pallet by weight (800 ÷ box
weight, rounded down), take the smaller of that and 48, then divide
the number of boxes by that and round up.
```

The assistant corrects it. Hamza runs all four tests again, and all pass.

His description had said "boxes cannot be split". The first version ignored that and still gave the right answer for his example. Only the unusual case showed the fault.

**Trying to break it.** He asks a colleague to use it without any explanation. She asks whether the weight is per box or for the whole order. He has the label changed to "Weight of ONE box (kg)".

**The four questions.**
- *Where does the data go?* He asks. Nothing is stored.
- *Who can open it?* Anyone with the link. It contains only arithmetic.
- *What will people type in?* Box counts and weights.
- *What if it is wrong?* Overloading a pallet is a safety matter. So he has the operations manager check and approve his test cases before he shares it, and writes a line on the tool itself: "Home-made tool. If the answer looks wrong, check by hand and tell Hamza."

He shares the link with the four supervisors. When one asks for mixed box sizes, a harder problem, he takes the working calculator to IT as an example of what they need.

## In your tool

- **Claude** builds working tools in a side panel and lets you share them by a link.
- **ChatGPT and Gemini** can each build and run small tools in their canvas view.
- **Dedicated app-building tools** go further, with data storage and sign-in. With those, the four questions matter even more.

## Try it on your own work

1. Think of a calculation, checklist or conversion that you or your team do by hand again and again.
2. Work out four test cases by hand, including one unusual case.
3. Describe the tool: who uses it, inputs, output, rules, and one worked example.
4. Build the simplest version. Run your tests. Report any failure precisely and re-run all of them after the fix.
5. Try to break it, and have someone else use it.
6. Answer the four questions. Decide whether it is for you alone, for your team, or for IT.

## Ignore for now

- Tools that need user accounts, payments or a database.
- Building anything that handles personal or confidential data.

## In the module session

The instructor builds a tool live from a learner's rules, has the group write the test cases that expose its flaw, and looks at where a shared tool's data really goes and who can reach it.

## Check yourself

1. Which of the five parts of a tool's description matters most, and what helps to make it unambiguous?
2. Why is one passing example not enough to trust a tool?
3. What are the four questions to answer before sharing a tool?
