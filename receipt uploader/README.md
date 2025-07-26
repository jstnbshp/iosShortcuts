# 🧾 Receipt Parser to Notion

This Shortcut lets you snap a photo of a receipt, parses the text with GPT‑4, and logs each line item to a Notion database. It is a lightweight way to track purchases without typing everything by hand.

---

## 🚀 What It Does

1. **Capture or select** a receipt image.
2. **Extract text** using iOS OCR.
3. **Parse** the text into structured items via GPT‑4.
4. **Insert** each item into your Notion database with date, vendor, quantity, and costs.

---

## 🧰 What You Need

- ✅ [OpenAI API Key](https://platform.openai.com/account/api-keys)
- ✅ [Notion Integration Token](https://www.notion.so/my-integrations)
- ✅ A Notion database with the fields listed below
- ✅ iOS Shortcuts app
- ✅ This repo cloned or downloaded with the `.shortcut` file

---

## 🧪 Notion Database Schema

Your database should contain these properties:

| Name            | Type  |
|-----------------|-------|
| `Date`          | Date  |
| `Vendor`        | Text  |
| `Item`          | Text  |
| `Quantity`      | Number|
| `Cost Per Item` | Number|
| `Total Cost`    | Number|
| `Category`      | Text or Select|
| `Notes`         | Text  |

Copy your **Database ID** so you can paste it into the Shortcut when prompted.

---

## 🔐 How Secrets Work

The Shortcut will ask for your OpenAI key, Notion token, and database ID the first time you run it. They are stored locally inside the Shortcut and used for the API calls.

---

## 🛠 Setup Instructions

1. **Clone or download** this repo.
2. **Open** `shortcut/ReceiptToNotion.shortcut` on your iOS device.
3. Import it into the Shortcuts app and grant the required permissions.
4. Run the Shortcut and enter your credentials when prompted.
5. Take a picture of a receipt and watch the items appear in Notion.

---

## 📂 Files in This Repo

```
receipt-parser-to-notion/
├── shortcut/
│   └── ReceiptToNotion.shortcut
├── src/
│   └── receipt_parser_prompt.txt
├── docs/
│   ├── architecture.md
│   ├── how-to-import.md
│   └── troubleshooting.md
├── examples/
│   ├── sample_ocr_text.txt
│   └── sample_notation_payload.json
├── .gitignore
├── LICENSE
└── README.md
```

---

## 📸 Example Output

```json
[
  {
    "Date": "2025-07-26",
    "Vendor": "Corner Market",
    "Item": "Bananas",
    "Quantity": 2,
    "Cost Per Item": 0.50,
    "Total Cost": 1.00,
    "Category": "Groceries",
    "Notes": ""
  }
]
```

---

## 💬 Why I Built This

Receipts pile up fast, and manually entering them is tedious. This Shortcut automates the process so everything lands in Notion where it’s searchable and organized.

---

## ⚖ License

MIT — use it, tweak it, and let me know if you build something cool.
