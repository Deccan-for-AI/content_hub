# Rubric 10: **Code**

<video src="${PRIVATE_CODE_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

##### **What is a tool call/ tool code?**

* To generate the responses, there are API calls made that contain following components (1) Tools, (2) Tool Methods, (3) Parameters, and (4) Processing/Reasoning Logic.
* To generate good quality responses the model needs to use the right tools ensuring the response generated aligns with the user’s query.

### **Intent of Code Quality:**

* The goal of tool calls is to ensure that the code provided in the response utilises the most appropriate **tools, functions, and parameters** to fulfil the user's intent.
* The response should effectively capture and execute the user's request by leveraging the correct coding elements. This evaluation ensures that the code is efficient, accurate, and relevant to the task, providing the best possible outcome based on the user's prompt and context.

##### **💡 IMPORTANT**

:::danger
1. Check whether the code includes the right information to address the user's request.
   * Examples: google\_flights.search, google\_hotels.search\_hotels, gemkick\_corpus.search, etc
2. Check whether the code uses the correct parameters to address the user's request. Checking the comment in the code and the output of the code execution can help you assess the code accuracy. *Don't assess the verbosity or formatting of the 'output' because it's not the output to the user.*
   * Taking google\_flights.search for example, the function parameters are destination, origin, latest\_departure\_date, etc
:::

### **How should you approach this rubric?**

1. There are three parts to a code, (i)Tools, (ii)Functions, (iii)Parameters.
2. If a wrong tool has been used as the first tool call, mark it as a Major issue
3. If a wrong tool has been used as the first tool call, but the model eventually deploys the correct tool later, mark it as minor issues.
4. If there are missing functions and parameters in a correct tool, mark it as minor issue
5. Pay attention to multi-tool usage in the task, where more than one tool has been used. The efficiency of tool use sequence should be judged and inefficient sequence of tool usage should be penalised.

💡 For example, if the user requests for videos in their prompt, the model should use YouTube to generate the most ideal response. Using google search for videos might not generate the most relevant and good quality videos.&#x20;

#### **Tools available to the model:**

| Tools available to the model | Purpose most ideal for                                                                                                                                                                                                                                                                                            |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Youtube 📹                   | Search for videos, associated information, and YouTube content                                                                                                                                                                                                                                                    |
| Google\_maps 🗺️             | Location searches, directions                                                                                                                                                                                                                                                                                     |
| Google\_search 🔎            | Search the web and provide relevant results                                                                                                                                                                                                                                                                       |
| Google\_flights ✈️           | Search for flights, compare prices, and look at other flight related data (like flight durations)                                                                                                                                                                                                                 |
| Google\_hotels 🏨            | Search for hotels and compare prices                                                                                                                                                                                                                                                                              |
| Browsing\_tool 📚            | For fetching URL content and summarisation                                                                                                                                                                                                                                                                        |
| Workspace\_tool ✏️           | Interact with Google Slides, Docs, Sheets, Gmail. The content\_fetcher library enables retrieving the full content or metadata of items. These could be files uploaded by the user, images, code files, documents from Google Drive, or emails from Gmail. Also, ‘gemkick\_corpus’ fetches Google workspace data. |
| Data Commons(rare) 📚        | Utilize public data sets                                                                                                                                                                                                                                                                                          |

:::tip
**Note**: This is not an exhaustive list, it may use tools that are not mentioned here. If the model uses a **new tool** that is **relevant to the query**, do not penalise the model.
:::

### **Rating Criteria:**

| Category           | Criteria                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **No issues**      | The code successfully captures as much as possible from the user intent and uses the correct tool(s), functions(s) and parameter(s) to create a useful response. **\|** In multi-tool scenarios, the model sequences the tool calls efficiently and takes into account all dependencies when setting the tool call order.                                                                                          |
| **Minor Issues**   | The code partially satisfies the user intent. Better tool functions or parameters that would have more completely satisfied the intent of the user and resulted in a more useful response. **\|** In multi-tool scenarios, the model could have sequenced the tool calls more efficiently or didn’t take into account a dependency that made the response not fully satisfy the user intent.                       |
| **Major Issues**   | The code fails to satisfy the user intent and doesn’t generate a useful response. The code involves the incorrect tool, tool functions(s), and/or is missing multiple critical parameters given the prompt & conversation. **\|** In multi-tool scenarios, the model didn’t sequence the tool in the right order and didn’t take into account any dependencies, make the response fail to satisfy the user intent. |
| **Not Applicable** | If no code/tool call is present.                                                                                                                                                                                                                                                                                                                                                                                   |

***

### **Key Things to Remember when Rating Code Quality**

<video src="${PRIVATE_CODE_IMPORTANT_POINTS_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

1\. If the code doesn’t produce any errors, then assume that it’s a valid and available tool for the specific task that you are on. Meaning, don’t expect the model to know about this tool in a different task.
2\. If the code produces an error from using tools/functions/parameters that are not documented, then this is a major issue in tool code quality.
3\. Based on the name of the tools/functions/parameters, if it looks appropriate for the prompt and there are no errors, then it is no issue.

### **Example**

<video src="${PRIVATE_CODE_EXAMPLE_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />