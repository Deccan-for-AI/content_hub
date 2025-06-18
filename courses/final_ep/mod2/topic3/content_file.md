# <span style="color:#364BC9">Adding Scope & Constraints</span>

<video src="${PRIVATE_PROMPTING_VIDEO_4}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

&#x20;Constraints serve as boundaries that improve focus, reduce unnecessary detail, and ensure responses are structured and usable.

### <span style="color:#364BC9">Why Constraints Matter:</span>

**❌  Without defined limits, models may**:

* Over-explain
* Include irrelevant information
* Hallucinate or fill in content unnecessarily

**✅  With constraints, output becomes**:

* Concise
* Aligned with purpose
* Easier to evaluate or reuse

### <span style="color:#364BC9">Prompt Refinement Example:</span>

* **Basic** - “*Summarise this report.*”
* **Refined** -  “*Summarize in 3 bullets, each under 15 words, focusing only on policy recommendations.*”

### <span style="color:#364BC9">Common Constraint Types:</span>

* **Length**: “In 280 characters or less”
* **Time scope**: “Focus only on events after 2020”
* **Content focus**: “Only include economic factors”
* **Perspective**: “From the point of view of a new user”
* **Output format**: “Respond in a table format”
* **Exclusion**: “Avoid mentioning brand names”

#### 💡 In model evaluation and dataset generation (e.g., SFT), constraints help test how well a model can:

:::tip
* Follow strict instructions
* Avoid prohibited content
* Maintain structure and clarity under limitations
:::