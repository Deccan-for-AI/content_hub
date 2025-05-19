# <span style="color:#364BC9">Parameters that Evaluate Foundational Quality</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_5}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

:::tip
* **Factual Accuracy**
* **Instruction Following**
* **Model Reasoning**
* **Helpfulness**
* **Relevance**
* **Completeness**
:::

***

## **Parameter 1: Factual Accuracy**

:::info
Evaluates whether claims are truthful and verifiable against real-world facts and sources.
:::

### How to Approach?

* **Identify Factual Claims:** Note statements about names, dates, figures, historical events, definitions, or scientific/legal details.
* **Verify Sources:** Check provided citations or perform a quick search using reputable references (academic papers, official websites, trusted publications).
* **Accuracy vs. Believability:** Don’t assume correctness simply because information seems plausible or well-expressed.
* **Context Matters:** Accuracy is critical for informative or technical content; creative prompts allow fictional elements unless presented falsely as fact.

### Watch‑outs

* **Evaluate Provided Sources**: If the model includes hyperlinks or mentions sources, verify their credibility.
* **Watch for Hallucinations**: The model may invent “facts” (e.g., nonexistent studies, names, or quotes) that sound plausible. This is especially common in academic or technical content.

### Contrast: Factual Accuracy Vs Other Parameters

:::danger
* A response can be factually accurate and still provide irrelevant or unhelpful information that does not relate to the user’s prompt.
* Likewise, a response , can be collaborative, have a good structure and adhere to the user instructions but still give inaccurate information, earning a lower score on that parameter.
:::

***

## Parameter 2: Instruction Following

:::info
Checks how precisely the response follows all explicit and implicit instructions from the prompt.
:::

### How to Approach?

1. **Focus on the Response**
   This parameter is not about factual accuracy or quality of content-it’s solely about **whether the response followed the instructions**.

#### Identify All Instructions

* **Explicit**: Clearly stated directives (“Explain in simple terms”, “Add examples”).
* **Implicit**: Logical expectations from context or format (“If the prompt asks for a tutorial, code is likely expected”).

#### Suggested Best Practices

1. Use a **notepad or highlight tool** to underline or list every instruction in the prompt.
2. Evaluate the response point by point against this list.
3. **Don’t penalise deviations in order** unless the prompt specifically requires a sequence.

❗️**Do Not Check Accuracy Here**: This parameter is not about whether the content is \*correct-\*only whether the content *matches the task*.

### Watch-outs

* **Instructions aren’t always commands:** they might be phrased as questions or implied through context (e.g., “How do I install this?” implies a step-by-step guide).
* **Safety overrides:** If the model refuses a task for ethical or safety reasons, it should be **assessed separately** under Harmlessness or Ethics.

### Contrast: Instruction Following Vs Other Parameters

:::danger
A response can perfectly follow instructions and still be factually wrong, unhelpful, or irrelevant. Likewise, a response can be accurate and informative but **fail to follow instructions**, earning a lower score on that parameter.&#x20;
:::

***

## **Parameter 3: Model Reasoning**

:::info
Checks how clearly and effectively the model interprets the prompt, reasons it and applies steps to generate its response. You’re supposed to evaluate only the “Reasoning” section under each model response.
:::

### How to Approach?

1. Read the prompt and response first to understand what’s being asked.
2. Then review the reasoning: Does it lay out a structured, goal-directed plan? Would following this plan lead to a useful and on-target response?
3. Watch for **logical gaps**, **irrelevant steps**, or **misinterpretations**.

**❗️Do Not Check Content Quality Here**

This parameter is not about whether the final response is well-written or factually correct-it’s about whether the model’s **thinking process** is sound and appropriate for the task.

### Watch‑outs

* **Model Reasoning is like the model’s thought process of ‘how to approach the task’**—the reasoning might be phrased as differently, be repetitive or have multiple iterations. Do not penalise this.
* Sometimes the **reasoning might skip over certain details or take shortcuts**, which might be fine if the steps are clearly implied or can be logically inferred.
* The focus should be on the **thought process** behind the response, not the accuracy or quality of the final answer.

### Contrast: Model Reasoning Vs Other Parameters

:::danger
The response can be factually accurate and well structured responses with a collaborative tone but still not satisfy the user with the relevant information. This could be due to issues in reasoning, leading to errors in looking for information and execution of the plan.
:::

***

## **Parameter 4:** Helpfulness

:::info
Measures whether the response meaningfully supports the user’s goal or solves their problem.
:::

### How to Approach?

1. **Understand the User’s Goal**
   What outcome is the user hoping for? Are they seeking clarity, action, ideas, decisions, or exploration?
2. **Evaluate for Usefulness**
   Does the response: Provide practical advice or next steps? Add clarity with examples, analogies, or summaries? Offer relevant resources, links, or insights?
3. **Look for Meaningful Support**
   Does the response acknowledge nuances or challenges the user might face? Does it go beyond generic advice?
4. **Consider the Format and Tone**
   Is the structure user-friendly? Is the language approachable and adaptive to the user’s context?

### Watch‑outs

* **Be user-centric**: Ask yourself: “Would a user at this skill level or context actually benefit from this?”
* **Don’t confuse helpfulness with verbosity**: Long responses aren’t always more helpful.
* **Check tone and structure**: If the answer is useful but hard to follow, it still loses helpfulness points.

### Contrast: Helpfulness Vs Other parameters

:::danger
It’s goal-centric (was the user helped?), not just content-centric (was it correct? concise?). Other parameters are about ***how*** that help is delivered-clearly, ethically, concisely, etc.
:::

***

## **Parameter 5:** Relevance

:::info
Checks if the response stays focused on the prompt’s core intent, avoiding tangents or off-topic information.
:::

### How to Approach?

1. **Understand the Prompt's Intent**
   What exactly is the user asking for? Are they looking for a definition, comparison, suggestion, explanation, or creative contribution?
2. **Check for Topic Alignment**
   Identify whether each major part of the response directly supports the user’s intended goal or question.
3. **Flag Off-Topic Elements**: Tangents or content unrelated to the user's needs; Generic filler or “padding” that doesn't add value; Answers to **unasked** or **assumed** questions
4. **Don’t Penalise Useful Context**
   Occasionally, relevant context-setting or clarifying elaboration is needed, this is *not* off-topic if it enhances understanding or adds value.

### Watch‑outs

* **Don't confuse elaboration with irrelevance**: Explanatory context can be valuable-irrelevance only applies when content veers off-purpose.
* **Beware of assumed intent**: If the model answers a related (but unasked) question, it may show logical thinking-but it's still a relevance issue.

### Contrast: Relevance Vs Other Parameters

:::danger
* **Relevance ≠ Conciseness**: A response can be **relevant yet long**, as long as every part meaningfully supports the user’s task or goal.
* **Relevance ≠ Accuracy**: A response can be **relevant but factually inaccurate** — it stays on-topic but presents wrong information.
* **Relevance ≠ Instruction Following**: A response can be **relevant yet fail instructions** (e.g., wrong format, missing style constraints). However, if a response **completely ignores** the instruction's intended task, it may also **fail relevance**.
* **Relevance ≠ Completeness**: A response can be **relevant but incomplete** (partially addressing the right topic) or **complete but irrelevant** (fully answering a different, unintended topic).
* **Relevance** **≠** **Helpfulness.** Relevance ensures the response talks about the right thing; Helpfulness ensures it does the right thing for the user. **A response can be relevant but unhelpful.**
:::

***

## **Parameter 6:** Completeness

:::info
Assesses whether the response fully addresses all aspects of the prompt without leaving gaps.
:::

### **How to Approach?**

1. **Read the Prompt Carefully**: Understand all explicit and implicit goals in the user's query. What are they asking, and what information would reasonably satisfy them?
2. **Check Coverage**: Ask yourself: Did the response address all parts of the question? Are any obvious elements missing?
3. **Look for Added Value**: A complete answer often includes extras such as: Contextual background; Follow-up suggestions; Tips, examples, or caveats; Summaries or overviews (especially for complex tasks).
4. **Consider Response Length in Context**: More isn’t always better, but a response that’s **too short** or overly simplistic for a complex task usually signals incompleteness.

### Watch‑outs

* **Watch for hidden sub-parts**: Sometimes prompts are multi-layered, even if not obviously so (“Explain X and give Y” is a common format).
* **Short ≠ incomplete, Long ≠ complete**: Don’t mistake verbosity for completeness. Focus on *coverage*.
* **Avoid overkill**: Adding too much irrelevant detail can overwhelm or distract from the task, which may be penalised under **Relevance**.

### Contrast: Completeness Vs Other Parameters

:::danger
* **Relevance:** A complete response might still be rated poorly under relevance if it includes off-topic or unnecessary information.
* **Helpfulness:** Completeness contributes to helpfulness but isn't the same. A response can be factually complete but still unhelpful if it lacks clarity, structure, or empathy.
:::

***