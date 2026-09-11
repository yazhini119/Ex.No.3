# Ex.No.3-Explaing the following Prompt Engineering types with examples - Straightforward Prompts - Tabular Format Prompting - Missing Word Prompting - Preceding Question Prompting.

### DATE: 08-09-2026  
### NAME: Yazhini S
### REGISTER NUMBER : 212223050062

# Aim: 
 To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. Using Straightforward Prompts - Tabular Format Prompting - Missing Word Prompting - Preceding Question Prompting techniques.


# Prompt Engineering Techniques for Chatbots

Prompt Engineering is the process of **crafting effective instructions** to guide an AI system toward producing accurate, helpful, and context-aware responses.

A **well-crafted prompt** can help a chatbot:

* Provide relevant answers to user queries.
* Maintain the desired tone (formal, friendly, empathetic).
* Handle different types of customer issues efficiently.
* Avoid misunderstandings by asking clarifying questions.

Different **prompting methods** can be applied depending on the complexity of the query and the detail required.

---

## Types of Prompt Engineering

### 1. Straightforward Prompts

**Definition:**
Direct and simple instructions given to the AI without extra context. Best for **deterministic, repetitive tasks** where the output format is fixed.

**Key Features:**

* Clear and direct phrasing.
* Minimal ambiguity.
* Works well for factual or standard replies.

**Use Cases:**

* Order tracking responses.
* Providing product availability.
* Greeting/closing messages.

**Example:**

```plaintext
Prompt: "When a customer asks for order status, reply with:  
'Your order is currently being processed and will be delivered by [date].'"
```

**Conversation:**

* Customer: *"What’s the status of order #1456?"*
* Chatbot: *"Your order is currently being processed and will be delivered by September 15, 2025."*

**Advantages:** Fast and reliable for structured queries.
**Limitations:** Lacks flexibility, may fail for vague queries.

---

### 2. Tabular Format Prompting

**Definition:**
Organizes information into a **structured table** for consistent responses.

**Key Features:**

* Easy mapping between **Issue → Solution → Tone**.
* Ensures consistency.
* Best when multiple query categories exist.

**Use Cases:**

* Troubleshooting guides.
* Policy summaries (refunds, returns, replacements).
* Tone-based responses.

**Example Prompt:**

| Issue Type           | Steps                         | Tone       |
| -------------------- | ----------------------------- | ---------- |
| Order Tracking       | Provide ETA + tracking number | Reassuring |
| Product Troubleshoot | Suggest fixes, then escalate  | Helpful    |
| Refund/Return        | Explain policy + return steps | Empathetic |

**Conversation:**

* Customer: *"My package hasn’t arrived yet."*
* Chatbot: *"I understand your concern. Your order is still in transit and is expected to arrive by September 14, 2025. Tracking number: TR123456."*

**Advantages:** Easy scalability & consistency.
**Limitations:** May feel robotic if overused.

---

### 3. Missing Word Prompting (Cloze Prompting)

**Definition:**
AI fills in **blanks in a template**, ensuring structured responses.

**Key Features:**

* Template-driven replies.
* Guarantees inclusion of required fields (name, ID, date).
* Reduces formatting errors.

**Use Cases:**

* Personalized responses.
* Order updates with placeholders.
* FAQs with uniform style.

**Example Prompt:**

```plaintext
"Fill in the blanks in this template:  
Hello [name], your order [order_id] is currently [status]. Expected delivery: [date]."
```

**Conversation:**

* Customer: *"Hi, I’m Arjun. My order 5678 hasn’t been delivered yet."*
* Chatbot: *"Hello Arjun, your order 5678 is currently delayed in transit. Expected delivery: September 16, 2025."*

**Advantages:** Highly structured & accurate.
**Limitations:** Rigid, may not handle free-flow conversations well.

---

### 4. Preceding Question Prompting

**Definition:**
The AI **first asks clarifying questions** when the query lacks details.

**Key Features:**

* Adds a confirmation step.
* Improves accuracy & trust.
* Reduces wrong replies.

**Use Cases:**

* Refund requests without order ID.
* Troubleshooting without device details.
* Subscription/account issues.

**Example:**

```plaintext
Prompt: "If customer’s query is missing details (like order ID), ask a clarifying question first."
```

**Conversation:**

* Customer: *"I need a refund."*
* Chatbot: *"I can help with that! Could you please share your order number so I can check the refund details?"*

**Advantages:** Prevents errors, builds trust.
**Limitations:** Adds extra steps (slightly longer conversation).

---

### 5. Few-Shot Prompting

**Definition:**
AI is provided with a **few examples (input → output pairs)** to learn a style or reasoning pattern.

**Key Features:**

* Learns through examples.
* Handles varied queries consistently.
* Best when strict rules don’t exist.

**Use Cases:**

* Technical troubleshooting.
* Domain-specific FAQs.
* Customer query handling with nuance.

**Example Prompt:**

```plaintext
Here are some examples:  


Customer: "My phone isn’t charging."  
Chatbot: "Please try using a different cable or adapter. If it still doesn’t work, it may need servicing."  


Customer: "The screen keeps flickering."  
Chatbot: "That seems like a display issue. Restart your device and check again."  


Now respond to:  
Customer: "My app keeps crashing."
```

**Expected Output:**

* Chatbot: *"It looks like the app might have a bug. Please try clearing the cache or reinstalling the app. If the problem continues, let me know and I’ll help further."*

**Advantages:** Flexible & adaptive.
**Limitations:** Needs well-chosen examples; too many can confuse the AI.

---

## Best Practices for Prompt Engineering

* Keep prompts **clear, concise, and unambiguous**.
* Use **structured formats (tables, templates)** where consistency is needed.
* Apply **preceding questions** for vague or incomplete queries.
* Provide **examples (few-shot)** to teach style/pattern.
* Always test prompts with **edge cases** (e.g., missing data, typos).

---
## Conclusion

Implementing diverse prompt engineering techniques empowers chatbots to deliver accurate, context-aware, and user-friendly interactions. Straightforward prompts ensure fast, reliable responses for routine queries, while tabular format prompts provide consistency and structure across multiple scenarios. Missing word (cloze) prompts enable precise personalization, and preceding question prompts enhance clarity by addressing incomplete inputs. Each approach has unique advantages, and strategically combining them maximizes efficiency, accuracy, and customer satisfaction. Thoughtful prompt design not only improves response quality but also fosters trust, scalability, and adaptability, positioning chatbots as effective, reliable, and intelligent tools in modern customer service ecosystems.

Key Takeaways:

1.Enhances accuracy, consistency, and personalization in responses.

2.Builds user trust by clarifying incomplete or ambiguous queries.

3.Supports scalability and adaptability in customer service operations.

## Result

By applying **Straightforward, Tabular, Missing Word, Preceding Question, and Few-Shot Prompting**, customer service chatbots can:

1) Deliver accurate answers.
2) Maintain a natural conversational flow.
3) Improve customer trust and satisfaction.

Each method has its **strengths and trade-offs**, and the right combination depends on the **type of query** and **business goals**.

---


