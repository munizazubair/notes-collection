# **a. Fundamentals**

### **1. What is Prompt Engineering?**

- The **art and science of crafting instructions** for AI models (like ChatGPT) to produce the desired output.
- In simple words, it’s *how you ask* the AI to do something.
- **Goal:** ➡️ To **tell the model how to behave and what to produce.**

**Why it matters:**

- You don’t need to be a programmer.
- A well-written prompt gives better, clearer, and more accurate results.
- It’s a key skill for **productivity, communication, and AI-related careers.**

---

### 🔹 **What is Context Engineering?**

- It means **providing relevant facts, data, or documents** that the model uses to answer correctly.
- In simple words, it’s *what you show* the AI to help it respond accurately.
- **Goal:** ➡️ To **supply the model with the right information** it should rely on when generating responses.

---

### 🆚 **Prompt vs. Context Engineering**

| Aspect | Prompt Engineering | Context Engineering |
| --- | --- | --- |
| **Goal** | Guide model behavior | Supply correct information |
| **Focus** | Wording, tone, examples | Data, documents, memory, tools |
| **Example** | “Be brief. Output JSON.” | “Use info from this PDF.” |
| **Common issue** | Unclear prompt → poor output | Missing data → hallucinations |
| **One-liner** | 🗣️ **How you ask** | 📄 **What you show** |

---

### ⚙️ **How They Work Together**

1. **Start with a strong prompt** → guides *how* the model responds.
2. **Add grounding context** → provides *what* the model should use.
3. Together, they make the response both **accurate and relevant.**

➡️ You usually need **both** for best results.

---

### **2. Understanding Large Language Models (LLMs)**

**🔹 What Are LLMs?**

- LLMs are **prediction engines** that:
    1. Take your text input (*prompt*).
    2. Predict the **next most likely token (word or symbol)**.
    3. Continue predicting until the response is complete.
- They learn these patterns from **large amounts of text data** during training.

#### - [How LLM Works](#how-llms-work-top-10-executive-level-Questions)

---

### **3. Common Failure Modes**

1. **Hallucinations** → False or imaginary info due to weak or missing context.
2. **Messy Outputs** → Caused by vague or poorly structured prompts.
3. **Outdated Info** → When the model isn’t grounded with up-to-date context or data.

---

### **4. Recommended Workflow**

1. **Start with a clear prompt** — define task, tone, and format.
2. **Add grounding context** — include data, documents, or background.
3. **In agentic systems:** feed tool or API results back into the context for the next step.
4. **Iterate and test** — refining prompts gives better results.

---

### **5. Key Concept — “Sophisticated Autocomplete”**

- LLMs don’t *understand* like humans — they *predict* what should come next.
- The quality of their prediction depends on the **prompt and context** you provide.
- So, prompting isn’t just asking — it’s *setting up the right environment* for accurate prediction.

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
