# <span style="color:#364BC9">Prompting Techniques | Part 1</span>

<video src="${PRIVATE_PROMPTING_VIDEO_9}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

## <span style="color:#364BC9">**Instruction Chaining**</span>

**Definition:** Breaking down a complex task into step-by-step instructions that the model completes in sequence.

**Why It Works:**

* Reduces ambiguity and skips
* Mimics logical, human-like reasoning
* Improves task adherence and structure

:::tip
**Tip:** Use explicit stepped numbers and include: *“Do not proceed to step 2 until step 1 is complete.”* when strict order is required.
:::

***

## <span style="color:#364BC9">**Few-Shot Prompting**</span>

**Definition:** Teaching the model using 1–2 solved examples before asking it to perform a similar task.

**Why It Works:**

* Aligns tone, logic, and structure
* Minimizes iteration and misunderstanding.
* Ideal for creative or nuanced tasks (e.g., titles, summaries, rewrites)

:::tip
**Tip:** Use examples that closely resemble the output you want-format, tone, and complexity matter.
:::

###