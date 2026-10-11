# What is safe to share: privacy basics

## Outcome

After this lesson you can decide in a few seconds whether a piece of information may go into an AI assistant, and you can remove the risky parts when it shouldn't go in as it is.

## Why it matters

The most useful thing you can give an assistant is real material from your work. That material is also where the risk is. People handle this badly in two ways: they paste a customer list into a personal account without thinking, or they are so cautious that they never give the assistant anything real and conclude it is not useful. A simple rule lets you avoid both.

## The idea

**What happens to what you type**

When you send a message, it goes to the provider's servers. Three things can then happen to it, depending on your account type and settings:

- **It is stored**, so that you can see your chat history. Deleting a chat usually removes it from your view at once and from the provider's systems after a period.
- **It may be used to train future models.** On personal accounts, providers may use conversations for this, sometimes by default and sometimes by your choice. There is a setting to control it.
- **It may be read by people**, in limited cases such as safety review or when you send feedback on a reply.

**The biggest difference is the account type**

- **Personal accounts** (free or paid) are covered by consumer terms. Whether your chats are used for training depends on a setting that you should check today.
- **Business accounts** provided by your employer are covered by a contract. The main providers state that they do not use business customers' content to train their models by default, and administrators get controls over retention and access.

So the same sentence can be fine in your company's business account and a policy breach in your personal one.

**The three-tier rule**

Sort anything you are about to paste into one of three tiers.

**Tier 1: Fine to share.** Information that is public or harmless.
- Published material, general knowledge questions.
- Your own draft writing that contains nothing confidential.
- Generic versions of work tasks: "a customer", "a supplier", round numbers.

**Tier 2: Check the policy first.** Internal business information.
- Internal documents, plans, meeting notes.
- Financial figures that are not public.
- Anything about a named customer, supplier or partner.
- Code and technical designs.

For tier 2, use it only in a tool your employer has approved, in the way the policy allows. If there is no policy, ask before you paste.

**Tier 3: Never share**, unless your employer has approved that tool for that data in writing.
- Personal data about identifiable people: names with health, pay, performance or contact details.
- Passwords, access keys, security details.
- Information under a confidentiality agreement or legal privilege.
- Unannounced results, deals or anything that could move a share price.
- Regulated data, such as patient records or payment card details.

**When in doubt, strip it down**

Usually you can get the same help without the sensitive part.

- **Replace names** with roles: "Client A", "the candidate", "a regional manager".
- **Round or scale numbers**: 4.83 million becomes "about 5 million", or multiply everything by a constant.
- **Remove identifiers**: account numbers, email addresses, addresses.
- **Describe instead of pasting**: "a two-page complaint about late delivery and a billing error" often gets you as good a draft reply as the real letter.

Then put the real details back yourself when the draft comes out.

## Worked example

Tomás is an account manager. A client has sent an angry email about a failed software rollout, and he wants help drafting a reply. His company allows AI tools for non-confidential work but has no business account.

The email names the client's company, three of its staff, the contract value, and a security fault. He sorts it:

- Client name and named individuals: tier 2 and tier 3.
- Contract value: tier 2.
- The detail of the security fault: tier 3.
- The shape of the complaint: tier 1.

So he does not paste the email. He writes:

```
Help me draft a reply to an unhappy client.

Situation: we rolled out software to a mid-sized client last month.
The go-live slipped by two weeks, their staff were given training
after launch instead of before, and a technical fault caused half a
day of downtime. Their operations director has written a sharp email
saying confidence in us is damaged and asking what we will do.

What I can offer: a named senior engineer on site for two weeks,
a written incident report by Friday, and a call with our director.
I cannot offer a refund.

Tone: accountable, specific, no excuses, no corporate language.
Under 200 words. Leave placeholders in [brackets] for names and dates.
```

He gets a strong draft with bracketed placeholders, fills in the real names and dates himself, and sends it. The assistant never saw who the client was or what the fault involved.

## In your tool

Each assistant has a setting that controls whether your conversations on a personal account can be used to improve its models. Find it and decide.

- **ChatGPT:** Settings, then Data Controls. The switch is labelled "Improve the model for everyone". There is also a Temporary Chat mode that is not saved to history or used for training.
- **Claude:** Settings, then Privacy. The switch covers whether your chats help improve Claude.
- **Gemini:** the activity setting for Gemini Apps in your Google account. Google states that some chats may still be reviewed by people even when activity saving is off.

Labels move, so if you cannot find the setting, search the provider's help pages for "training" and "data controls".

## Try it on your own work

1. Open the privacy or data settings in your assistant. Find the training setting and choose.
2. Look at the last three things you pasted, or wanted to paste, into an assistant. Put each into tier 1, 2 or 3.
3. Take one tier 2 or tier 3 item and write a stripped-down version, as Tomás did. Use it to get the help you wanted.
4. Find your employer's AI policy. If there is none, send one email asking what is permitted.

## Ignore for now

- The fine print of each provider's retention periods. Know that it exists and where to find it.
- Technical security measures such as encryption standards.
- Privacy law in detail. Your company's policy is the practical version of it for you.

## In the module session

The instructor walks through each provider's current data settings on screen, explains what actually happens to a conversation after you send it, and works through real "can I paste this?" cases from the group.

## Check yourself

1. Why can the same text be acceptable in one account and not in another?
2. Which tier is a spreadsheet of employee salaries, and what would you do if you needed help analysing it?
3. Name three ways to strip down sensitive material before sharing it.
