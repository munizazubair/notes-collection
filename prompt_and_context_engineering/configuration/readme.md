# b. Configuration

### **1. Temperature (0–1 Scale)**

**Definition:**

Controls the **randomness and creativity** of model responses.

**Tip:**

- Temperature **0** → best for accurate, repeatable answers (deterministic)
- Temperature **0.7+** → for open-ended or artistic text.

**Use Case:**

| Range | Behavior | Use Case |
| --- | --- | --- |
| **Low (0–0.3)** | Focused, logical, deterministic (same output every time) | Math, coding, factual Q&A |
| **Medium (0.4–0.7)** | Balanced creativity and consistency | Explanations, essays |
| **High (0.8–1.0)** | Creative, diverse, and imaginative | Storytelling, poetry, brainstorming |

---

### **2. Top-K Sampling**

**Definition:**

Restricts the model’s next-token choice to the **top K most likely tokens**.

*Think:* “How many best word options should the AI look at before choosing?”

**Use Case:**

| Range | Behavior | Use Case |
| --- | --- | --- |
| **Low K (e.g., 20)** | Narrow selection | logical, focused text. |
| **High K (e.g., 40+)** | Broader selection | more creativity. |

---

### **3. Top-P Sampling (Nucleus Sampling)**

**Definition:**

Instead of picking a fixed number of tokens, Top-P chooses from the **smallest set of tokens (the nucleus)** whose **total combined probability (threshold)** equals *P*.

*Think:* “How wide the model’s probability window should be.”

---

**Example:**

For the sentence:

> “The cat is sitting on the ___”
> 

If **Top-P = 0.9** → we keep adding probabilities until the total = **0.9**

✅ {mat, bed, floor, chair} = **nucleus**

The model randomly picks the next word **only from this nucleus**, ignoring the rest.

---

**Key Terms:**

- **Nucleus:** The *core group* of most likely tokens whose total probability equals *P*.
- **Threshold:** The *stopping limit* (e.g., 0.9 means stop when the total probability reaches 90%).

---

**Use Case:**

| Range | Behaviour | Use Cae |
| --- | --- | --- |
| **Low Top-P (0.8–0.9)** | Small nucleus | Focused, logical output |
| **High Top-P (0.95–0.99)** | Wide nucleus | Creative, diverse text |

---

### **4. Output / Token Limits**

**Definition:**

Controls the **maximum length** of the model’s response.

**Use Case:**

| Setting | Behaviour | Use |
| --- | --- | --- |
| **Low token limit** | Short, concise, cheaper outputs. | for summaries or factual Q&A |
| **High token limit** |  Longer, detailed, higher cost. |  for essays, articles, or creative writing |

---

### **5. Recommended Starting Points**

| Mode | Temperature | Top-P | Top-K | Best For |
| --- | --- | --- | --- | --- |
| **Conservative** | 0.1 | 0.9 | 20 | Coding, logic, math |
| **Balanced** | 0.2 | 0.95 | 30 | General writing, explanations |
| **Creative** | 0.9 | 0.99 | 40 | Poetry, brainstorming, storytelling |

---

> Use **low values for factual/consistent tasks** and **higher values for creative or open-ended writing**.

---
