# Rubric 8: Truthfulness

<video src="${PRIVATE_TRUTHFULNESS_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

**Intent of Truthfulness:**

* The goal of truthfulness is to ensure that all factual claims made in the response are accurate and supported by reliable, reputable sources.
* Fact-checking is essential to guarantee the integrity of the response, especially when it includes information that the user might rely on.
* If the tool output is provided it should be used as one of the sources of truth when assessing the truthfulness of the final response.
* Check the model for hallucinations.

**How should you approach this rubric?**

1. The focus of this rubric are the **factual claims in the response**.
2. Identify the Primary and secondary claims in the response first
   * ***Primary Claims** - Claims about the intents mentioned in the user's prompt.*
   * ***Secondary Claims** - Claims unrelated to intents mentioned in the user’s prompt.*
3. The source of truth will always be the grounding information.
4. If and only if the grounding information is absent from the task, try to look for any links that are mentioned in the response itself.
5. If there are no links mentioned in the response as well, take 15 minutes to google search and verify the claims and mark accordingly.



:::caution
💡 **What are Hallucinations?**&#x20;

Hallucinations in an AI model refer to instances where the model generates information that is incorrect, nonsensical, or fabricated but presented as factual or coherent. However, the model may generate data that is not backed up by evidence in creative tasks (e.g. story writing), and is not considered as a hallucination in such cases.
:::

| Category           | Criteria                                                                                                                                                                                                                                                                                        |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | All claims are grounded and supported by usable information.                                                                                                                                                                                                                                    |
| **Minor Issues**   | Primary claims (necessary for addressing the prompt) are accurate and supported by usable information, but at least one secondary claim is inaccurate or not supported by usable information.                                                                                                   |
| **Major Issues**   | •The code or the code output are incorrect and therefore the final response is inaccurate. The code in the response or the code output are correct but the final response is hallucinated.                                                  •If claims are not supported by usable information. |
| **Cannot Assess**  | Cannot determine validity of all the claims made in the response. Select this option if properly researching the claims in the response would take more than 15 minutes. Mark this is Response is a Punt.                                                                                       |
| **Not Applicable** | The response does not have any explicit or implicit factual claims.                                                                                                                                                                                                                             |

:::info
**💡 What to do to check the correct information for variable metrics?**


For information that should come from a tool output, meaning one of the tool APIs is specialised for the user query, we should consider the tool output as the only source of truth. The model without the use of extensions tools does not have access to real time data. Meaning, when the model presents a list of hotels with prices, or a list of flights, and the tool output does not show this information, we can consider this to be unsupported information and thus major issues.
:::