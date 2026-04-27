# 💍 AI Wedding Planner — LangChain Agent-Based System

An intelligent, tool-augmented wedding planning assistant that transforms a simple user query into a **structured, actionable wedding plan**—including budget allocation, vendor recommendations, and a complete timeline.

Built using a **LangChain ReAct agent architecture**, this project demonstrates how LLMs can be combined with deterministic tools to create **reliable, semi-real-world decision systems**, not just text generators.

---

## 🚀 What Makes This Project Stand Out

Unlike typical “AI demo apps,” this system is:

* 🧠 **Agent-driven** (not just prompt-based)
* 🛠️ **Tool-augmented** (logic + LLM hybrid)
* 📊 **Deterministic where needed** (budget, timeline)
* 🎯 **Structured output enforced** (not free-form text)
* 🎨 **Product-focused UI** (clean, card-based interface)

---

## 🧩 Core Features

### 💰 Intelligent Budget Allocation

* Rule-based allocation across:

  * Venue
  * Catering
  * Decor
  * Miscellaneous
* Dynamically adjusts based on user priorities (e.g., decor-heavy, food-focused)

---

### 🏢 Vendor Recommendation Engine

* LLM-powered but **strictly controlled output**
* Generates:

  * Venue
  * Catering
  * Decor vendors
* Structured format ensures UI consistency
* Context-aware (city + budget)

---

### 📅 Timeline Generator

* Predefined, optimized wedding planning timeline
* Covers entire lifecycle:

  * Months before → wedding day execution

---

### 🤖 LangChain ReAct Agent

* Uses **tool-based reasoning loop**
* Agent decides:

  * when to allocate budget
  * when to fetch vendors
  * when to generate timeline

Architecture:

```text
User Input
   ↓
LangChain Agent (ReAct)
   ↓
Tools:
   - Budget Allocation (deterministic)
   - Vendor Generator (LLM)
   - Timeline Generator (deterministic)
   ↓
Final Structured Plan
```

---

### 💬 Plan Refinement Loop

* Users can iteratively refine plans:

  * “Reduce budget”
  * “Make decor more luxurious”
* Agent updates while preserving structure

---

### 🎨 Modern UI (Streamlit)

* Clean, wedding-themed interface
* Tab-based navigation:

  * Budget
  * Vendors (card UI)
  * Timeline
* Styled with custom CSS for product-like feel


<img width="941" height="431" alt="image" src="https://github.com/user-attachments/assets/5717a01c-5950-42b9-8291-6677af57b118" />

---

## 🧠 Tech Stack

| Layer    | Technology        |
| -------- | ----------------- |
| LLM      | Groq (LLaMA 3.1)  |
| Agent    | LangChain (ReAct) |
| Backend  | Python            |
| Frontend | Streamlit         |
| Styling  | Custom CSS        |

---

## ⚙️ How It Works

1. **User Input**

   ```
   Plan a wedding in Raipur under 5L with decor focus
   ```

2. **Agent Reasoning**

   * Extracts city, budget, preference
   * Decides tool sequence

3. **Tool Execution**

   * Budget → rule-based logic
   * Vendors → LLM (structured prompt)
   * Timeline → predefined logic

4. **Final Output**

   * Clean, structured plan rendered in UI

---

## 🖥️ Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/your-username/ai-wedding-planner.git
cd ai-wedding-planner
```

---

### 2. Install Dependencies

```
pip install -r requirements.txt
```

---

### 3. Set Environment Variable

#### Windows (PowerShell):

```powershell
$env:GROQ_API_KEY="your_api_key"
```

#### Mac/Linux:

```bash
export GROQ_API_KEY="your_api_key"
```

---

### 4. Run the App

```
streamlit run app.py
```

---

## 📌 Example Output

```
💰 Budget:
Venue: ₹2,00,000
Catering: ₹1,50,000
Decor: ₹1,00,000
Misc: ₹50,000

🏢 Vendors:
[Structured vendor cards]

📅 Timeline:
- 3 months before: Book venue
- 2 months before: Finalize vendors
...
```

---

## 🔮 Future Improvements

* 🔍 Real-time vendor search via APIs (Google Places / Foursquare)
* ⭐ Vendor ranking & scoring system
* 📍 Geo-based filtering
* 💾 Save/export wedding plans
* 🧠 Memory-enabled conversational planning
* 📊 Budget optimization via ML models


---

## ⭐ If you found this interesting

Give it a ⭐ and share!

---
