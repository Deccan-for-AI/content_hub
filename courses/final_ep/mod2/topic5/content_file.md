# <span style="color:#364BC9">Handling Edge Cases - What If the Model Doesn’t Know?</span>

<video src="${PRIVATE_PROMPTING_VIDEO_7}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

### <span style="color:#364BC9">Why It Matters:</span>

In sensitive domains such as healthcare, finance, or model evaluation workflows (e.g., RLHF), inaccurate outputs can be misleading or harmful. AI models often generate guesses unless instructed otherwise.

**To improve output reliability, include a fallback clause:**

:::tip
Adding a fallback phrase improves response accuracy, reduces hallucination, and enhances safety, especially when prompting is used in high-stakes or auditable environments.
:::

### <span style="color:#364BC9">Example:</span>

* **Basic** -  *“Summarise expert views on AI in national security.”*
* **Refined** - *“Summarise expert views based on published sources. If no consensus exists, say: ‘Conflicting opinions found.’”*

### <span style="color:#364BC9">Edge-Case Instructions:</span>

* “If unsure, say: ‘Not enough information available.’”
* “If the answer is uncertain, respond: ‘Insufficient data.’”
* “If examples don’t apply, return: ‘No relevant match found.’”
* “Avoid speculation. Add a disclaimer if information may be biased.”

#### 💡 Edge-case handling helps test a model’s ability to:

* Admit uncertainty
* Follow safety-conscious instructions
* Distinguish between knowns and unknowns