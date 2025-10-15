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

### **2. Understanding Large Language Models (LLMs)**

**🔹 What Are LLMs?**

- LLMs are **prediction engines** that:
    1. Take your text input (prompt).
    2. Predict the **next most likely word or token**.
    3. Continue predicting to form a complete response.
- They learn patterns from **large datasets** during training.

#### - [How LLM Works](#how-llms-work-top-10-executive-level-Questions)

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

## How LLMs Work: Top 10 Executive-Level Questions 

### **1. How does an LLM decide when to stop?**

- LLMs generate **one token at a time**.
- Stopping is controlled by:
    - **End-of-sequence (EOS)** token
    - **Max token limit**
    - **Stop sequences** or **external logic**
- 🧠 The stop decision is made by **both** the model and the system — not by the LLM alone.

---

### **2. Does an LLM update itself when corrected?**

- ❌ **No instant updates.**
- Corrections may improve **future versions**, not the current one.
- Real-time **memory** (like in ChatGPT) remembers personal info, not factual fixes.

---

### **3. How can an LLM “remember” past chats?**

- By default, LLMs **don’t recall** old chats.
- Some use **memory** to store details (name, interests, etc.) and add them to new prompts.
- 🧠 Often powered by **RAG** (Retrieval-Augmented Generation) to include relevant past info.

---

### **4. How can LLMs answer about post-cutoff events?**

- They don’t “know” after their **training cutoff**.
- Some models (like ChatGPT with browsing) use **live web search**.
- Others guess from **older data**, which may be outdated or wrong.

---

### **5. Can LLMs use only uploaded documents?**

- ❌ **No full control.**
- Even with **RAG** or clear prompts, the model may still blend **training knowledge** with your documents.
- You can **prioritize**, but not **limit** it strictly.

---

### **6. Can I trust LLM citations?**

- ❌ **Not always.** LLMs can **hallucinate** or misuse real sources.
- Some tools verify citations, but checks aren’t perfect.
- ✅ Always **verify sources** yourself.

---

### **7. Is RAG still needed with long context windows?**

- ✅ Yes — RAG keeps input **relevant, focused, and cheaper**.
- Long contexts can cause **irrelevant data**, **higher cost**, and **slower responses**.
- RAG improves **accuracy and efficiency**.

---

### **8. Can hallucinations be eliminated?**

- ❌ **No**, but they can be reduced with:
    - **Prompt engineering**
    - **RAG or fine-tuning**
    - **Validation checks**
- 🎯 We can **minimize**, not remove, hallucinations.

---

### **9. How to check LLM answers efficiently?**

- ⚙️ Use a **hybrid approach**:
    - **Humans** → reliable but costly
    - **AI judges** → scalable but imperfect
    - **Automation** → good for structured data (e.g., code, JSON)
- ✅ Best results = **AI + human review**.

---

### **10. Can LLM answers stay identical each time?**

- ❌ Exact repetition isn’t guaranteed.
- You can reduce variation with:
    - **Temperature = 0**
    - **Fixed model version**
    - **Caching past answers**
- Meaning stays same, wording may differ slightly.

---
