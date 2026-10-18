# GODRAM Daily Word

An installable app (PWA) of KJV scriptures and Christian quotes from GODRAM TV.

**Live app:** https://godram-tv.github.io/daily-word/

```

WHAT'S IN THIS FOLDER
  index.html             The widget itself
  content.json           The 500 verses and quotes (edit this to change content)
  manifest.webmanifest   Tells phones and PCs this is an installable app
  sw.js                  Makes it work offline
  icons/                 App icons made from the GODRAM logo

PUT IT ONLINE (free, about 10 minutes) - GitHub Pages
  1. Create a free account at github.com.
  2. Click "New repository". Name it  daily-word  and set it to Public.
  3. Click "uploading an existing file", then drag in EVERYTHING from this
     folder (including the icons folder). Click "Commit changes".
  4. Go to Settings > Pages. Under "Branch" choose  main  and  / (root),
     then Save.
  5. After a minute or two your app is live at:
        https://YOUR-USERNAME.github.io/daily-word/
  (Netlify Drop at app.netlify.com/drop also works: drag the folder in.)

INSTALL IT
  Android (Chrome):  open the link > menu (3 dots) > "Add to Home screen"
                     or "Install app".
  iPhone (Safari):   open the link > Share button > "Add to Home Screen".
  PC (Chrome/Edge):  open the link > click the Install icon in the address
                     bar, or use the "Install" button in the widget.
                     It then opens in its own small window, like a program.

UPDATE THE VERSES LATER
  Edit content.json on GitHub (pencil icon) and save. Installed copies pick
  up the new list the next time they open with internet.
  Each entry looks like this:
    {"id": 501, "type": "verse", "topic": "Hope",
     "text": "...", "ref": "Psalm 27:13 (KJV)"}
  type is "verse" or "quote". Keep the commas between entries.

  The Rainmeter desktop skin and the Android widget will read this same
  content.json link, so one edit updates everything.

TEST IT ON YOUR PC WITHOUT HOSTING
  Opening index.html by double-clicking won't load the verses (browsers
  block that). Instead, in this folder run:   python -m http.server
  then visit  http://localhost:8000
```
