# <span style="color:#364BC9">Prompting Techniques | Part 2</span>

<video src="${PRIVATE_PROMPTING_VIDEO_10}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

## Chain-of-Thought (CoT) Prompting

**Chain-of-Thought prompting**, is a technique that guides the model to reason step by step rather than producing a final answer immediately. This improves accuracy on multi-step tasks and reveals reasoning errors early.

#### Use Cases:

* Math and logic problems
* Multi-variable policy or risk analysis
* Structured decision-making tasks

### Example

**Scenario:** Estimating carbon footprint reduction for a delivery fleet switching to electric vehicles.

**Prompt with CoT:**

:::tip
*"You are an environmental data analyst.*&#x20;

1. *Show all steps*
2. *Compute annual reduction*
3. *Calculate emissions for diesel and electric vehicles*

*Finally, summarize the annual CO₂ savings.”*
:::

### Best Practices:

:::tip
* **Use CoT instructions:** “Explain your reasoning step by step before giving the final answer.”
* **Break into stages:** For complex logic, use numbered sub-steps (e.g., Step 2a, 2b).
* **Prompt with scaffolds:** Add cues like “Let’s think this through” or “Break it down logically.”
* **Confirm intermediate values:** Ask the model to verify calculations before moving forward.
:::

***

## Tree-of-Thought (ToT) Prompting

**Tree-of-Thought prompting**, is a technique that enables models to explore multiple reasoning paths in parallel before selecting the best outcome. It’s especially useful for decision-making, creative generation, and complex evaluations.&#x20;

#### Use Cases:

* Strategic decisions
* Product or policy design
* Story branching or idea generation

### Example

**Scenario:** Expanding rural internet access
**Prompt:**

:::tip
*“List 3 strategies for expanding rural internet access. For each, outline pros, cons, and a final recommendation. Rate feasibility (1–5), then compare all options based on cost, impact, and complexity.”*&#x20;
:::

### Best Practices:

:::tip
* **Guide branch-level reasoning:** Include prompts for individual evaluation of each option.
* **Limit branch depth:** Add constraints like “explore at most two sub-options.”
* **Structure for comparison:** Request summary tables or side-by-side analysis before final selection.
* **Encourage synthesis:** Prompt with “After evaluating all branches, choose the most viable option with justification.

ToT prompting enables more nuanced, reflective model behaviour by simulating comparative decision-making, ideal for high-complexity or creative tasks.
:::

###