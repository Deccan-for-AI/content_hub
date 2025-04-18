# Rubric 11: Code Output

<video src="${PRIVATE_CODE_OUTPUT_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

#### Intent of Code Output:

* Code Output refers to how well the model’s code output aligns with the user’s input.
* The goal of code output is to ensure that the response includes sufficient, accurate, and relevant information to fully capture the user's intent.
* A high-quality grounded response may also provide additional information that enriches the user's understanding or enhances the response beyond the original prompt.

### How should you approach this rubric?

Check if the user’s intent has been addressed in the grounding information/code output.&#x20;

### Evaluation Criteria with Examples

| Category           | Criteria                                                                                                                                                                                | Example                                                                                                                                                                                                                                                                                 |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | The code output is correct and includes all the information to satisfy the user intent. May include relevant information beyond what the user asked for but that enriches the response. | \[ { "airline": "Delta", "price": "$450", "departure": "2025-04-28 13:00", "duration": "14h 35m" "from": "new york" "destination": "Tokyo" }, { "airline": "ANA", "price": "$480", "departure": "2025-04-29 15:20", "duration": "13h 55m" "from": "new york" "destination": "Tokyo" } ] |
| **Minor Issues**   | The code output includes information that doesn’t completely satisfy the user intent. The code output contains some incorrect information.                                              | \[ { "airline": "Delta", "departure": "2025-06-28 13:00", "duration": "14h 35m" }, { "airline": "ANA", "departure": "2025-05-30 15:20", "duration": "13h 55m" } ]                                                                                                                       |
| **Major Issues**   | The code output fails to satisfy the intent of the user and doesn’t provide a useful response. The code output includes incorrect information and therefore the answer is wrong.        | \[ { "airline": "Delta", "duration": "14h 35m" }, { "price": "$480", "duration": "13h 55m" } ]                                                                                                                                                                                          |
| **Not Applicable** | If no code output/grounding information is present.                                                                                                                                     | No tool code/tool call made, only textual explanation.                                                                                                                                                                                                                                  |