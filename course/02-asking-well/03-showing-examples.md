# Showing examples of what you want

## Outcome

After this lesson you can get an assistant to match a style, format or standard by showing it examples, and you know how to choose examples that teach the right thing.

## Why it matters

Some things are hard to describe and easy to show. Try explaining in words how you write to customers, what a good status update looks like in your team, or how formal is "formal enough" for your industry. You will use words like "professional" and "friendly", which mean something different to everyone. One or two real examples carry more information than a paragraph of adjectives, and the assistant is very good at picking up a pattern from them.

## The idea

**Describing versus showing**

Tell an assistant "write in a warm but professional tone" and it will produce its own idea of warm but professional, which is usually a little too cheerful. Paste in two emails you actually sent and say "write it like these", and it will pick up your sentence length, how you open and close, how direct you are, and the words you tend to use. You could not have listed all of that, and you didn't need to.

**When examples help most**

- **Voice and tone.** Making a draft sound like you, or like your company.
- **Format.** A report layout, a ticket format, how your team writes meeting notes.
- **Standard.** What "good" looks like: a strong answer to a customer, a well-written objective.
- **Classification.** Sorting things into your categories: "these three are urgent, these three are not; now sort the rest."

**How to give examples well**

1. **Use real ones.** Pick things you or your team actually produced and were happy with. Remove anything confidential first.

2. **Give two or three, and make them different.** With a single example, the assistant may copy it too closely, including its topic and particular phrases. With two or three that vary in subject but share the quality you want, it works out what they have in common.

3. **Say what to take from them.** Examples contain many features. Point at the ones you care about: "Match the tone and length of these. Ignore the subject matter."

4. **Mark them clearly.** Separate the examples from your instructions so the assistant does not confuse them. A plain label does the job: "Example 1:", "Example 2:", then "Now write:".

5. **Show a bad one if that is clearer.** "Here is the kind of thing I don't want" with a short sample is sometimes the fastest route. Use it sparingly, and always alongside a good example, so the assistant has something to aim at.

**What can go wrong**

- **Over-copying.** The result reuses a distinctive phrase or the structure of your example too exactly. Fix it with more varied examples, or by saying "don't reuse specific phrases from the examples".
- **Wrong lesson learned.** All your examples happened to be about refunds, so the new draft drifts towards refunds. Vary the examples, or state what to ignore.
- **Bad examples in, bad result out.** The assistant will faithfully reproduce the weaknesses of whatever you show it. Choose examples you would be glad to see copied.

**Examples for format**

For format, you often do not need a real example at all. A skeleton works:

```
Use exactly this layout:

Customer: [name]
Issue in one line: [...]
What we've done: [...]
What happens next: [...]
Owner and date: [...]
```

The assistant fills in the skeleton. This is one of the most reliable ways to get consistent output from one day to the next.

## Worked example

Ingrid is a sales lead at a firm selling industrial cleaning equipment. After every site visit she writes a follow-up email. Her emails are short, specific and a little dry, and customers respond well to them. When she asks an assistant to write one, it comes out gushing: "It was an absolute pleasure to meet you and your wonderful team!"

She tries describing what she wants: "Make it more direct and less enthusiastic." The next draft is curt and still does not sound like her.

So she shows it. She takes two follow-ups she sent last month, replaces the customer names with placeholders, and writes:

```
I write a follow-up email after each customer site visit. Below are
two I've sent. Match their tone, length and structure. Don't reuse
their exact phrases, and ignore the specific products mentioned.

Example 1:
Hi [Name],
Thanks for the walk-round on Tuesday. Three things I took away:
your floor scrubber is fine for the warehouse but too wide for the
packing aisles; the night shift does most of the cleaning; and
downtime matters more to you than purchase price.
On that basis I'd look at the compact model with the service plan.
I'll send figures by Friday. If the night shift supervisor wants to
try one first, I can bring a demo unit the week after.
Ingrid

Example 2:
Hi [Name],
Good to see the site yesterday. My read: the current machines are
doing the job, but you're spending more on repairs than a replacement
would cost over two years. I've attached the comparison.
No rush on a decision. The one date that matters is the end of March,
when the current service contract renews.
Ingrid

Now write a follow-up for this visit:
- Food processing plant, met the hygiene manager
- They need to clean between production runs in under 20 minutes
- Current kit takes about 35
- Interested in the ride-on model but worried about training time
- I promised a training outline and a quote by next Wednesday
```

The draft that comes back opens "Thanks for showing me the plant on Monday", states her read of the problem in two sentences (35 minutes against a 20-minute window), recommends the ride-on model, deals with the training worry, and ends with the Wednesday commitment. It uses her dry tone and her habit of naming one date that matters, without borrowing a phrase from either example.

Ingrid saves the prompt with the two examples in her notes file. From then on, each follow-up takes her three minutes.

## Try it on your own work

1. Choose a kind of thing you write regularly: updates, replies, summaries, notes.
2. Find two or three you were pleased with. Remove names and anything confidential.
3. Write a request that includes them, labelled, with one sentence saying what to match and what to ignore.
4. Ask for a new one on a different subject.
5. Compare the result with what you get from describing the style in words alone.
6. Save the prompt and the examples together for reuse.

## Ignore for now

- The term "few-shot prompting". It is the technical name for what you have just done.
- Building large libraries of examples. Two or three good ones per recurring task is plenty.
- Training or "fine-tuning" a model on your writing. Examples in the request achieve most of the effect with none of the cost.

## In the module session

The instructor shows live how the number and variety of examples change the output, demonstrates capturing a voice from samples and saving it for reuse, and works on format skeletons for the recurring documents the group produces.

## Check yourself

1. Why do two varied examples usually work better than one?
2. Your draft has copied a distinctive phrase from your example. Name two ways to fix it.
3. When is a skeleton better than a real example?
