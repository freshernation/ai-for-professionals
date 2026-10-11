# Why bare requests get generic answers

## Outcome

After this lesson you can explain why a one-line request produces a bland answer, and spot what is missing from a request before you send it.

## Why it matters

The most common complaint about AI is "it gave me something generic". People conclude the tool is mediocre. Usually the request was the problem. A one-line request leaves the assistant to guess nearly everything about your situation, and it guesses the most ordinary version of each thing. Once you see why that happens, you can fix it in under a minute.

## The idea

**The assistant fills every gap with the average.**

An assistant writes the most likely response to what you gave it. Suppose you type "write a LinkedIn post about our new product". It has to settle a great many things you did not mention:

- What is the product?
- Who is it for?
- What is special about it?
- Who is reading the post?
- What should they do afterwards?
- How does your company sound: formal, playful, technical?
- How long should it be?

You gave it none of these, so it supplies the most typical answer to each. The typical product is "innovative", the typical audience is "businesses", and the typical tone is upbeat marketing. Add those together and you get the post you have already seen a thousand times. That post is an accurate reply to the question you asked. It is the average of every post that question could mean.

**A bare request is a request for the average.**

This also explains why the same vague request gives everyone much the same output, and why text produced that way is so easy to recognise.

**The stranger test**

Before you send a request, imagine handing it, on a slip of paper, to a capable stranger who knows nothing about you or your work. Ask yourself: *what would they have to guess?*

Every guess is a place where you will get the average. Write down the answers to the guesses that matter, and the request stops being bare.

You do not need to answer everything. Three or four gaps usually matter far more than the rest:

1. **What is this actually about?** The specific facts.
2. **Who is it for?** The reader or listener.
3. **What is it meant to achieve?** The result you want.
4. **What should it look like?** Length, tone, format.

**Specific in, specific out**

The assistant cannot be more specific than the material it has. If you want a result that sounds as though it was written by someone who knows your product, your customer and your situation, that knowledge has to be in the request. It will not be anywhere else.

It follows that the effort moves. You spend two minutes describing the situation and get back a draft that would have taken thirty. People who say "by the time I've explained it, I could have written it myself" are usually picturing a much longer explanation than is needed.

## Worked example

Nadia runs marketing for a company that makes scheduling software for dental clinics. They are launching a feature that sends patients a text when an earlier appointment opens up.

**The bare request**

```
Write a LinkedIn post about our new product feature.
```

What comes back:

> 🚀 Exciting news! We're thrilled to announce our latest feature, designed to revolutionise the way you work. Our innovative solution streamlines your workflow, boosts productivity and helps your business thrive. Ready to take things to the next level? Get in touch today! #Innovation #Productivity

Every phrase in it could describe any product from any company. Nadia applies the stranger test and lists what a stranger would have had to guess: the product, the feature, the reader, the benefit, the tone, the call to action. That is six guesses, and the assistant gave the average answer to all six.

**The same request with the gaps filled**

```
Write a LinkedIn post announcing a new feature.

What it is: our scheduling software for dental clinics now texts
patients on the waiting list automatically when an earlier appointment
opens up. The first patient to reply gets the slot.

Why it matters: a cancelled appointment usually means an empty chair.
In our pilot with 14 clinics, about 6 in 10 cancelled slots were
refilled the same day.

Reader: practice managers at independent dental clinics. They are busy,
sceptical of software promises, and care about empty chair time.

Goal: get them to book a 15-minute demo.

Tone: plain and practical, like one practice manager talking to
another. No emojis, no hashtags, no words like "revolutionise".
Under 120 words.
```

What comes back:

> A cancellation at 9am used to mean an empty chair at 2pm.
>
> Our scheduling software now handles that for you. When a slot opens, it texts the patients on your waiting list. The first to reply gets the appointment. Your front desk doesn't lift a finger.
>
> We piloted it with 14 clinics. About 6 in 10 cancelled slots were refilled the same day.
>
> If empty chair time is costing you, I'd be glad to show you how it works. It takes 15 minutes.

Nadia changes one sentence and posts it. The second request took her about two minutes to write. She already knew everything in it. She had not thought to say it.

## Try it on your own work

1. Take a request you have recently made to an assistant, or one you are about to make. Write it as you naturally would.
2. Apply the stranger test. List everything a stranger would have to guess. Aim for at least five items.
3. Circle the three guesses that would most change the result.
4. Rewrite the request with those three filled in.
5. Run both versions. Put the results side by side and mark the phrases in the first one that could apply to anyone.

## Ignore for now

- Prompt "frameworks" with acronyms. They are all ways of remembering to fill the gaps. The stranger test does the same job.
- Advice to write very long prompts. Length is not the aim. Filling the gaps that matter is.
- Special phrases that supposedly unlock better answers.

## In the module session

The instructor takes bare requests from the group and rebuilds them live, shows how much of an answer changes with each added piece of context, and explains what the assistant is doing internally when it fills a gap.

## Check yourself

1. Why does a vague request tend to produce text that sounds like everyone else's?
2. What is the stranger test, and what does each "guess" tell you?
3. In the example, where did the information in the second request come from?
