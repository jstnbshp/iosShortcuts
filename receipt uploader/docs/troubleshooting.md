# 🚑 Troubleshooting

If the Shortcut isn’t working as expected, try these tips:

1. **Credentials** – double‑check your API keys and tokens in the Shortcut.
2. **Network Access** – the Shortcut needs internet for GPT and Notion.
3. **Database Schema** – your Notion DB should contain Date, Vendor, Item, Quantity, Cost Per Item, Total Cost, Category, and Notes.
4. **Prompt Tweaks** – edit `src/receipt_parser_prompt.txt` if line items aren’t parsed correctly.

If issues persist, remove and re-import the Shortcut.
