# <span style="color:#364BC9">Formatting Your Output — Get Clean, Usable Responses</span>

<video src="${PRIVATE_PROMPTING_VIDEO_6}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

### <span style="color:#364BC9">Why Formatting Matters:</span>

Language models mimic structure as well as content. Without clear format instructions, responses may default to free text or inconsistent layouts.

### <span style="color:#364BC9">Prompt Refinement Example:</span>

* **Basic** - *“What are 3 climate policies?”*
* **Refined** -  *“List 3 climate policies in a table with columns: Policy | Country | Year.”*

### <span style="color:#364BC9">Common Formatting Instructions:</span>

* “List in bullet points”
* “Number the steps from 1 to 5”
* “Return as a markdown table with two columns”
* “Reply in JSON with keys for title, author, and summary”
* “Write two short paragraphs, 3 sentences each”
* “Only output the headline — no explanation”

#### 💡 Use in SFT and RLHF - Formatting is essential when creating:

:::caution
* Supervised fine-tuning (SFT) training samples
* Evaluation prompts with consistent structure
* Model outputs intended for annotation or downstream tasks
:::