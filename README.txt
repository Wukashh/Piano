LAYLA'S PIANO
=============

A piano that runs entirely on the iPad. It makes its own sounds, so there is
nothing to download while playing: no ads, no accounts, no tracking, and no
requests to any other website.

PUT IT ON THE IPAD (one time, about five minutes)
-------------------------------------------------
An iPad can only install a web app from a web address, so the files need to
sit on a website once. After that the iPad keeps its own copy and never needs
the internet again.

1. Put this whole folder on any free static host that serves https, for
   example Netlify Drop (drag the folder onto the page), GitHub Pages or
   Cloudflare Pages.
2. On the iPad, open the address it gives you in Safari and wait for the
   piano to appear.
3. Tap the Share button, then "Add to Home Screen", then "Add".
4. Open "Piano" from the Home Screen once while still online.
5. Done. It now opens full screen and works in airplane mode.

Tip: turn off the iPad's Silent Mode in Control Center if you hear nothing.

FILES
-----
index.html            the whole app (page, styles, sound and songs)
sw.js                 saves the files on the iPad for offline use
manifest.webmanifest  name, icon and full-screen settings
icon-180.png / icon-512.png   Home Screen icons

CHANGING IT LATER
-----------------
Songs are plain text near the bottom of index.html, in the TUNES list:
note names with an octave number, and ":2" for a note twice as long.
After any change, raise the version in sw.js (v1 to v2) so the iPad
fetches the new copy the next time it is online.
