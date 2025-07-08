# Contract Review Agent 🧠📑

An intelligent LLM-powered agent that reads legal contracts and highlights potential issues, risky clauses, and missing standard terms. Built to help startups and legal teams catch red flags early.

---

## 🔍 Features

- 🧾 Upload PDF or Word (.docx) contract files
- 🧠 AI agent reads and extracts all clauses
- ⚠️ Highlights vague, ambiguous, or missing clauses
- ✍️ Suggests improved clause wording
- 📊 Generates structured report with risk ratings

---

## 🛠️ Tech Stack

- Python 3.10+
- LangChain + OpenAI GPT-4
- PyPDF / python-docx
- Streamlit or Gradio
- (Optional) JSON schema output

---

## 📦 Installation

```bash
git clone https://github.com/HiraWaheed/contract-review-agent.git
cd contract-review-agent
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
````

---

## 🔑 Setup

Create a `.env` file:

```env
OPENAI_API_KEY=your_openai_key
```

---

## 🚀 Usage

Start the app with:

```bash
streamlit run app.py
```

Upload your contract PDF or DOCX to begin the review.

---

## 🧠 Agent Behavior

1. Breaks down the document into clauses
2. Classifies each clause by type (NDA, payment, indemnity, etc.)
3. Flags problematic clauses:

   * Missing terms
   * Unclear obligations
   * Biased language
4. Provides rewritten suggestions (optional)

---

## 🖼️ Example Output

```
Clause: "The client may terminate the agreement at any time..."
⚠️ Risk: Unilateral termination clause favors only one party.
💡 Suggestion: Add mutual termination conditions with notice period.

Clause: Missing confidentiality clause
⚠️ Risk: Confidentiality not addressed
💡 Suggestion: Add standard NDA clause here
```

---

## 🔧 Improvements (Future)

* Add multiple jurisdiction support (US, EU, etc.)
* Export reviewed contracts with highlights
* Integrate with Notion / Slack for team feedback

