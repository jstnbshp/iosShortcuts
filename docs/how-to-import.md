# 📲 How to Import the Shortcut

Here’s how to get this thing running on your iPhone in under 5 minutes.

---

## 🔧 Prerequisites

- iOS device with the **Shortcuts** app installed  
- A valid **OpenAI API Key**  
- A working **Notion Integration Token** and **Database ID**

---

## 🧭 Step-by-Step

1. **Download this repo**  
   - Either clone it or download as a ZIP.
2. **Open the Shortcut file**  
   - Go to `shortcut/voice-memo-to-notion.shortcut` and tap to open it in Shortcuts.
3. **Grant permissions**  
   - Allow access to Files, Network, and Notion when prompted.
4. **Enter your credentials**  
   - The Shortcut will ask for your:
     - OpenAI API Key
     - Notion Token
     - Notion Database ID
   - Paste them in when prompted. You can also edit the Shortcut later to store them securely.
5. **Run the Shortcut**  
   - Pick a voice memo.
   - Wait for transcription + summary.
   - Check your Notion DB — the new entry should be there.

---

## 🧼 Pro Tips

- If Notion isn’t updating, double-check your database has the right properties: `Title`, `Transcription`, `Summary`, `Date`.
- You can automate trigger phrases with Siri by renaming the Shortcut to something like _"Memo to Notion."_ Try saying it out loud.

