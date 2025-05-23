# Evidencing the right way

<video src="${PRIVATE_VIDEO_RAG_4}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

Take a quick look at the query creation process here:

<a href="${INTERNAL_LINK}" target="_blank" rel="noopener noreferrer">
  Click here
</a>

***

Evidencing is the cornerstone of effective information retrieval. This is how you train the model to justify its accuracy. It serves as a guide, enabling the model to pinpoint the exact source and context of the information it uses. To ensure seamless and accurate retrieval, every evidence should include the following key elements.

| Element                                  | Description                                                    | Why do you need to state it?                                                                                                                                                      |
| ---------------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Document URL (Publicly Accessible)       | The link to the document that is being used as the data source | Provides the exact location of the document, allowing the model or user to trace the source.                                                                                      |
| Page Number                              | The relevant page where the answers are                        | Directs the retrieval process to the specific section of the document where the information is located.                                                                           |
| Evidence Text                            | Paragraph, table, or image that contains the answer            | Helps narrow the scope of retrieval to the relevant thematic area within the document.                                                                                            |
| Span                                     | Relevant words/numbers/sentences that are the answers          | Ensures the model has precise and contextual input, reducing the likelihood of errors.                                                                                            |
| Span Rating (0-3 rating explained below) | Rate the span based on how well it answers the query           | Helps evaluate how well the selected span supports the answer.                                                                                                                    |
| Span Type                                | The type of evidence you are using                             | Helps the model understand the format and structure of the retrieved evidence. This distinction allows the model to interpret, process, and present information more effectively. |

:::caution
**Span Rating Criteria:**

1- The Span doesn’t answer the query but can be a keyword for the query

2- The Span is answering the query but not the complete answer

3- The Span contains the complete answer

0- If you don’t have a span (Hypothetical case)
:::

***

## Example:

:::info
**Evidence\_1**

**Document URL:** [https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf](https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf)

**Page number:** 12

**Evidence Text:** The Learning Passport, an innovative mobile learning platform, was launched in 7 countries, reaching a total of 38, with over 6 million registered users and an offline solution for schools with limited to no connectivity.

**Span:** The Learning Passport

**Span Rating:** 2

**Span Type:** Text



**Evidence\_2**

**Document URL:** [https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf](https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf)

**Page number:** 13

**Evidence Text:** UNICEF launched the Five Million Futures action and advocacy framework to mobilize support for over 50 countries to scale up evidence-based interventions around early learning, parenting support, and the transition to primary education. UNICEF also supported systems strengthening approaches, including alternative learning pathways to prepare adolescents for re-enrollment or work, strengthening curricula to integrate a full range of skills, and supporting school-to-work transition and community-based skills development programmes.

**Span:** Five Million Futures

**Span Rating:** 2

**Span Type:** Text



**Evidence\_3**

**Document URL:** [https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf](https://www.unicef.org/media/157491/file/UNICEF%20Annual%20report%202023%20EN.pdf)

**Page number:** 29

**Evidence Text:** UNICEF strengthened foundational learning systems in 16 countries; digital learning systems in six countries through the Airtel partnership; and accelerated girls’ education results and gender-responsive education sector plans in seven countries. UNICEF also supported disability inclusive national education strategies in nine countries.

**Span:** strengthened foundational learning systems

**Span Rating:** 2

**Span Type:** Text
:::