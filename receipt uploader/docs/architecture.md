# 🧱 Shortcut Architecture: Receipt to Notion

This document outlines how the Receipt to Notion Shortcut works.

## 🔄 Data Flow

1. **Capture or Upload Photo**
   - The Shortcut lets you take a new photo or choose one from your library.
   - OCR is performed on the image using the built‑in "Get Text from Image" action.

2. **Receipt Parsing**
   - The recognized text is sent to GPT-4 with the prompt in `src/receipt_parser_prompt.txt`.
   - GPT returns a JSON array of line items with date, vendor, quantity, costs, and more.

3. **Notion Insertion**
   - Each line item is sent to the Notion API to create a row in your database.
   - The Notion token and database ID are stored inside the Shortcut.

## 🛡️ Credentials

- **OpenAI API Key** – used for the GPT call.
- **Notion Integration Token** – for authentication with Notion.
- **Notion Database ID** – identifies where rows should be created.

All secrets stay on your device within the Shortcut.

## 🌐 APIs Used

- [OpenAI GPT-4](https://platform.openai.com/docs/guides/text-generation)
- [Notion API](https://developers.notion.com/reference/post-page)
