# **b. Configuration**

### **1. Temperature (0–1 Scale)**

**Definition:**

Controls the **randomness and creativity** of model responses.

**Tip:**

- **0** → Accurate, repeatable answers (deterministic)
- **0.7+** → More open-ended or artistic responses

**Use Case:**

| Range | Behavior | Use Case |
| --- | --- | --- |
| **Low (0–0.3)** | Focused, logical, deterministic (same every time) | Math, coding, factual Q&A |
| **Medium (0.4–0.7)** | Balanced creativity and consistency | Explanations, essays |
| **High (0.8–1.0)** | Creative, diverse, imaginative | Storytelling, poetry, brainstorming |

---

### **2. Top-K Sampling**

**Definition:**

Restricts the model’s next-token choice to the **top K most likely tokens**.

*Think:* “How many best word options should the AI consider before choosing?”

**Use Case:**

| Range | Behavior | Use Case |
| --- | --- | --- |
| **Low K (e.g., 20)** | Narrow selection | Logical, focused text |
| **High K (e.g., 40+)** | Broader selection | More variety and creativity |

🧠 **Tip:** Often used with Top-P — Top-K limits randomness first, then Top-P filters by probability.

---

### **3. Top-P Sampling (Nucleus Sampling)**

**Definition:**

Instead of using a fixed number of tokens (like Top-K), Top-P chooses from the **smallest set of tokens (the nucleus)** whose **total combined probability** equals *P*.

*Think:* “How wide the model’s probability window should be.”

---

**Example:**

> “The cat is sitting on the ___”
> 

| Word | Probability |
| --- | --- |
| mat | 0.40 |
| bed | 0.25 |
| floor | 0.15 |
| chair | 0.10 |
| roof | 0.05 |
| table | 0.03 |
| car | 0.02 |

If **Top-P = 0.9**, we keep adding probabilities until total = **0.9**

✅ {mat, bed, floor, chair} = **nucleus**

The model randomly picks the next word **only from this nucleus**, ignoring the rest.

---

**Key Terms:**

- **Nucleus:** The *core group* of tokens whose total probability equals *P*
- **Threshold:** The *stopping limit* (e.g., 0.9 = stop when total probability reaches 90%)

---

**Use Case:**

| Range | Behavior | Use Case |
| --- | --- | --- |
| **Low Top-P (0.8–0.9)** | Small nucleus | Focused, logical output |
| **High Top-P (0.95–0.99)** | Wide nucleus | Creative, diverse text |

---

### **4. Output / Token Limits**

**Definition:**

Controls the **maximum length** of the model’s response.

Higher limits increase detail — and cost.

**Use Case:**

| Setting | Behavior | Use Case |
| --- | --- | --- |
| **Low token limit** | Short, concise, cheaper outputs | Summaries, factual Q&A |
| **High token limit** | Longer, detailed, higher cost | Essays, articles, creative writing |

---

### **5. Recommended Starting Points**

| Mode | Temperature | Top-P | Top-K | Best For |
| --- | --- | --- | --- | --- |
| **Conservative** | 0.1 | 0.9 | 20 | Coding, logic, math |
| **Balanced** | 0.2 | 0.95 | 30 | General writing, explanations |
| **Creative** | 0.9 | 0.99 | 40 | Poetry, brainstorming, storytelling |

---

> ✅ Use low values for factual or consistent tasks, and higher values for creative or open-ended writing.
> 

---
