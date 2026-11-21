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

NEW IN vw-v5 (app version v5)
- New bottom tab "Verbs": 250 everyday verbs for Dutch and for English (a hand-picked mix of the most useful ones, not a strict frequency list).
  Each row shows the meaning and the main forms (Dutch: infinitive, simple past, perfect with hebben/zijn; English: past, participle).
- Tap a verb to see all tenses. Dutch: present, simple past, present perfect, past perfect, future, conditional, imperative.
  English: present simple, present continuous, past simple, present perfect, past perfect, future.
  The AI writes the table the first time; it is then stored on the device, so reopening is instant and free. "Regenerate" asks again.
- "Add to my words" saves a verb as a normal card. "Add the next 10 to my words" saves ten unsaved verbs at once.
- Saved verbs show a "Show tenses" button on their card and on the flashcard back.
- The list itself works offline. Only the first look at a verb's tenses needs the internet and your API key.

NEW IN vw-v6 (app version v6)
- Quiz > Verbs: practice for the 250 verbs. Questions: simple past, past participle, heeft or is (Dutch), and fill-in-the-blank sentences.
  Choose Forms (works offline), Sentences, or Both, and All verbs, Irregular only, or Saved only.
- Sentence questions: the AI writes them the first time (one request for up to 10 verbs), then they are kept on this device.
- A saved verb you miss becomes due again in your flashcards.

--- v7: easier adding ---
Add tab: type a word and press Add. It is looked up and saved in the background,
so you can type the next one straight away. "Look up first" shows the full card
before saving, like before. Failed items show Retry; waiting items survive a reload.

Batch adding: one line per word, columns separated by | (or tab, or ;):
  word | where I saw it | my own sentence | nl or en
Only the word is required. Leave the language out to use the selected one.
Copy template / Download template give you a ready-to-fill list (the download is
a CSV that opens in Excel or Sheets). Load a file accepts .csv, .tsv and .txt.
You can also paste straight from a spreadsheet.
