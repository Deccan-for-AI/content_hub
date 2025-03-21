# Getting Better Responses from LLMs with Prompting Techniques

<video src="${PRIVATE_PROMPTING_101_VIDEO_3}" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

Think of prompting as giving instructions. If one way doesn’t work, you try another—just like explaining directions to a friend using landmarks or a map. Language models work similarly. Different tasks need different prompting techniques to get the best results.

Sometimes, showing examples helps (**Few Shot method**). For more complex reasoning, breaking down tasks step-by-step (**Chain of Thought method**) or exploring multiple possibilities works better (**Tree of Thought method**).

In the next few sections we’ll look at the three methods mentioned here. Learning these techniques is like adding tools to your problem-solving toolbox.

<img height="900" width="900" src="${PRIVATE_PROMPTING_101_8}" />

## Few-Shot Prompting

Imagine learning a new card game. If someone explains the rules with just a few example rounds, you quickly pick up the gameplay and can play on your own.

This is how **Few-Shot Prompting** works for language models. You show the model a few examples, and it learns the pattern to respond correctly.

> ### Why Few-Shot Prompting Works:-**Clear Guidance:** Learning from examples reduces ambiguity and sets clear expectations.-
> **Better Answers:** With a few examples, the model understands the task and produces more accurate responses.

***

### ✅ Steps to Few-Shot Prompting:

1. Provide sample Q\&A with correct answers to set a pattern.
2. After seeing a few examples, the model applies the pattern to new prompts—even if the exact answer wasn’t shown earlier.

***

### Example:

```txt
❌ Classify the following product review:  
   "The battery life is great, but the camera quality could be better."  
   as Positive/Neutral/Negative.
```

<img height="900" width="900" src="${PRIVATE_PROMPTING_101_9}" />