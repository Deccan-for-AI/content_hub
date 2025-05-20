# <span style="color:#364BC9">Preference Ranking in RLHF</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_3}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

**Reinforcement Learning from Human Feedback (RLHF) uses preference ranking as a core component to train Large Language Models.**&#x20;

Preference Ranking is a method where human evaluators compare multiple AI-generated responses to a given prompt according to specific parameters, such as accuracy, clarity, helpfulness, or alignment with instructions, and rank one of the two responses to be a better one. Preference Ranking helps identify responses that humans prefer, directly influencing how the model learns and improves over time.

<img height="400" width="600" src="${PRIVATE_PREFERENCE_RANKING_IMAGE_3}" />

## Preference Ranking: The Process

<img height="200" width="500" src="${PRIVATE_PREFERENCE_RANKING_IMAGE_4}" />

#### **1. Start with the user’s intent**

Start by carefully reading the user prompt. Go beyond the literal request—try to understand the user's **underlying goal** and **context**:

* What problem are they trying to solve?
* Are they looking for a quick solution, an in-depth explanation, or creative inspiration? Do they expect a factual summary, or a step-by-step guide?

Understanding the "**why**" behind the "**what**" is crucial for fair evaluation.

#### **2. Evaluation of responses along parameters**

With the user's intent in mind, examine the first AI-generated response. Assess it independently using the standardized rubric. You will begin by using the provided parameters in the rubric to analyze various aspects of the response. Parameters could include clarity, relevance, depth of information, and overall helpfulness. Assign ratings based on how well the response meets these criteria. **Similarly, response two must be evaluated.**

#### **3. Comparative Ranking on the Likert Scale**

Once both responses have been evaluated, rate them **relative to each other** using a **1–7 Likert scale**.

#### **4. Justify your reasoning**

Conclude by writing a **concise but insightful justification** for your chosen score. This is the one of the most critical parts of the process, as it reflects your analytical reasoning and highlights what made one response stronger (or why both were equal). Refer to justification writing guidelines

:::tip
**💡 Think Like the User**. It’s not just about correctness. The best response is the one that helps the user clearly, effectively, and responsibly.
:::