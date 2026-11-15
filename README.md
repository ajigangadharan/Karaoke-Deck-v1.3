# Karaoke Deck

**Website:** https://ajigangadharan.github.io/Karaoke-Deck-V1/ · **Download:** [latest release](https://github.com/ajigangadharan/Karaoke-Deck-V1/releases/latest)

A simple two-deck audio/video player for live singers, with a lyrics pane built in. Everything is in one window: two decks at the top, your song list below, and lyrics on the right.

## Install on Windows (no setup needed)

1. Download the **KaraokeDeck-Windows-x64** zip from the [latest release](https://github.com/ajigangadharan/Karaoke-Deck-V1/releases/latest) and unzip it somewhere permanent, for example `C:\Karaoke Deck` or `D:\Apps\Karaoke Deck`.
2. Open the folder and double-click **Karaoke Deck.exe**.
3. The first time, Windows may show "Windows protected your PC" because the app is not code-signed. Click **More info**, then **Run anyway**.
4. Optional: right-click `Karaoke Deck.exe` and choose **Send to > Desktop (create shortcut)**.

Nothing else needs to be installed. The converter for unusual formats (ffmpeg) is already inside the folder.

## First run

1. Click **+** next to "Music folders" and pick the folders with your songs (you can select several at once; add more any time). They are remembered.
2. In the lyrics pane, click **Folders…** and add your lyrics folders (if you skip this, the music folders are searched for lyrics).
3. Open **⚙ Settings > Audio outputs**:
   - **Main output**: what your audience hears. Pick the sound card (or virtual audio cable) that TikTok Live Studio / OBS / Streamlabs captures.
   - **Preview output**: your headphones.
   - You can set these separately for Deck A and Deck B.

## How to use it

| What you want | How |
|---|---|
| Load a song | Double-click it (goes to the active deck), drag it onto a deck, select and press **↑ A** / **↑ B**, or drag a file straight from Windows Explorer onto a deck |
| Choose the active deck | Click the deck, or press **1** / **2** |
| Play / pause | **Space** (active deck) or ▶ |
| Stop (back to start) | **S** or ■ |
| Restart from the beginning | **R** or ⏮ |
| Waveform | Each deck shows the song's audio like a DJ player. The **upper strip scrolls** with the music: the white line is "now", music to the right is still coming, grey bars are silence. The **lower strip is the whole song**: the dim part is already played, click or drag on it to jump. When the deck is in a silent part, a yellow tag says **"silence · audio in 3.2 s"** (or "silence to the end"). The waveform takes a second or two to appear the first time a song is loaded, then it is instant |
| Change speed without changing key | Tempo slider or − / + (0.5% steps, ±30%). Double-click the slider to reset |
| Change key | ♭ − / ♯ + in half-steps, up to 5 up or 5 down. Speed does not change |
| Listen in headphones first | 🎧 **Preview** sends that deck to the preview output instead of the main output. In Settings you can choose to keep it on the main output too |
| BPM | Detected automatically after loading and remembered. If it shows half or double the real tempo, press ½ or ×2, or tap **Tap** along with the beat |
| Reset only tempo or only key | **↺ 0** at the end of the Tempo row or the Key row |
| Stereo width / mono → stereo | **FX Width**: 100% = as recorded, 0% = mono, above 100% widens. For a mono song, move it to about 150–170% to turn it into stereo |
| Reverb | **FX Reverb**: 0% = off. **↺** at the end of the FX row resets both |
| Reset a deck | **↺ Reset** sets tempo, key, width, reverb, volume and preview back to normal. Loading a new song always resets tempo, key, width and reverb |
| Find new songs you just copied into the folder | **⟳ Refresh** (or F5) |
| Search songs | Type any part of the name in the filter box. The **File name** column shows the real file name on disk, extension included (long names wrap onto two lines instead of being cut off). Smart search: words can be anywhere and in any order, `_ - .` and spaces are ignored, and small spelling differences still match (mounagal finds Mounangal, ende finds Ente). Best matches come first. The same words also search your lyrics folders |
| Column widths | Drag the right edge of any column title. Double-click the edge for the default. Remembered |
| Filter and sort | Pick audio/video only or a sub-folder, click a music folder on the left to see only that folder, click any column title to sort (click again to reverse) |
| Several music folders | **+** next to "Music folders". Right-click a folder to remove it from the list (nothing is deleted) |
| Rename a file | Select it and press **Rename** (or F2). The real file on disk is renamed, and your playlists and virtual folders follow it. Eject the song from a deck first |
| Virtual folders | **+** next to "Virtual folders". Add songs with **+ Folder**, the right-click menu, or by dragging songs onto the folder. Your files are not moved or copied |
| Playlists | **+** next to "Playlists". Right-click any song (also in search results) and pick **Add to playlist: …** directly. Or drag songs onto a playlist. Drag rows to reorder. **Export** saves an `.m3u8` (opens in VLC and most players) or `.json`. **⤓** imports `.m3u`, `.m3u8` or `.json` |
| Local lyrics | When you load a song, the lyrics folder is searched for a matching file. Search by file name or by words inside TXT and Word files. Click a result to show it. The 🔍 slider zooms (50–300%; Ctrl + mouse wheel also works, double-click the slider for 100%). **⧉ Float** opens the lyrics in a separate floating window: move it anywhere (even another screen), resize it, tick **Above all windows** to keep it on top, ⛶ for full screen, **✕ Close** to close it. It follows whatever lyrics you open in the main window (untick **Follow** to keep it on one song). Drag the bar under the results list up or down to give more height to the list or to the lyrics. ☾ switches text lyrics to a dark page (PDFs always stay white). **Scroll** auto-scrolls (slider = speed). You can also drag a lyrics file from Explorer onto the lyrics page |
| Recent lyrics tabs | Every lyrics file you open gets a tab under the lyrics title bar, so the last **8** songs stay one click away (switch between them during a live). **✕** or a middle-click closes a tab. The tabs, and the lyrics that were showing, come back when you restart the app |
| Web lyrics | **Web lyrics** tab: pick a site, type the song name (it is filled in from the loaded song) and press Search. The site opens inside the app. **Manage sites…** lets you add, edit, remove sites and choose the default. You can also type a full web address |
| YouTube (karaoke and EDM remix videos) | **▶ YouTube** tab in the right pane: type a song name (it is filled in from the loaded song) and press Search, or paste a YouTube link. YouTube opens inside Karaoke Deck; links never take you out to your browser. **Tempo − / +** changes the speed without changing the key (it goes back to 0 when a new video starts). **Output** picks the sound card YouTube plays on (choose the one your streaming app captures). **⧉ Float** continues the same video in its own window (from the same second) that you can move, resize, make full screen or keep **above all windows**; Esc leaves full screen. Sign in to YouTube once inside the tab and it stays signed in |
| Big video (karaoke videos) | Press **⧉ Video** on the deck (or double-click its small video). The video opens in its own floating window: drag it where you want, resize it, tick **Above all windows**, or press **Full screen**. The bar hides when you don't move the mouse. Space / S / R still control the deck from that window. Sound stays on the deck's normal output |
| Remembered positions | The video windows (one per deck) and the floating lyrics window reopen where you last left them, at the same size, with the same "Above all windows" choice |

### Lyrics file types

Shown inside the player: TXT, LRC (time tags are hidden), PDF, Word **.docx**, RTF, HTML and pictures (JPG, PNG, WEBP, GIF, BMP). Malayalam text displays with the Windows "Nirmala UI" font.

Other files found in the lyrics folders (old Word .doc, .odt, PowerPoint, Excel…) are listed too: **double-click** opens them in their normal Windows program, and **right-click** offers *Open with default program* and *Show in folder*.

### Adding your own lyrics website

In **Manage sites…**, add a name and a search address with `%s` where the song name should go. Examples:

- `https://www.google.com/search?q=site%3Amalayalasangeetham.info+%s` (searches only that site through Google; this is the default)
- `https://www.google.com/search?q=%s+malayalam+lyrics`
- An address without `%s`, for example `https://malayalasangeetham.info`, just opens that site.

### About VST plug-ins

Loading VST effect files is not possible in this player. The built-in **Width** and **Reverb** cover the mono-to-stereo and reverb need. If you want a specific VST, OBS Studio can load VST 2 plug-ins as a filter on your audio source (Filters > + > VST 2.x Plug-in).

## Formats

Plays directly: MP3, WAV, FLAC, OGG, OPUS, M4A/AAC, MP4, M4V, MOV, WEBM, most MKV.

Converted automatically the first time, then cached: WMA, AIFF, AC3, DTS, APE, AVI, WMV, FLV, MPG/MPEG, VOB, TS/M2TS, 3GP and others ffmpeg can read, plus videos whose codec the player can't show (for example some HEVC/H.265 files). Audio converts in a few seconds; a long video can take a minute. You'll see a progress percentage on the deck.

## Where your settings are kept

`%APPDATA%\Karaoke Deck\settings.json` holds the folders, playlists, virtual folders, lyrics sites, output devices and remembered BPMs. Converted copies of unusual formats are kept in `%APPDATA%\Karaoke Deck\converted` (safe to delete; they are recreated when needed).

## Known limits

- **Key change sound quality**: real-time and clean for voice and music within about ±3 half-steps; at ±4 or ±5 you may hear a slight "phasey" sound, like most free key changers. It adds about 40 ms of delay while the key is not 0, which is not noticeable on video.
- **Tempo**: uses the built-in time-stretch. It sounds natural up to about ±10%; at the extremes of ±30% there are audible artifacts.
- **BPM** is an estimate. Songs with a soft or free rhythm can read half or double; use ½, ×2 or Tap.
- **Preview** moves a deck to the headphone output (or to both). It is not a full DJ cue mixer with a cue/master blend knob.
- **Not supported**: MIDI/KAR karaoke files, CDG (MP3+G) graphics, and copy-protected (DRM) files.
- **Web lyrics**: Google may ask you to accept cookies the first time. Some websites refuse to be shown inside other apps; if one stays blank, open it in your normal browser.
- **YouTube**: the key (♭/♯) cannot be changed on YouTube videos, and they don't go through the decks (no waveform, BPM, reverb or preview). YouTube shows ads unless you are signed in to YouTube Premium; for a live, sign in to Premium inside the YouTube tab. If Google refuses the sign-in inside the app, the videos still play, just with ads. Only use YouTube in line with YouTube's own rules for your stream.
- **Video** windows don't reopen by themselves when you start the app; press ⧉ Video again and they come back in their remembered place.

## Keeping it smooth during a live

- Close the floating windows you are not using, and keep reverb at 0% on decks that don't need it (reverb only uses CPU while it is above 0%).
- The first time a song is loaded, the app reads its waveform and BPM in the background; after that they are remembered.
- Your song list and lyrics folders are read once and kept in memory while the app runs, and saved for the next start, so searching never waits for the folders. The very first time, the words inside your TXT and Word lyrics are read in the background (a yellow line shows how many are left); names are searchable straight away. After that only new or changed files are read. Press **⟳ Refresh** (songs) or **⟳** (lyrics) after copying in new files; the app also re-checks the folders by itself when you search, at most once a minute.
- If your laptop is on battery, plug it in. Windows slows the processor on battery, which can make any player stutter.
