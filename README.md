Vivid Words (standalone)
========================

Files: index.html, manifest.webmanifest, sw.js, icon-180.png, icon-192.png, icon-512.png
Upload ALL of them together, in the same folder, to any static web host.

First run
---------
1. Open the page. Tap the sliders icon (top right) > paste your Anthropic API key > Save key > Test key.
2. Tap "Hear Dutch" / "Hear English" to check the phone voices.
3. Add the page to your Home Screen (iPhone: Safari Share > Add to Home Screen. Android: Chrome menu > Install app).

Important
---------
- Your words and your API key are stored in the browser on that device only, tied to the page's address.
  Always open the app from the same address. A new address starts with an empty library.
- On iPhone the Home Screen app has its own storage, separate from Safari. Install it first,
  then enter the key and import your words inside the installed app.
- Export a backup now and then (Words tab, bottom: "Move your words").
- When you upload a new index.html, change VERSION in sw.js (for example "vw-v2") so phones pick up the update.
- In the Anthropic Console, set a monthly spend limit for the key.

NEW IN THIS VERSION (vw-v2)
- My own sentence: on any saved word (Words tab, flashcard back) write a sentence you could really say.
  "Check my sentence" asks the AI whether it sounds natural (articles, prepositions, word order). Saved automatically.
- Flashcards > Speak mode: you see the meaning, say a sentence with the word OUT LOUD, optionally record yourself,
  then reveal the word and compare with the phone voice. Recordings are not stored; they are only for comparing right now.
  The first time, your phone asks for microphone permission. Allow it.
- Quiz > Type it: type the missing word in an example sentence (or in your own sentences). Mixed mode combines everything.
- If you are updating an existing install: upload the new files over the old ones. Close and reopen the app once or twice
  so the new version loads (the service worker cache is now vw-v2). Your words stay.
