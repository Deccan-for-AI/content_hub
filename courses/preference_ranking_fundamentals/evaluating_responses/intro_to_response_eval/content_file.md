# <span style="color:#364BC9">Introduction to Rubric Evaluation</span>

<video src="${PRIVATE_PREFERENCE_RANKING_VIDEO_4}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

## What is a Rubric?

A rubric is a structured evaluation guide used to assess the quality of model-generated responses. When comparing two or more outputs from an AI system (such as a language model), rubrics help human evaluators make consistent, informed decisions about which response is better-and why.&#x20;

Rubrics are foundational to training AI with Reinforcement Learning from Human Feedback (RLHF) or other comparative evaluation systems. They ensure that human preferences are captured systematically and can be used to optimise model behaviour.

## What are parameters?

The rubric used here is built on **20 parameters divided into 4 broad groups** in an increasing order of complexity to fine tune the model. Each parameter reflects a key factor that contributes to a high-quality, user-aligned AI response.

<img height="300" width="500" src="${PRIVATE_PREFERENCE_RANKING_IMAGE_5}" />

:::tip
💡 You can think of parameters as the “axes” of evaluation: a model output might be accurate but unclear, or clear but unhelpful. By splitting evaluation across parameters, we can more precisely identify strengths and weaknesses in model behaviour. Thus, each response is judged against a combination of parameters from different groups that are most important to that prompt.
:::

Don’t guess-**read the parameter explanations carefully** before scoring. The **interpretation of each parameter is contextual**, meaning:

* What “clarity” means for a programming answer might differ from what it means for a creative writing prompt.
* What qualifies as “utility” might vary between technical, educational, or conversational responses.

Your scoring should be **informed by these context-specific guidelines**, not just generic definitions.

### Rating Scale

<img height="400" width="600" src="${PRIVATE_PREFERENCE_RANKING_IMAGE_6}" />