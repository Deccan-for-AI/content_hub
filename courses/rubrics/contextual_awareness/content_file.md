# Rubric 3: Contextual Awareness

<video src="${PRIVATE_CONTEXTUAL_AWARENESS_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

### Intent of Contextual Awareness:

💡 <u>Usually you have two set of conversations</u> :

***Single Turn*** A single-turn conversation consists of one interaction between the user and AI, where the AI responds once, and the conversation ends.

**For Example**&#x20;

:::caution
**User:** "What is the capital of France?"                                                                                          **AI:** "The capital of France is Paris."
:::

***Multi Turn*** A multi-turn conversation involves multiple exchanges between the user and AI, with back-and-forth dialogue continuing beyond the initial response.

**For Example**&#x20;

:::caution
**User:** "Can you recommend a good book?"                                                                              **AI:** "Sure! What genre are you interested in?"                                                                     **User:** "I enjoy science fiction."                                                                                                       **AI:** "I recommend Dune by Frank Herbert. It's a classic science fiction novel with a rich universe and complex characters. Would you like to know more about it?"
:::



* The goal of contextual awareness is to evaluate how well the AI Assistant remembers and incorporates information from earlier in the conversation (multi-turn conversation).&#x20;
* A contextually aware response should demonstrate a clear understanding of the ongoing dialogue, referencing previous exchanges to provide coherent and relevant responses.
* It should maintain continuity and consistency, ensuring that prior details, instructions, and constraints are acknowledged and integrated into its answers.

### *How should you approach this rubric?*

1. Check if there are any previous conversations between model and the user (it should be a multi-turn).
2. If it’s a multi turn task (previous conversation is available), check if the model is effectively remembering and building upon information and instructions from previous prompts.
3. If it’s a multi turn task (previous conversation is available), but the prompt is not related to the previous conversation at all, go for no issues.
4. If its a single-turn, go for N/A - Not Applicable

**Let’s understand the categories of this rubric in detail based on the multi turn conversation above.**

| Category           | Criteria                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | • This response consistently recalled and built upon information from the previous conversations.                              • It demonstrated a clear understanding of the ongoing context, referencing and incorporating details from earlier exchanges to provide coherent, relevant, and personalised responses.                                                                                                                |
| **Minor Issues**   | • The response partially recalled and built upon information and instructions from previous turns and from the context for the user prompt, but there were a few instances where it could have done so, more effectively.                                                         • It may have occasionally missed minor details, slightly misinterpreted prior statements, or failed to incorporate certain information seamlessly. |
| **Major Issues**   | • The response struggled to consistently remember or build upon information and instructions from previous conversations including the user prompt.                                                    • It frequently contradicted earlier statements, failed to take into account previously communicated constraints or important details, or provided responses that seemed disconnected from the ongoing conversation.           |
| **Not Applicable** | Response is the first turn in conversation.                                                                                                                                                                                                                                                                                                                                                                                           |