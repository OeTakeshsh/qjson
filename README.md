# qjson

Compact JSON format to convert text into structured knowledge (Q/A + relations + dependencies).

---

## 📦 Structure

```
.
├── examples/
│   ├── mixed_topics.json
│   └── philosophy_basics.json
├── prompt.json
├── qjson.prompt.json
├── schema.json
└── README.md
```

---

## 🧠 What each file does

* **schema.json** → defines the format structure
* **prompt.json** → human-readable prompt
* **qjson.prompt.json** → compact version (for direct LLM use)
* **examples/** → real format examples

---

## ⚙️ Usage

1. Take text (chat, notes, docs)
2. Apply the prompt (`qjson.prompt.json`)
3. Get structured JSON

---

## 🧩 Format (overview)

```json
{
  "summary": "...",
  "topics": [
    {
      "subject": "...",
      "q": "...",
      "a": "...",
      "k": ["..."],
      "ex": "...",
      "rel": ["..."],
      "deps": ["..."]
    }
  ],
  "meta": {
    "coverage": 0-1,
    "depth": 0-1
  }
}
```

---

## 🧠 Use cases

* studying (flashcards)
* knowledge organization
* input for AI systems

👉 not limited to programming

---

## 🧾 TL;DR

Text → qjson → reusable knowledge

