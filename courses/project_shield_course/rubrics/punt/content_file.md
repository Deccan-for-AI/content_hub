# Rubric Evaluation

<video src="${PRIVATE_RUBRIC_EVAL_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

***

# Rubric 1: Punt

<video src="${PRIVATE_PUNT_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

If a model refuses to answer the prompt, this should be considered as a ‘punt’.&#x20;

### **How should you approach this rubric?**

* The focus of this rubric is the response.&#x20;
* Check to see if the response doesn’t answer the prompt.&#x20;

| Categories                        | Criteria                                                                                                                                                                                                                                                              |
| --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Response is a punt**            | Examples - “Sorry, a response could not be produced”, “As an AI language model, I can’t access recent information”                                                                                                                                                    |
| **Response is a useful punt**     | The response doesn’t answer the prompt directly, does it still provide some related yet useful information or alternative solutions to find an answer. If yes, add in the comment box to explain how the related information or alternative solutions may be helpful. |
| **Response is not a useful punt** | The response does not provide any related useful information or alternative solutions to find an answer.                                                                                                                                                              |
| **Response is not a punt**        | The response is not a punt. It has answered the user query as a normal response.                                                                                                                                                                                      |

### **Example**

User Query: ***"Who won the FIFA World Cup in 2022?"***

| Model Response                                                                                                                                                                                                            | Category                          | Why?                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- | ---------------------------------------------------------------------------------------------- |
| "Unfortunately, I was unable to produce a response ”, “As an AI language model, I can’t perform this action”                                                                                                              | **Response is a Punt**            | The model provides just a statement denying the user’s query.                                  |
| "Argentina won the 2022 FIFA World Cup, defeating France in a dramatic penalty shootout."                                                                                                                                 | **Response is Not a Punt**        | This directly answers the prompt, therefore not a punt.                                        |
| "As an AI language model without real-time data access, I can’t provide the winner of the 2022 FIFA World Cup. However, you can check the official FIFA website or a reliable news source for the most accurate results." | **Response is a Useful Punt**     | It punts the question but still provides helpful guidance, therefore a useful punt.            |
| "Sorry, I can’t provide that information." However, you can check the highlights of Slum Soccer’2024 on google for the details.                                                                                           | **Response is Not a Useful Punt** | It punts  and gives no helpful context or alternative information therefore not a useful punt. |

***