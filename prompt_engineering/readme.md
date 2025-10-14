# **a. Fundamentals**

### 1. What is Prompt Engineering?

- It is the **art and science of crafting instructions** for AI models (like ChatGPT) to produce desired outputs.
- In simple words, it’s *how you ask* the AI to do something.
- **Goal:** ➡️ To **tell the model how to behave and what to produce.**

**Why it matters:**

- You don’t need to be a programmer.
- A well-written prompt gives much better and more accurate results.
- It’s an important skill for productivity and AI-related careers.

---

### 🔹 What is Context Engineering?

- It means **providing relevant facts, documents, or data** that the model uses to give correct and grounded answers.
- In simple words, it’s *what you show* the AI to help it answer correctly.
- **Goal:** ➡️ To **give the model the right information or facts** it should rely on when answering.

---

### 🆚 **Prompt vs. Context Engineering**

| Aspect | Prompt Engineering | Context Engineering |
| --- | --- | --- |
| **Goal** | How to guide the model’s behavior | What info the model should use |
| **Focus** | Wording, structure, examples | Documents, data, tools, memory |
| **Example** | “Be brief. Output JSON.” | “Use info from this PDF.” |
| **Common issue** | Unclear prompt → bad output | Missing data → hallucinations |
| **One-liner** | 🗣️ **How you ask** | 📄 **What you show** |

---

### ⚙️ **How They Work Together**

1. **Start with a good prompt** → The **prompt guides** the model’s behavior.
2. **Add grounding context** → The **context supplies** the knowledge.

➡️ You usually need both together for best results.

---

## **2. Understanding Large Language Models (LLMs)**

### 🔹 What Are LLMs?

- LLMs are **prediction engines** that:
    1. Take your text input (prompt).
    2. Predict the **next most likely word or token**.
    3. Continue predicting to form a complete response.
- They learn patterns from **large datasets** during training.

---

### **3. Common Failure Modes**

1. **Hallucinations:**
    - When the model creates false or imaginary information due to missing or irrelevant context.
2. **Messy Outputs:**
    - Caused by vague or unclear prompts.
3. **Outdated or Inaccurate Info:**
    - When the model isn’t properly grounded with fresh or correct data.

---

### **4. Recommended Workflows**

1. **Start with a clear prompt** (define the task, tone, and structure).
2. **Then ground it with context** (add documents, data, or tools).
3. **In agentic systems:**
    - Feed tool or API outputs back into context for the next step.
4. Always **iterate and test** prompts for best performance.

---

### 5. Key Concept — “Sophisticated Autocomplete”

- LLMs don’t **understand** like humans.
- They **predict** what should come next based on the given input.
- That’s why **your prompt and context** matter so much — they set up the right “autocomplete environment.”

---
