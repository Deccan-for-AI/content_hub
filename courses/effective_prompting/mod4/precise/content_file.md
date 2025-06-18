# <span style="color:#364BC9">The P.R.E.C.I.S.E. Framework</span>

<video src="${PRIVATE_PROMPTING_VIDEO_11}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

### The P.R.E.C.I.S.E. framework is a comprehensive checklist for building high-quality prompts, particularly in high-stakes environments like SFT and RLHF.

:::tip
Each letter represents a key design component to ensure prompts are complete, structured, and safe:

* **P – Purpose & Persona**
  Define the prompt’s goal and speaker’s role.
  ***Tip**:* Start with “You are a…” to fix identity and tone.
* **R – Requirements & Restrictions**
  Set clear boundaries (e.g., word limits, tone, exclusions).
  ***Tip**:* Be explicit about constraints to avoid ambiguity.
* **E – Examples**
  Show 1–2 samples to model the target output.
  ***Tip**:* Crucial in few-shot or training contexts.
* **C – Context & Background**
  Anchor the task in a clear setting or scenario.
  ***Tip**:* Reduces hallucination and increases precision.
* **I – Instruction Structure**
  Lay out the format or flow clearly.
  ***Tip**:* Use steps or sections for clarity and control.
* **S – Style & Sensitivity**
  Specify tone, voice, and any cultural considerations.
  ***Tip**:* Define style explicitly, especially for public-facing content.
* **E – Evaluation & Refinement**
  Build in self-checks or alternate outputs.
  ***Tip**:* Useful in reward modelling or iterative workflows.&#x20;
:::