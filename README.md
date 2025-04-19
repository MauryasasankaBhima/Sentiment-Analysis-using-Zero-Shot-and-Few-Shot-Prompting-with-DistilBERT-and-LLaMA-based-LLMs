# Sentiment-Analysis-using-Zero-Shot-and-Few-Shot-Prompting-with-DistilBERT-and-LLaMA-based-LLMs
This project demonstrates the use of **Large Language Models (LLMs)** for performing **sentiment analysis** on textual data using both **zero-shot** and **few-shot prompting**. It explores two powerful models—**DistilBERT** for lightweight transformer-based classification, and **LLaMA** for few-shot conversational-style inference.
---

##  Objective

To perform sentiment classification (positive, neutral, negative) without traditional supervised training using:

- Zero-shot classification (just a task description)
- Few-shot prompting (task + a few labeled examples)

---

##  Tools & Technologies

| Task                         | Tool / Model          |
|------------------------------|------------------------|
| Zero-Shot Classification     | HuggingFace Pipeline (DistilBERT) |
| Few-Shot Prompting           | Open-source LLaMA-style LLM (chat-based) |
| Text Preprocessing           | SpaCy, NLTK           |
| Visualization                | Matplotlib, Seaborn   |
| Notebook Environment         | Jupyter / VS Code     |

---

##  Project Workflow

1. **Input Dataset**  
   - A collection of user reviews or textual feedback (can be scaled or swapped for tweets, comments, etc.)

2. **Zero-Shot Sentiment Classification**  
   - Uses DistilBERT with class labels like: `["positive", "negative", "neutral"]`
   - Doesn’t require any fine-tuning
   - Quick and accurate for many general domains

3. **Few-Shot Prompting with LLaMA (or Chat-like LLM)**  
   - Adds a prompt with 2–3 sample labeled reviews
   - Enhances understanding in context-rich or domain-specific language
   - Great for subjective or nuanced text

4. **Evaluation & Comparison**  
   - Side-by-side predictions from both methods
   - Accuracy check (if ground truth available)
   - Visualization of sentiment distribution

---

##  Key Highlights

-  **No training needed** – leverages the power of pretrained LLMs  
- **Natural language prompts** – easy to scale and adapt  
- **DistilBERT for speed**, **LLaMA for depth**  
- Visual analysis of results  

---

## Sample Prompt for Few-Shot LLaMA

```text
Review: “The delivery was late and the packaging was terrible.”  
Sentiment: Negative  

Review: “Absolutely loved the food and the atmosphere.”  
Sentiment: Positive  

Review: “The product was okay, nothing special.”  
Sentiment: Neutral  

Review: “The staff were friendly, but the food was cold.”  
Sentiment:
