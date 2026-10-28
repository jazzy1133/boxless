# Boxless
Your portal. No box. No hardware info.

## ⬇ [Download Boxless.apk](https://github.com/jazzy1133/boxless/raw/main/Boxless.apk)
Current version: 0.4.25 — tap the link, then open the downloaded file and allow install when Android asks. Future versions will also be offered as updates inside the app.

## What is Boxless?

Boxless is an app for watching your own TV portal on Android — live channels, movies, and series — on your phone, tablet, or Android TV. It replaces the set-top box: no extra hardware, and no hardware information sent from your device.

It works with Ministra / Stalker portals. Boxless doesn't come with any channels — it plays the ones from your own portal subscription.

## What's new in 0.4.25

- **Recommend matching actually works now** — tapping a trending card used to find nothing even for exact titles (the matcher was scoring the portal's full display label, "The Crown (English) - ENGLISH | SERIES", so an exact title scored 0.38 and never reached the match bar). It now scores the title only, so the real title ranks first in the close-matches list.
- **Indian titles in the Netflix and Prime rows** — the rows already asked TMDB for India, but stacked the US list first, so Indian titles sat far down and never surfaced. The regions are now mixed together, so an Indian title appears every few cards in the same rows.
- **The screen stays awake while you watch** — nothing in the app ever asked Android to keep the screen on, so it dimmed mid-play on phone and tablet. The fullscreen player and the preview pane now hold the screen while playing (including while a slow stream is still buffering); pause and it dims normally, and browsing lists still sleep as before.
- **Search uses the exact words** — "Grey's Anatomy" was searched as "grey s anatomy" because the apostrophe was turned into a space. Punctuation now stays as-is, so the portal gets the real title words.

## What's new in 0.4.24

- **Recommend is now tap-to-pick** — trending and smart cards show TMDB titles; tap one and Boxless lists the close matches on your portal, so you pick the right language or version (it broadens the search automatically if the full title finds nothing, and says "Not on your portal" when a title isn't there at all). No more silent 0-matches.
- **Send tells you why it failed** — the support log button used to say "no connection" for every failure, even when the phone was online. It now names the cause (address lookup, secure connection, too slow, and so on), and retries once for the failures that can succeed on a second try.
- **Continue Watching posters come back** — cards saved before posters existed get their poster filled in automatically when you open Recommend, and resuming a title from its ⋮ menu no longer wipes the poster it already had.
- **A refused stream gets one more chance** — if the streamer refuses a direct play link (403), Boxless now asks the portal to mint a proper link once instead of failing straight away.

## What's new in 0.4.23

- **QR phone setup** — typing portal details on the TV is hectic, so Profiles now has **Set up from phone**: the TV shows a QR code, you scan it with your phone, and type the title, host, MAC and TMDB key on the phone keyboard. The TV saves the new profile and offers to connect straight away. The setup page is served by the app itself on your own Wi-Fi, runs only while the QR screen is open, and needs the 6-digit code shown on the TV — it stops the moment the screen closes, the setup completes, or the code expires (10 minutes).
- **Set TMDB key from phone** — in Settings, next to the TMDB key button: the same QR flow for the key alone.
- Typing on the TV still works exactly as before — the QR flow is an extra option, not a replacement.

## What's new in 0.4.22

- **Recommend** — the Continue Watching tile is now Recommend. It opens with big hero slides of the top trending titles, then your Continue Watching grid, then **Trending on Netflix** and **Trending on Prime Video** rows, smart **Because you watched** rows, and a **Channels you watch most** strip. Tap a card and Boxless lists the close matches on your portal, so you pick the right language or version — a title that isn't on your portal says so instead of pretending to play.
- **Needs your free TMDB key** — the trending and smart rows come from TMDB (themoviedb.org), which is free: sign up there, go to Settings → API, copy the v3 key, and paste it in Boxless under Settings → Recommend. Without a key, Continue Watching and your channels still work; the trending rows just show a card pointing you to Settings.
- The Apple TV look: full-bleed hero with a white Play pill, rows with bold headers, and a focused card that lifts with a white glowing border.

## What's new in 0.4.21

- **Continue Watching** — a new tile, first in the row on Home, opens its own screen listing everything you stopped halfway through: movies and episodes, most recent first, each with its poster, a progress bar, and how much time is left. Tap a card and it resumes exactly where you stopped.
- **Remove from Continue Watching** — long-press a card (or its ⋮ menu, or the MENU key on a remote) to take a title off the list.
- Nothing half-watched yet? The screen says so instead of showing an empty grid.

## What's new in 0.4.20

- **One tap opens things now** — some rows needed two taps: the first tap only highlighted the row and the second one opened it. Rows now open on the first tap, on phone and tablet. The TV remote works exactly as before: one press of OK to open, long-press OK still toggles favourites.
- **A tap while something is loading now says so** — if you tap a season or a genre while its list is still loading, the app shows a brief "Loading…" instead of silently ignoring the tap.

## Install

Boxless isn't on the Play Store, so you install it directly from this page. It takes about a minute.

1. Tap the download link above to get `Boxless.apk`.
2. Open the downloaded file. Your browser may ask you to allow installs from it — tap **Settings**, turn on **Allow from this source**, then go back and tap the file again.
3. Tap **Install**, then **Open**.
4. Add your portal: give it a name, enter your portal address, and the MAC address your provider registered for your account. Pick the profile and it signs in.
5. That's it. Updates arrive inside the app (Settings → Check for updates) — you don't need to come back here to download again.

Needs Android 7.0 or newer, on a phone, tablet, or Android TV.

## What it can do

- Live TV, movies, and series from your portal, with a programme guide and catch-up where your portal offers it.
- Resume: start a movie or episode again and pick up where you stopped.
- Episodes auto-play the next one when one finishes (5-second countdown you can cancel; switch it off in Settings → Playback).
- Search that searches the whole catalogue, not just what's on screen.
- Favourites saved only on your device — they never leave it and never sync to the portal.
- A hardware-info switch for each profile, off by default: with it off, Boxless sends nothing about your device — only the portal serial your provider already knows.
- Two looks: Normal Black and Rainbow Butterfly.
- Same app on phone, tablet, and TV, with remote-friendly navigation on TV.
- In-app updates, and a built-in way to send logs to support if something goes wrong.
- Recommend: hero slides plus trending and smart rows from TMDB (needs your free TMDB key); tap a card to see its close matches on your portal and pick the version to play.

## Privacy

- No ads, no analytics, no account, no tracking.
- The only thing Boxless ever sends outside your portal is an anonymous check for a new version (once a day at most) and a log file — only when you press Send yourself.
- If you add a TMDB key, Boxless also asks TMDB (themoviedb.org) for trending lists and poster art — only with your own key, and nothing about you or your viewing leaves the device except the title names it looks up.
- It asks for five permissions only: internet, network state, wake lock, run at start-up, and installing its own updates.

## Support

Something not working? In the app, go to Settings → Diagnostics → Send logs to support. You'll get a short code — share that code when you report the problem and the log can be found with it.
