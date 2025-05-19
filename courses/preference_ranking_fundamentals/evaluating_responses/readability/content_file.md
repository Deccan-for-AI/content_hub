# <span style="color:#364BC9">Parameters that Evaluate Readability</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_6}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

:::tip
* Clarity
* Persona Adherence
* Conciseness
* Structure
* Tone
:::

***

## **Parameter 1: Clarity**

:::info
Assesses whether ideas are expressed clearly, directly, and understandably, especially for the intended audience.
:::

### How to Approach?

1. **User Perspective**: Imagine you're the user reading this for the first time—can you easily understand it, or do you need multiple reads?
2. **Match User Expertise**: Adjust clarity based on the user's expertise level—beginners need simple explanations, while experts prefer concise precision.
3. **Logical Flow**: Check if ideas smoothly build upon each other, clearly addressing the user's query from start to finish (e.g., introduction → explanation → conclusion).

**Note**: Do **not** evaluate formatting or structure here; that is handled separately.

### Watch‑outs

* Always evaluate clarity from the user’s viewpoint and stated needs.
* Avoid confusing clarity with formatting or structural issues; focus specifically on how easily ideas and concepts are understood.
* Consider whether minor clarity improvements would notably enhance user comprehension. If yes, lean towards minor issues rather than no issues.

### Contrast: Clarity Vs Other parameters

:::danger
**Clarity** focuses on making the *meaning* easy to understand through precise wording, coherent phrasing, and idea flow, avoiding unnecessary technical language (e.g., “The function evolves over an infinite-parameteral algebra” might confuse a lay user). **Structure** ensures the *layout and visual flow* are easy to follow by organising content clearly through paragraphs, sections, and formatting, avoiding dense blocks of text (e.g., a response without breaks or clear segmentation).
:::

***

## Parameter 2: Persona Adherence

:::info
Assesses whether the model consistently adopts the voice or role expected (e.g., teacher, doctor, peer).
:::

### How to Approach?

1. **Identify the expected persona**: Is the model acting as a coach, expert, teacher, or casual peer? The prompt will often contain tone hints.
2. **Evaluate consistency**: Does the voice match throughout the entire response? Does it shift styles unexpectedly?

### Watch-outs

* **Jarring tone shifts**: A sudden switch from warm encouragement to rigid instruction can be disorienting.
* **Over-exaggeration**: A "pirate" persona doesn’t need to talk *only* in “Arrr!”, commitment is good, overdoing it isn’t.
* **Persona clash with content**: Using a playful voice in a serious legal or medical response may feel tone-deaf.

### Contrast: Persona Adherence Vs Other parameters

:::danger
* If the prompt **explicitly requests a persona** (e.g., “respond as a doctor” or “speak like a tutor”) and the model fails to adopt that role, the response reflects a failure in **both Persona Adherence** and **Instruction-Following**.
* **Tone** refers to the **emotional or stylistic quality** of the response (e.g., friendly, neutral, empathetic) and applies **regardless of whether a persona is requested**.
:::

***

## **Parameter 3:** Conciseness

:::info
Checks if the response avoids unnecessary repetition or filler, using efficient and precise language.
:::

### How to Approach?

* **Focus on value**: Every sentence (or paragraph) should meaningfully contribute to the user’s goal.
* **Look for common problems**: **Repetition** of the same idea in slightly different words. **Over-explaining** simple points beyond what the user needs. **Wandering** into tangents or non-essential information.

### Watch‑outs

* **Don’t cut clarity**: Conciseness should *enhance* clarity, not sacrifice it.
* **Precision ≠ brevity**: Short is not always concise. Precision matters more than length.
* **Contextual tolerance**: Formal explanations may allow slight elaboration for accessibility.
* **Avoid jargon stuffing**: Don’t substitute wordiness with dense technical language unless appropriate.

### Contrast: Conciseness Vs Other Parameters

:::danger
* **Conciseness** ensures nothing extra; **completeness** ensures nothing is missing. A balance is crucial.
* **Relevance** filters *what* should be said; **conciseness** trims *how much* is said.
:::

***

## **Parameter 4:** Structure

:::info
Looks at the visual and organisational layout-how well formatting (e.g., bullets, headings) supports readability.
:::

### How to Approach?

1. **Check formatting**: Are headings, paragraphs, bullet points, or other layout tools used to break up text effectively?
2. Assess **scannability**: Can a user visually parse key information at a glance?
3. Only judge **format and layout** — don’t consider flow of ideas or correctness here.

### Watch‑outs

* Structure is about how the content is visually presented — layout, segmentation, and formatting. It is not about idea clarity or logical order.
* A **wall of text** might be *clear* in language but still a *structural failure*.
* Conversely, a well-structured answer with clear bullets can still be **confusing in meaning** — that’s a *Clarity* issue, not Structure.

### Contrast: Structure Vs Other Parameters

:::danger
**Clarity** involves making the meaning of content easy to understand through careful wording, coherent phrasing, and avoiding overly technical or vague language, such as jargon-heavy statements ("The function evolves over an infinite-parameteral algebra"). **Structure**, on the other hand, focuses on organising content clearly, emphasizing visual flow and formatting (e.g., paragraphs and sectioning), while avoiding dense, uninterrupted blocks of text ("The entire response is a single block of text without any breaks or flow").
:::

***

## **Parameter 5:** Tone

:::info
Evaluates appropriateness and user-awareness in phrasing (friendly, empathetic, respectful).
:::

### How to Approach?

1. **Read the prompt carefully**: Is the user asking for advice, comfort, explanation, or critique? Tone should match the emotional need.
2. **Watch for red flags**: Preachy phrasing that might be lecturing the user (“You *should* always…”). Cold or dismissive tones (“That’s not a good idea.” without reasoning).
3. **Look for positive indicators**: neutral, friendly, respectful language; Tone is **aligned with user context**, not generic or mismatched.

### Watch‑outs

* **Don’t confuse tone with persona** – Tone is emotional/stylistic (e.g., warm, neutral); persona is role-based (e.g., a coach or doctor).
* **Tone matters even if not requested** – Evaluate appropriateness for the context, not just instruction compliance.
* **Watch for patronising or preachy phrasing** – Tone fails if the model sounds superior, moralising, or dismissive.
* **Separate tone from writing quality** – Clarity or verbosity issues belong elsewhere; don’t mislabel them as tone problems.

### Contrast: Tone Vs Other parameters

:::danger
* When a prompt **explicitly specifies a tone** (e.g., "write this apologetically") and the model fails to reflect it, this is a failure in both **Tone** and **Instruction Following**.
* In contrast, if no tone is specified, Tone is still rated based on **appropriateness to the situation and audience**, while Instruction Following may not be affected.
:::

***