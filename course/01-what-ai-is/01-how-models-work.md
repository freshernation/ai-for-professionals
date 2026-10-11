# How these models work, in plain terms

## Outcome

After this lesson you can explain in two minutes what an AI assistant is doing when it answers you, and use that picture to predict when it will be reliable and when it won't.

## Why it matters

Most disappointment with AI comes from the wrong mental picture. People treat an assistant as a search engine, a database or a colleague who knows their company, then feel let down when it behaves like none of them. With the right picture, its odd behaviour stops being surprising, and you can decide what to trust before you have been burned.

## The idea

An assistant such as ChatGPT, Claude or Gemini is built on a **language model**. Four ideas explain almost everything it does.

**1. It predicts what comes next.**
The model was built by showing it an enormous amount of text and having it practise one thing: given some text, predict the next piece. Do that across a large share of what people have written, and to predict well the model has to pick up grammar, facts, styles, reasoning patterns and how a contract differs from a birthday message. When you type a question, it writes the continuation that best fits, one small piece at a time. It is composing, not looking anything up.

**2. What it knows is frozen, and blurry.**
The text it learned from stops at a date, often many months before you are using it. It also does not store that text as documents it can reopen. It keeps something closer to a strong general memory. It usually knows that a famous report exists and roughly what it argued, but it may misremember a figure or a page number, just as you might.

**3. It only sees what is in the conversation.**
Everything the model can work with at a given moment is called its **context**: your messages, its earlier replies, any files you attached, and instructions the tool adds behind the scenes. That is all. It does not know your company, your project or what you meant but didn't say. In most tools, a new chat starts empty. Context is also limited in size, so in a very long conversation the early material can get less attention.

**4. It makes choices with a little randomness.**
At each step there are several plausible next words, and the model does not always take the top one. That is why asking the same question twice gives two differently worded answers. For a draft this is useful. For a fact it is a warning: if two tries give two different numbers, at least one is wrong.

**What follows from this**

- It is fluent by construction. Sounding confident is what it does. Confidence is not evidence of accuracy.
- It is strongest where its training text was plentiful: common business writing, well-known subjects, popular software.
- It is weakest on the specific and the recent: your internal data, last week's news, an exact quotation, a niche regulation.
- The quality of what you put into the context decides the quality of what comes out. Paste the real document and it works from the document. Leave it out and it works from blurry memory.

Modern assistants add tools on top of the model: web search, file reading, running calculations. These tools fill the gaps above. Searching puts fresh pages into the context, for example. The model underneath still works the same way.

## Worked example

Priya manages operations at a logistics firm. A shipment for a key customer will arrive three days late and she needs to tell them.

First she types:

```
Write an email to a customer about a delayed shipment.
```

She gets a polite, generic apology that could have come from any company. It invents a reason for the delay and promises a discount she has no authority to offer. The model had nothing to work from, so it predicted the most typical email of that kind.

Then she runs it a second time and gets a different email with a different invented reason. That is idea 4: the details were never facts, only plausible filler.

Now she puts the facts into the context:

```
Write an email to a customer about a delayed shipment.

Facts:
- Customer: a retail chain, relationship of six years, contact is the
  supply chain lead.
- Order of 40 pallets was due Monday 14th. It will arrive Thursday 17th.
- Cause: a customs inspection at the port. It is cleared now.
- We can send 12 pallets by road to arrive Tuesday if they want.
- I cannot offer a discount.

Tone: direct, takes responsibility, no grovelling. Under 150 words.
```

This time the email is specific, accurate and usable after a light edit. Nothing about the model changed. The context did.

## Try it on your own work

1. Pick a message you need to write this week.
2. Ask your assistant for it in one bare sentence. Save the result.
3. Ask again with the same sentence in a new chat. Note what changed between the two.
4. Now add the real facts, the reader, and the tone you want, as Priya did. Compare.
5. Write down one thing the assistant invented in step 2. That is what "predicting plausible text" looks like in practice.

## Ignore for now

- The mathematics. You do not need neural networks, parameters or training methods to use these tools well.
- Model names and version numbers. They change every few months.
- Arguments about whether the model "really understands". Interesting, but it does not change how you should work with it.

## In the module session

The instructor opens the lid: what a token is, how training differs from answering, why a longer context is not always better, and a live demonstration of the same prompt producing different answers. Bring any behaviour that has puzzled you.

## Check yourself

1. A colleague says, "It told me the figure was 14%, so I put it in the deck." Using the ideas above, what would you ask them?
2. Why does a new chat not remember what you told the assistant yesterday?
3. You ask the same factual question twice and get two different answers. What does that tell you?
