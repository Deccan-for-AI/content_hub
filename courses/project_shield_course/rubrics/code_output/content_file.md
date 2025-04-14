# Rubric 11: Code Output

<video src="${PRIVATE_CODE_OUTPUT_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

***Intent of Code Output:***

* Code Output refers to how well the model’s code output aligns with the user’s input.
* The goal of code output is to ensure that the response includes sufficient, accurate, and relevant information to fully capture the user's intent.
* A high-quality grounded response may also provide additional information that enriches the user's understanding or enhances the response beyond the original prompt.


***How should you approach this rubric?***

Check if the user’s intent has been addressed in the grounding information/code output.&#x20;

**Evaluation Categories for Grounding Information Quality:**

| Category           | Criteria                                                                                                                                                                                |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | The code output is correct and includes all the information to satisfy the user intent. May include relevant information beyond what the user asked for but that enriches the response. |
| **Minor Issues**   | The code output includes information that doesn’t completely satisfy the user intent. The code output contains some incorrect information.                                              |
| **Major Issues**   | The code output fails to satisfy the intent of the user and doesn’t provide a useful response. The code output includes incorrect information and therefore the answer is wrong.        |
| **Not Applicable** | If no code output/grounding information is present.                                                                                                                                     |

**Example**
<video src="${PRIVATE_CODE_OUTPUT_EXAMPLE_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />