# **c. Prompting Techniques**

Prompting techniques are methods used to **guide and control AI responses**.

They are divided into **Basic** and **Advanced** types.

---

## **Basic Prompting Techniques**

### **1. Zero-Shot Prompting**

**What:** Ask directly **without examples** — model uses its own knowledge.

**Example:**

> Classify this review as positive, negative, or neutral: “The film was visually stunning but the plot felt rushed.”
> 
> 
> **Use for:** Simple, factual tasks.
> 
> 🧠 **Tip:** Be clear and specific.
> 

---

### **2. One-Shot Prompting**

**What:** Give **one example** to show the pattern or format.

**Example:**

> Translate English to French:
> 
> 
> English: "Hello, how are you?" → French: "Bonjour, comment allez-vous?"
> 
> English: "Where is the library?" → French:
> 
> **Use for:** Formatting or translation tasks.
> 
> 🧠 **Tip:** One example guides the style.
> 

---

### **3. Few-Shot Prompting**

**What:** Give **3–5 examples** to teach structure or logic.

**Example:**

> Feedback: "Great service, but food was cold" → JSON: {"service":"positive","food":"negative","overall":"mixed"}
> 
> 
> **Use for:** Pattern recognition, classification, structured output.
> 
> 🧠 **Tip:** *Few-shot = teach by example.*
> 

---

### **4. Role Prompting**

**What:** Assign a **role/persona** to shape tone/expertise.

**Example:**

> Act as an experienced software architect and suggest scalable app design ideas.
> 
> 
> **Use for:** Expert or tone-based responses.
> 
> 🧠 **Tip:** Start with **“Act as a…”** to define the role.
> 

---

### **5. System Prompting**

**What:** Defines the model’s **overall behavior or personality** for the session.

**Example:**

> You are a helpful tutor who explains technical topics simply and encouragingly.
> 
> 
> **Use for:** Consistent tone and style across a session.
> 
> 🧠 **Tip:** Use at session start to maintain control.
> 

---

### **6. Contextual Prompting**

**What:** Provide **background or audience info** to guide the response.

**Example:**

> Context: Writing for beginners. Explain what an API is in simple words.
> 
> 
> **Use for:** Audience-specific or contextual writing.
> 
> 🧠 **Tip:** State the **context first**, then the task.
> 

---

## **Advanced Prompting Techniques**

### 1. Chain of Thought (CoT)

- **What:** Make the model **think step-by-step**.
- **Use for:** Math, logic, multi-step tasks.
- **Prompt:** “Let’s think step by step.”
- **Tip:** Use **temperature = 0** for consistent reasoning.

---

### 2. Self-Consistency

- **What:** Generate multiple independent reasoning traces and **pick the most common final answer**.
- **Use for:** Improve reliability in reasoning tasks.
- **Tip:** Medium temp (0.3–0.7); run 3–5 tries and choose the majority answer.

---

### 3. Step-Back Prompting

- **What:** Ask a **general question first**, then the **specific** one.
- **Use for:** Design, analysis, optimization.
- **Example:**
    1. “What are the key factors of good UI design?”
    2. “Now use them to improve this app.”

---

### 4. ReAct (Reasoning + Acting)

- **What:** Interleave **Thoughts** (reasoning) with **Actions** (tool use) and **Observations**.
- **Use for:** Tasks needing external data or tools.
- **Pattern:** Question → Thought → Action → Observation → Thought → Final Answer.
- **Who does it:** **The LLM** performs the loop (human provides the task).
    
    **Example flow:**
    
1. Human: “What’s the current population of Pakistan?”
2. LLM Thought → Action: search → Observation (result) → Thought → Final Answer.

---

### 5. Tree of Thoughts (ToT)

- **What:** Generate multiple reasoning branches, evaluate/prune them, then synthesize the best.
- **Use for:** Strategic planning, creative problem solving.
- **Tip:** Use higher temp for generation, lower temp for evaluation.

---

### Common Pitfall

- **Long chains** can hallucinate; unbounded branching is costly; consensus can reinforce a wrong premise — validate assumptions.

---
