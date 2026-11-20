---
title: Shortcut — NotesMigrator
permalink: /shortcut/
---

# Get your Apple Notes into NotesMigrator on iPhone and iPad

iOS doesn't let apps read the Notes app directly. The **NotesMigrator: Send All Notes** Shortcut finds your notes and
passes each one to NotesMigrator. Everything stays on your device until you migrate it to your own OneNote account.

[**Add “NotesMigrator: Send All Notes” to Shortcuts**](https://www.icloud.com/shortcuts/f97c4464ea92428eaf6de1c9736a4145)
(NotesMigrator opens this link for you when you tap **Add the Shortcut**.)

## Run it

1. In NotesMigrator, tap **Import My Notes**. Shortcuts opens and runs **NotesMigrator: Send All Notes**.
2. The first time, Shortcuts asks twice: to access Notes and to share them with NotesMigrator. Tap **Always Allow**
   both times.
3. Wait until it finishes (about a second per note). Shortcuts brings you back to NotesMigrator, which shows how many
   notes arrived.

You can also run the Shortcut straight from the Shortcuts app; your notes load the next time you open NotesMigrator.

Running the Shortcut again updates notes that were already sent instead of adding copies.

## Build it yourself

The ready-made Shortcut above is the easiest way. It sends your notes in batches, so it works with any number of
notes. The simple version below works for up to about 500 notes (Shortcuts stops a single search after 30 seconds),
or for one folder at a time.

NotesMigrator must be installed first, so its action appears in Shortcuts.

1. In **Shortcuts**, tap **+** and name the Shortcut **NotesMigrator: Send All Notes**.
2. Add **Find Notes** (leave it on *All Notes*).
3. Add **Repeat with Each**.
4. Inside the repeat, add **Make HTML from Rich Text** and set its input to **Repeat Item**.
5. Still inside the repeat, add **Add Note to NotesMigrator** and set:
   - **Title:** Repeat Item → **Name**
   - **Content:** **HTML from Rich Text**
   - **Folder:** Repeat Item → **Folder**
   - **Creation Date:** Repeat Item → **Creation Date**
   - **Modification Date:** Repeat Item → **Last Modified Date**
6. Tap **Done** and run it.

Locked notes are skipped by the Notes app. To send only some notes, add a filter to **Find Notes** (for example
*Folder is Work*).

## Other ways

You can also import a folder of HTML or Markdown files: in NotesMigrator, tap **Import My Notes**, open **Other ways
to import** and tap **Choose Files**.

Have a Mac? NotesMigrator for Mac reads all your notes directly, including attachments, without a Shortcut.

Questions? See [Support]({{ site.baseurl }}/support/).
