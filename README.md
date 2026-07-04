# REMsound — Download Hub 🎙️

**Voice dictation that runs 100% on your own PC.** Hold a key, talk, release —
your words are typed into whatever app you're using. No cloud, no accounts,
no subscription. Your speech never leaves your machine.

## ⬇ Download

**[Get the latest REMsound for Windows here →](../../releases/latest)**

1. Download the zip and unzip it anywhere
2. Double-click `INSTALL.bat` (puts icons on your Desktop & Start Menu)
3. Launch REMsound, hold **Right Ctrl**, and talk

> Windows SmartScreen will warn once because the app isn't code-signed —
> click **More info → Run anyway**.

The first dictation downloads the speech model (~75 MB) — one time only,
then it's fully offline.

## Requirements

- Windows 10/11, 64-bit
- A microphone

*This repository hosts release downloads only.*

---

<details>
<summary>Maintainer notes (release process)</summary>

- Built from the private source repo (`lJazzpahlol/REMsound`) — see its
  `ARCHITECTURE.md` for the full packaging recipe (bundled Python runtime,
  bytecode-only app, sanitized config).
- The zip asset is **always named `REMsound-win64.zip`** so the
  `/releases/latest/download/REMsound-win64.zip` URL used by the website
  (remsound-website → Vercel) never breaks. Versions live in the tag (vX.Y.Z).
- Publish: `gh release create vX.Y.Z REMsound-win64.zip --repo lJazzpahlol/remsound-download --title "REMsound X.Y"`.

</details>
