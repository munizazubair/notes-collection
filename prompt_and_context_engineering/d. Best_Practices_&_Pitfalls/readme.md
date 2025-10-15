# **d. Best Practices & Pitfalls**

### **1. Best Practices for Effective Prompts**

### **a. Be Specific and Clear**

**Bad:**

> Write about dogs.
> 

**Good:**

> Write a 300-word informative article about the health benefits of owning a dog, focusing on mental health, physical activity, and social connections. Use a friendly, accessible tone for general readers.
> 

✅ **Tip:** Clear prompts lead to predictable, high-quality outputs.

---

### **b. Use Action Verbs**

Use **explicit, goal-focused verbs** to guide the model clearly.

Examples of powerful verbs:

**Analyze, Compare, Create, Describe, Evaluate, Extract, Generate, List, Rank, Summarize, Translate, Write, Explain, Classify**

---

### **c. Provide Examples When Possible**

Show, don’t just tell — examples help the model learn your intent.

If you want a certain style or tone, **include a short sample** of what the output should look like.

---

### **d. Structure Your Prompts**

Break your prompt into labeled parts for clarity and control.

**Example format:**

```
Task: [What you want done]
Context: [Background information]
Format: [How you want the output structured]
Example: [Sample of desired output]
```

✅ Helps models stay on track and return organized outputs.

---

### **e. Use Positive Instructions Over Negative Ones**

**Better:**

> Write a professional email summarizing the key points from our meeting.
> 

**Avoid:**

> Write an email but don’t make it too long or too informal or too detailed.
> 

✅ Focus on what to *do*, not what *not to do.*

---

### **f. Control Output Format**

Always define how you want the answer presented.

**Example (JSON format):**

```json
{
  "main_idea": "string",
  "supporting_points": ["string", "string"],
  "confidence_level": "high/medium/low"
}
```

✅ Structured formats like JSON, lists, or tables improve consistency.

---

### **g. Use Variables for Reusability**

Design flexible prompt templates that can be reused easily.

**Example:**

```
Role: You are a {expertise} expert.
Task: Analyze the {document_type} and give recommendations for {target_audience}.
Context: This is for a {industry} company with {company_size} employees.
```

✅ Great for automation, coding, or multi-user workflows.

---

### **h. Iterate and Document**

Prompt engineering is experimental — keep testing and refining.

- Track what works best
- Document your most effective prompts
- Test variations to improve accuracy and tone

---

### **2. Common Pitfalls and How to Avoid Them**

| **Pitfall** | **Problem** | **Solution** |
| --- | --- | --- |
| **Ambiguous Instructions** | Vague requests → unpredictable outputs | Be specific and measurable in your request |
| **Contradictory Instructions** | Conflicts confuse the model | Review prompts for internal consistency |
| **Too Many Constraints** | Limits creativity | Use clear positive goals instead of long “don’t” lists |
| **Ignoring Token Limits** | Output gets cut off | Set clear output length or summarize if needed |
| **Not Testing Variations** | First attempt may not be best | Test multiple phrasings, formats, and examples |

---

### **3. Hands-On Examples**

### 🧩 **Example 1 — Content Creation**

**Basic Prompt:**

> Write a social media post about coffee.
> 

**Improved Prompt:**

> Write an engaging Instagram post for a local coffee shop’s new seasonal drink.
> 
> 
> **Context:** Fall launch of Pumpkin Spice Maple Latte
> 
> **Audience:** Coffee lovers aged 25–40
> 
> **Tone:** Warm, inviting, not overly promotional
> 
> **Format:**
> 
> - Main text (max 150 characters)
> - 3–5 relevant hashtags
> - Call to action
> 
> Include sensory details about taste and aroma.
> 

---

### 📊 **Example 2 — Data Analysis**

**Basic Prompt:**

> What do customers think about our product?
> 

**Improved Prompt:**

> Analyze the following customer reviews and provide insights:
> 
> 
> **Reviews:** [paste reviews here]
> 
> Please include:
> 
> 1. Sentiment breakdown (positive/negative/neutral %)
> 2. Top 3 positive aspects
> 3. Top 3 issues or concerns
> 4. Recommendations for improvement
> 5. Confidence level in your analysis
> 
> **Format:** Structured report with clear headings.
> 

---

### 💻 **Example 3 — Code Generation**

**Basic Prompt:**

> Write a function to sort a list.
> 

**Improved Prompt:**

> Write a Python function that:
> 
> - Sorts a list of dictionaries by a specified key
> - Handles missing keys gracefully
> - Supports ascending/descending order
> - Includes proper error handling
> - Has a clear docstring
> 
> **Example usage:**
> 
> ```python
> data = [{"name": "Alice", "age": 30}, {"name": "Bob", "age": 25}]
> result = sort_by_key(data, "age", descending=False)
> ```
> 
> Please include:
> 
> - Function definition with type hints
> - Docstring (parameters + return value)
> - Example usage
> - Brief explanation of the approach

---

**Meaning of Some Words:**

- Pitfalls = things that can go wrong if you’re not careful.
- Ambiguous = unclear or confusing.
- Vague = not detailed enough.
- Contradictory = instructions that disagree with each other.

---
