Dhara ❦ Pranjal — wedding invitation website
=============================================

Files
  index.html   the invitation guests open
  send.html    your page for making personal links (open it at  …vercel.app/send )
  vercel.json  makes /send work without .html
  couple.webp  Dhara & Pranjal's illustration (background removed), shown in the doorway,
               the hero arch and the footer
  og.jpg       the picture WhatsApp shows when you send the link (1200 x 630)
  music.mp3    "A Thousand Years" (violin & piano) from your video, looped, plays when the doors open

PUT IT ONLINE / UPDATE IT
-------------------------
  npx vercel login        (first time only)
  npx vercel --prod       (run inside this folder; same command every time you update)
Your invitation:   https://dhara-weds-pranjal.vercel.app
Your link maker:   https://dhara-weds-pranjal.vercel.app/send

IMPORTANT: the WhatsApp link preview uses the full address of og.jpg. If Vercel gives you a
different address, open index.html and change the two lines near the top that contain
"dhara-weds-pranjal.vercel.app" (og:url and og:image), then deploy again.
WhatsApp remembers previews, so test with a fresh link such as  …vercel.app/?v=2

SEND PERSONAL INVITATIONS
-------------------------
1. Open  https://dhara-weds-pranjal.vercel.app/send  on your phone.
2. Type the guest's full name exactly as it should appear (Gujarati, Hindi or English),
   e.g.  શ્રી રમેશભાઈ પટેલ પરિવાર
3. Optional: their WhatsApp number, and the language the invitation should open in.
4. Tap "Send on WhatsApp". WhatsApp opens with the message and their personal link ready.
For many guests: paste one per line ("Name, number"), tap "Make links", then send each row.
Rows you've sent are marked ✓ Sent on that phone.

When a guest opens their link, their name hangs on a nameplate in the middle of the palace doors
and is already filled in on the RSVP form.

MUSIC
-----
music.mp3 is "A Thousand Years" (violin & piano), taken from your video and made into a smooth
57-second loop. It starts softly when the doors open; guests can pause it with the round button.
To use another song, replace music.mp3 (same name) and run  npx vercel --prod  again. To skip an
intro, open index.html, find  musicStartAt: 0  near the top of the <script> and set the seconds.

EDITING TEXT
------------
All wording, times, family names and the RSVP WhatsApp number are near the top of the
<script> in index.html (CONFIG, EVENTS, FAMILY, INVITE and T for Gujarati/Hindi/English).

CHANGING THE COUPLE PICTURE
---------------------------
Replace couple.webp with another picture of the same shape (portrait, transparent background works
best, about 640 px wide). Faces should be in the top third, like the current one.
