# CleanTV apps: releases

Ready-to-install Android APKs of the family's home apps. Only the builds live here; the source is kept elsewhere.
Each app has its own releases, tagged `<app>-v<version>`.

| App | What it is | Latest |
|---|---|---|
| **SIMKL Tracker** (`com.cleantv.tracker`) | Your movies, series and anime on the phone, synced with [SIMKL](https://simkl.com): Up Next, Upcoming, your lists, search, episode marking, ratings, Where to Watch, trailers, and automatic tracking of what you watch in Netflix, Disney+, Prime Video, Crunchyroll and others. | [Releases](../../releases?q=simkl-tracker) |
| **TV Home, its add-ons + TV Remote** (`com.gathin.tvhome`, `com.cleantv.nowplaying`, `com.cleantv.simkl`, `com.cleantv.tvtools`, `com.cleantv.remote`) | Released together, tagged `tv-home-v…`. On the TV: the home screen (the [CleanYourTV](https://github.com/Gathin23/cleanyourtv) launcher, MIT, with the family's additions: Quick Panel, the Companion service), **Now Playing** (music screen and screensaver with synced lyrics in the Radiant Lyrics style), **SIMKL for TV** (your SIMKL lists on Home and tracking) and **TV Tools** (Night Sound, Bedtime, Picture Off and more). On the phone: the remote that pairs with it (D-pad, keyboard, apps, inputs, Now Playing, the TV's screen live), which connects to whichever of your TVs is on the Wi-Fi. The release notes list the adb commands each TV app needs. | [Releases](../../releases?q=tv-home) |

## Install on an Android phone

1. Open the latest release on your phone and download the `.apk` file.
2. Open it. Android asks to allow installs from your browser or Files app the first time: allow it, then **Install**.
3. To update later, install the newer APK the same way; your sign-in and settings stay.

Android 8 or newer. To check a download, compare its SHA-256 with the one in the release notes.

## SIMKL Tracker: first start

- **Your own SIMKL account.** Everyone signs in with their own SIMKL account, so lists and tracking are yours alone.
  You approve a code at simkl.com/pin, and the app never sees your password.
- **Which SIMKL app.** The first screen asks how to connect. **Use the shared app** works for most people. **Use my own
  app** is for anyone who made their own app at simkl.com › Settings › Developer (type "TV, devices & command
  line"): paste its Client ID. Either way your data is your own. To switch later, choose Profile › **Sign out and
  use another SIMKL app**.
- **Optional service keys** (Profile › Keys): TMDB, MDBList, OMDb, fanart.tv, TheTVDB, RPDB, TOP Posters, Gemini,
  OpenRouter and Anime Skip each add something (Where to Watch, ratings, artwork, AI recaps …). Tap a service to
  paste its key; each row links to the page where you get one. Keys are saved, encrypted, in the family's small key
  service on Cloudflare, under your SIMKL account only, so they come back after a reinstall. No one else's sign-in
  can read them. Signing out removes them from the phone.
- **Automatic tracking** (Profile) needs notification access, granted on Android's own page from the app's button.
