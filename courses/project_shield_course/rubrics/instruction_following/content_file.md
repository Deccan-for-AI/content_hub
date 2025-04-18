# Rubric 2: Instruction Following

<video src="${PRIVATE_INSTRUCTION_FOLLOWING_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

**Intent of Instruction Following:**

* The model should follow all explicit and implicit instructions given in the prompt.&#x20;
* Responses should not circumvent the task or provide unwarranted refusals unless they involve safety concerns.&#x20;
* Look at the table below for the categories of this rubric.

### **How should you approach this rubric?**

1. The focus of this rubric is the response.
2. Check to see if all the intents of users are addressed in the response.
3. Do not check if the claims made in the response are correct or not.

| Category           | Criteria                                                                                                                                                              |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | Response follows each one of the instructions in the prompt and completely fulfils the user intent. The response can is as helpful as it can be.                      |
| **Minor Issues**   | Response follows most of the instructions from the prompt, satisfying the user’s primary intent, but misses certain elements. The response is only partially helpful. |
| **Major Issues**   | The response ignores or avoids answering key parts of the prompt, making the response unhelpful to the user.                                                          |
| **Not Applicable** | There are no explicit or implicit instructions given in the prompt (e.g. “I like clouds”, “The rainbow is pretty”…)                                                   |

### **Suggested Best Practices**

:::tip
* Take a notepad and underline the different instructions present in the prompt.
* Do not give importance to order of the instructions unless it is given in the prompt explicitly.
* Check the model’s response on every underlined instruction.
:::

### **Example**

> User Prompt: "**Write a short paragraph explaining how solar panels work, and include a metaphor to make it easy to understand for kids."**

| Category       | Response                                                                                                                                                                                                        | Explanation                                                                                                                             |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| No issues      | Solar panels work by capturing sunlight and turning it into electricity using special cells called photovoltaic cells. It’s like a magic sponge that soaks up sunshine and squeezes out power to run your home! | ✔️ Explains how solar panels work. ✔️ Uses a metaphor. ✔️ Written in a fun, kid-friendly way.                                           |
| Minor Issues   | Solar panels turn sunlight into electricity using photovoltaic cells. It’s a great way to power your home.                                                                                                      | ✔️ Explains how solar panels work. ❌ Misses the metaphor. ➡️ It’s still helpful and addresses the main intent but isn’t fully complete. |
| Major Issues   | Solar panels are used in many homes these days. They are becoming more popular around the world.                                                                                                                | ❌ Doesn’t explain how solar panels work. ❌ No metaphor. ➡️ Completely skips the instructions—major issues here.                         |
| Not Applicable | I love how sunny days make everything brighter.                                                                                                                                                                 | This is just a statement with no instructions, so this rubric doesn’t apply.                                                            |