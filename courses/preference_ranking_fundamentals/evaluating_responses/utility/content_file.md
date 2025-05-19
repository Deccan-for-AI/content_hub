# <span style="color:#364BC9">Parameters that Evaluate Utility</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_7}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

:::tip
* Actionability
* Collaborativity
* Resourcefulness
* Depth
* Context Awareness
:::

***

## **Parameter 1:** Actionability

:::info
Evaluates whether the response gives clear, practical steps the user can take.
:::

### How to Approach?

1. **Look at the user’s intent**: Are they asking for a plan, process, guide, recommendation, or fix?
2. **Check for concrete outputs**: Does the response provide a **list of steps**, **tools**, **tips**, or **decisions**? Would the user know exactly what to do next?

### Watch‑outs

* Ask yourself: *Can the user actually do something right now with this information?*
* Even with correct facts or tone — **if the user can’t apply it, it’s not actionable**.

### Contrast: Actionability Vs Other parameters

:::danger
* ***Helpfulness*** is about **relevance and value** to the user's goal. A helpful response may summarise background or clarify concepts-but if it doesn't tell the user **what to do next**, it may lack **Actionability**.
* ***Resourcefulness*** is about **knowing when and how to bring in extra tools, sources, or data**. It supports actionability, but a response can be resourceful (e.g., linking a paper) without itself giving **direct steps**.
* **Collaborativity** is about being an engaged, flexible partner-adapting to the user’s needs, inviting clarification, or offering alternatives. A response may be collaborative and conversational, but if it doesn’t offer concrete steps or solutions, it may lack **Actionability**.
:::

***

## Parameter 2: Collaborativity

:::info
Evaluates how well the model engages the user in dialogue, invites feedback, or supports iterative interaction.
:::

### How to Approach?

To evaluate collaborativity, look for signals that the AI is trying to:

1. **Engage the user in dialogue** rather than delivering a static response.
2. **Anticipate next steps** in open-ended or ambiguous tasks.
3. **Ask clarifying or follow-up questions** to refine or personalize the answer.
4. **Offer options**, alternatives, or flexible suggestions that invite participation.

### Watch-outs

* **Over-helping isn’t collaboration**: Just being verbose doesn’t mean the response is collaborative, look for *user-oriented engagement*.
* **“Let me know…” ≠ meaningful collaboration**: Phrasing like “let me know if you have questions” is polite, but without follow-through or options, it may feel hollow.
* **Avoid shutting down dialogue**: Responses that end with “this is the best approach” or “you don’t need to do anything else” close off collaboration prematurely.

### Contrast: Collaborativity Vs Other parameters

:::danger
* **Actionability** is about giving clear, usable steps. A response might outline a great plan but feel one-sided or rigid if it doesn’t engage with the user’s constraints or invite iteration-lacking **Collaborativity**.
* **Helpfulness** is about relevance and value to the user’s goal. A helpful response may solve the problem directly, even if it doesn’t adapt to the user’s evolving needs-making it low on **Collaborativity**.
:::

***

## **Parameter 3:** Resourcefulness

:::info
Measures the model’s ability to recognise and provide when external tools, sources, or deeper inquiry would benefit the user.
:::

### How to Approach?

1. **Ask**: Would a resource, tool, or link enhance this response? If yes, did the model recognise and act on that need?
2. **Look for relevance**: Was the resource **well-matched** to the user’s query and level of expertise? Did it feel **context-aware**, not just tacked on?

### Watch‑outs

* **Relevance over quantity**: A **single well-matched tool or resource** is better than 3 generic ones.
* **Don’t force tool use** where it adds no value.
* **Internal tools** (charts, maps, calculators) and **external references** (e.g., Stack Overflow, GitHub, academic papers).
* Avoid linking to **outdated**, **broken**, or **unreliable** sources.

***

## **Parameter 4:** Depth

:::info
Evaluates whether the response shows nuanced reasoning and explores complexities beyond surface-level answers.
:::

### How to Approach?

1. **Check for analysis, not just description**: Does the response unpack ideas or just name them?
2. **Look for nuance and balance**: Are different angles, exceptions, or trade-offs considered?
3. **Spot reasoning**: Does the model explain *why* something matters-not just *what* it is?
4. **Depth ≠ length**: A long response can still be shallow. The key is **conceptual richness**.

### Watch‑outs

* **Buzzword flooding**: Throwing in jargon without actually explaining it.
* **False balance**: Pretending two sides are equally valid without weighing evidence.
* **Superficial structure**: A list of points ≠ deep engagement with the topic.

### Contrast: Depth Vs Other Parameters

:::danger
* **Completeness** analyses coverage of parts, does the response *mention everything* relevant to the prompt?
* **Helpfulness** looks at practical value, does this response actually *move the user forward* in solving their problem?
:::

***

## **Parameter 5:** Context Awareness

:::info
Checks whether the model remembers and meaningfully builds on earlier turns, incorporating user-stated facts, preferences, and tone to maintain coherent, personalised dialogue.
:::

### How to Approach?

1. **Read the entire exchange** (not just the current prompt).
2. Identify relevant context: facts, requests, tone, preferences.
3. See if the model’s reply actively builds on or at least respects that information.
4. Watch out for **false memory** or outdated references.

### Watch‑outs

* **Name switches**: Referring to a person or item differently than before (e.g., “Project Phoenix” becomes “Project Aurora”).
* **Goal drift**: Forgetting a user’s core aim across turns.
* **Tone mismatch**: Jumping from casual to overly formal when the context hasn’t changed.

### Contrast: Context Awareness Vs Other parameters

:::danger
* **Context Awareness**: Memory across turns (Forgets that the podcast is for teens, uses business lingo)
* **Relevance:** Staying on-topic (Shifts from science to marketing)
:::

***