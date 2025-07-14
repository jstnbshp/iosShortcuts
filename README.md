# 📱 Voice Memo to Notion (with Whisper + GPT)

Welcome to my automation setup — this Shortcut takes a **voice memo**, runs it through **OpenAI Whisper** for transcription, **GPT-4** for summarization, and drops it into a Notion database called "Memos".

It’s simple, fast, and built for real-world use. No gimmicks. Just a streamlined capture pipeline for thoughts, journal entries, meeting notes, rants, or whatever else ends up in your voice memos.

---

## 🚀 What It Does

1. Lets you **choose a voice memo file** (manually or from the share sheet).
2. **Transcribes** the audio using Whisper via OpenAI's API.
3. **Summarizes** the content using GPT-4.
4. **Uploads** it to your Notion database with fields for title, transcription, summary, and date.

---

## 🧰 What You Need

- ✅ [OpenAI API Key](https://platform.openai.com/account/api-keys)
- ✅ [Notion Integration Token](https://www.notion.so/my-integrations)
- ✅ A Notion database ready to accept new rows (with proper fields)
- ✅ iOS Shortcuts app installed (obviously)
- ✅ This repo cloned or downloaded with the `.shortcut` file

---

## 🧪 Notion Database Schema

Your Notion database should have these properties:

| Name         | Type     |
|--------------|----------|
| `Title`      | Title    |
| `Transcription` | Text   |
| `Summary`    | Text     |
| `Date`       | Date     |

You’ll need to copy your **Database ID** and paste it into the Shortcut when prompted.

---

## 🔐 How Secrets Work

You’ll be prompted to enter your:
- OpenAI API key
- Notion token
- Database ID

💡 These are stored locally on your device inside the Shortcut’s fields. Nothing leaves your phone except the API calls.

---

## 🛠 Setup Instructions

1. **Clone or download** this repo.
2. **Open the `.shortcut` file** from the `shortcut/` folder.
3. iOS will prompt you to import it into the Shortcuts app.
4. When running it for the first time:
   - Select a voice memo file.
   - Enter your credentials (API Key, Notion Token, DB ID).
5. Test it — you should see a new entry in Notion.

---

## 📂 Files in This Repo

```
iosShortcuts/
├── shortcut/
│   └── voice-memo-to-notion.shortcut
├── docs/
│   ├── architecture.md
│   ├── how-to-import.md
│   └── troubleshooting.md
├── examples/
│   └── sample-output.json
├── .gitignore
├── LICENSE
└── README.md
```

---

## 📸 Example Output (Notion Entry)

```json
{
  "Title": "Dog Training Notes",
  "Transcription": "Okay, Clover was barking when the mailman came...",
  "Summary": "Notes about improving Clover’s reaction to door sounds and strangers.",
  "Date": "2025-07-14T10:00:00-07:00"
}
```

---

## 💬 Why I Built This

Because voice memos are the rawest form of thought capture, and Notion is where I want those thoughts to go — organized, searchable, and summarized. No more forgetting ideas that were spoken into the void. This Shortcut catches them midair and files them away like magic.

---

## 🧠 Future Ideas

* Auto-tag entries by content type (`#journal`, `#meeting`, `#idea`)
* Optional sentiment analysis or mood scoring
* Custom reminders triggered from entries
* Routing different audio types to different Notion DBs

---

## ⚖ License

MIT — use, remix, improve. If you end up building something rad with it, drop me a line.

