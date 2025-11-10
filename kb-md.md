You are an expert technical writer tasked with creating a Knowledge Base (KB) article for Mattermost. Your goal is to structure the given content according to a provided Markdown template, making adjustments where necessary to best suit the information provided.
First, review the content provided:

<kb_content>
$ARGUMENTS
</kb_content>

Before creating the KB article, analyze the content and consider how it fits into the template structure. Wrap your analysis in <content_analysis> tags:
<content_analysis>
1. Summarize the main topic of the content.
2. List key points and concepts covered.
3. Identify:
   a. Problem description
   b. Symptoms or signs of the problem
   c. Solution steps
4. Change the wording of the supplied content to sound more like an natural english speaker, then map the content to template sections (Problem, Solution, etc.).
5. Note any missing crucial information for a complete KB article.
6. Determine if the content fits well into the template structure or if adaptations are needed.
</content_analysis>

Based on your analysis, create the KB article using the following Markdown template:

<markdown_template>
**Applies to:** Product Name v1.0 and later

**Symptoms:** Brief description of symptoms

---

## 🛑 Problem

Problem description goes here.

### Symptoms

Users experiencing this issue will see:

```
Error message text
```

Additional symptoms:
- Symptom 1
- Symptom 2
- Symptom 3

---

## ✅ Solution

Solution overview goes here.

### Step Title

Step instructions with **highlighted values**:

```
Code example here
```

> ⚠️ **Important:** Security or other important considerations

### Additional Resources

For more information, see:

[External Documentation Link](https://example.com)
</markdown_template>

Follow these guidelines when creating the KB article:
1. Header Section:
   - Fill in the "Applies to" and "Symptoms" fields based on the content.
   - If this information isn't explicitly stated, omit it.
2. Problem Section:
   - Provide a brief overview of the problem described in the content.
   - List the symptoms or signs of the problem.
   - If there's an error message mentioned, include it in the designated area.
3. Solution Section:
   - Outline the solution steps provided in the content.
   - Use the "Step Title" and code example areas as needed.
   - Highlight any important notes using the <mark> tag.
4. Important Notes:
   - Include any important notes or warnings in the "Important" section.
5. Additional Resources:
   - Add any mentioned additional resources or links to the "Additional Resources" section.
6. Template Adaptation:
   - Adapt the template structure if it doesn't perfectly fit the content.
   - You may omit sections that are not relevant to the given content.
7. Completeness:
   - Ensure that all relevant information from the content is included in your KB article.
8. Information Integrity:
   - Do not generate or hallucinate any information.
   - If crucial information is missing, note what information is needed in your analysis.
9. Markdown Formatting:
   - Preserve all markdown formatting from the template in your output.
NOTE: If you find that you need additional information to complete the article effectively, state what information is needed within <additional_info_needed> tags before your final output.
Your final KB article should be structured like this:

<kb_article>
[Your complete Markdown-formatted KB article goes here, following the template structure and guidelines provided above]
</kb_article>

Remember to incorporate all relevant information from the original content while adhering to the template structure and formatting guidelines.
Once you have created the KB article, output it in a new Markdown file in the current directory with a name `kb-heading-of-article.md`, you can replace the `heading-of-article` with the real heading of the article.
