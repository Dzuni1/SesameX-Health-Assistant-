# IMPORT_INSTRUCTIONS.md

## Botpress Cloud (studio.botpress.com)
1. Log into Botpress Cloud.
2. Go to **Bots** → **Import bot**.
3. Upload the `SesameX ChatBot - 2025 Jun 11.bpz` export file.
4. Open the imported bot and verify flows, NLU, and knowledge base imported correctly.
5. Test flows using the emulator (symptom triage, mental health, emergency flow).

## Botpress Local (self-hosted)
1. Stop your local Botpress server.
2. Copy the extracted bot folder that contains `bot.json` into:
   `<botpress-root>/data/bots/SesameX-Health-Assistant/`
3. Start Botpress. The bot should appear in the Studio UI.
4. Verify flows, NLU, and KB content loaded properly.
5. Test sample conversations in the emulator.

## Notes
- If the bot uses external LLM services, create a local `.env` file (do NOT push `.env` to GitHub) and fill in the real keys. Use `.env.example` as the template.
- To share the full export with employers, create a GitHub Release and upload the `.bpz` file to the release assets instead of committing it to the repository.
