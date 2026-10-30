Học Phật Pháp (hocphatphap.net) - static HTML version
=====================================================

Upload the CONTENTS of this folder (including the hidden .htaccess file) to the web root of
hocphatphap.net, or to any subfolder for a staging preview. All links are relative.
Needs Apache or LiteSpeed with .htaccess / mod_rewrite enabled.

290 pages, all at their original URLs:
- 213 video pages (/videos/N), the video list (/videos/), audio and document pages
- news, introduction, photo library (including Vietnamese-character URLs), /lybrary/... photos
- Drupal /node/N and /taxonomy/term/N pages, and the paged photo list (?page=1)
Pages without a trailing slash are stored as .html files; .htaccess serves them at the
original address. /videos (no slash) redirects to /videos/, which is the same list.

Upload tip: some folder and file names contain Vietnamese characters. Extract the zip on the
server (e.g. in the hosting file manager) rather than on Windows, so the names stay exact.

Not included
------------
- /contact: the live contact page returns a server error (500) after ~55 seconds, so there was
  nothing to copy. The menu link to it will show "not found".
- RSS feeds (/taxonomy/term/N/all/feed).

Already broken on the live site (unchanged here)
------------------------------------------------
- Videos use the old Flash YouTube player, which modern browsers do not play.
- Two audio files are missing on the server ("Nhạc Xưng Tán Đức Phật A Di Đà..." and
  "Nhạc Niệm Phật Quán Thế Âm - Rất Hay.mp3"), plus some old theme images and icon fonts.

Noindex (staging)
-----------------
Every page has <meta name="robots" content="noindex, nofollow" /> and .htaccess sends an
X-Robots-Tag: noindex, nofollow header, so search engines will not index this copy.
BEFORE GOING LIVE on the real domain: remove that meta line from each page and delete the
"BEGIN noindex ... END noindex" block from .htaccess, or the site will drop out of Google.
