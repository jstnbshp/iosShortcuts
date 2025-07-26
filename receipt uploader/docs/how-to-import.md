# 📲 How to Import the Shortcut

Follow these steps to get the Receipt to Notion Shortcut running on your iPhone.

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
   - Tap `shortcut/ReceiptToNotion.shortcut` to import it into Shortcuts.
3. **Grant permissions**
   - Allow access to Photos, Network, and Notion when prompted.
4. **Enter your credentials**
   - The first run will ask for your:
     - OpenAI API Key
     - Notion Token
     - Notion Database ID
   - You can edit the Shortcut later to store them securely.
5. **Run the Shortcut**
   - Snap or select a photo of a receipt.
   - Wait for the items to appear in your Notion database.

---

## 🧼 Pro Tips

- Ensure your Notion database has the properties listed in the README.
- If parsing fails, tweak the prompt in `src/receipt_parser_prompt.txt`.
