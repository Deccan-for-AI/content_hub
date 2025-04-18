# Rubric 9: **Information Retrieval**

<video src="${PRIVATE_INFORMATION_RETRIEVAL_VIDEO}" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; object-fit: cover;" controls="" controlslist="nodownload nofullscreen" style="width: 100%" />

#### **Intent of Information Retrieval:**

If applicable, how well did the model retrieve the correct information (from documents, files or emails) for the response

### **How should you approach this rubric?**

1. The focus of this rubric are the response and Files, Documents or Emails present in the task.
2. Check if the information present in the response is correctly retrieved from the files, documents or emails. and mark accordingly.
3. If no files, documents or emails are present, mark N/A - Not Applicable.

### Rating Criteria with Examples

The user uploads a **project brief** that says the deadline is *May 10th* and asks: ***“Can you remind me when this project is due?”***

| Category           | Criteria                                                                                        | Examples                                                                                                                                                                                                          |
| ------------------ | ----------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No issues**      | The AI Assistant retrieved the correct information to fulfil the user intent.                   | *“According to the project brief, your deadline is May 10th.”* ✔ **That’s accurate. It pulled the correct date directly from the document.**                                                                      |
| **Minor Issues**   | The AI Assistant didn’t retrieve all the correct information.                                   | If the AI says:*“Your project is due in early May.”* **➖ That’s not wrong, but it’s vague. It didn’t extract the exact detail. ➖ Maybe it skimmed or oversimplified.**                                            |
| **Major Issues**   | The AI Assistant didn’t retrieve any information or all the information retrieved is incorrect. | Now if the AI says:*“Your project deadline is June 5th.”* ❌ **That’s just incorrect. It either misread the file or didn’t reference it at all. ❌ The user asked for a specific answer—and the AI got it wrong.**  |
| **Not Applicable** | If there are no documents, emails or files in the prompt explicitly.                            | If the prompt doesn’t include any files, documents, or emails, this rubric does not apply.                                                                                                                        |