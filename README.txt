ATA QUEST - PROGRESSIVE WEB APP FILES
=====================================

Upload ALL of these to the same folder in your GitHub repository,
right where your current game file lives:

  index.html              (the game - replaces your current file)
  manifest.json           (app name, icons, colors)
  sw.js                   (service worker - offline play)
  icons/icon-192.png
  icons/icon-512.png
  icons/icon-maskable-512.png

IMPORTANT - FILE NAME
These files are set up for a game file named "index.html".
If you ever rename it, update this line in manifest.json to match:

  "start_url": "./index.html",

and this line near the bottom of sw.js:

  caches.match('./index.html')

FUTURE UPDATES
- Changing the game: just upload the new index.html. Players get it
  automatically the next time they open the game with internet.
- Changing the icons or manifest: also open sw.js and bump the version
  at the top, e.g. 'ata-quest-v1' -> 'ata-quest-v2'. Do the same in
  index.html (search for ata-quest-v1).
