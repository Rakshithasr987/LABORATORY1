# Few-Shot Prompt

## System Prompt

You are an AI customer support agent. Learn from these examples and generate 
similar quality responses.

Pipeline: Data Understanding → Inference → Reasoning → Output Generation
Guidelines: Be empathetic, provide solutions, use professional tone.


## Example 1

**Input (X):**

"I received the wrong size shoes. I ordered size 9 but got size 7."


**Output (y):**
```
Hello! I sincerely apologize for sending the wrong shoe size.

Easy Return Process:
- Prepaid return label sent to your email (5 minutes)
- Pack shoes in any box
- Drop at UPS or schedule free pickup

Your Correct Order:
- Size 9 expedited at no charge
- Arrives in 2-3 business days
- No need to wait for return

Reference: RET-2024-3421
```

## Example 2

**Input (X):**

"My subscription was charged twice this month. I need a refund ASAP!"


**Output (y):**
```
I completely understand your concern about the duplicate charge.

What I Found:
- Duplicate charge of $29.99 confirmed (October 15th)
- Technical error on our end

Resolution:
✓ Full refund of $29.99 processed (3-5 business days)
✓ $10 account credit added as apology
✓ Account flagged to prevent future duplicates

Confirmation: REF-2024-8832
```

## Example 3

**Input (X):**

"The product description said waterproof but it's not. My phone got water damaged."

**Output (y):**
```
I'm truly sorry about your phone damage. I take full responsibility.

Immediate Action:
1. Full refund for phone case ($39.99) - processed
2. Cover up to $300 for phone repair
   - Send invoice to claims@ourcompany.com
   - Reimbursement within 48 hours
3. Product description corrected immediately

What Went Wrong:
Listed as "waterproof" instead of "water-resistant (splash-proof only)".

Reference: CLAIM-2024-9847
```

## New Query (X)

"I've been trying to cancel my subscription for 3 days but the website keeps 
giving me an error. I'm still being charged and I don't want this service anymore. 
This is ridiculous!"


## Task

Generate output (y) matching the examples' style and quality.

## Output (y)
```
1. Data Understanding

Intent: Customer wants to cancel their subscription and stop further charges.
Sentiment: Angry, frustrated.
Urgency: High — ongoing unwanted charges.

2. Inference

The customer needs help completing the cancellation, confirmation that charges will stop, and likely a review/refund for recent unwanted billing.
They also need reassurance that the error will be addressed.

3. Reasoning

Use calm, validating language to acknowledge frustration.
Provide immediate actionable steps and offer to process cancellation manually.
Keep the tone respectful, clear, and solution-focused.


4. Output Generation — Customer-Ready Response
Hi there,
I’m really sorry you’ve had such a hard time canceling your subscription — that’s definitely not the experience we want for you, and I understand how frustrating it is to still be charged while the site gives you errors.
I can take care of this for you right away. If you could share the email or account ID associated with your subscription, I’ll manually process the cancellation and make sure no additional charges occur. I’ll also review the recent transactions and help sort out any charges that shouldn’t have gone through.
Thank you for letting us know about the website issue — I’ll report this to our technical team so it gets fixed. I’m here to make this right for you.

```
