# REMsound - Download Hub

**Local-first voice dictation for Windows.** Hold a key or click the floating orb,
talk, release, and your words are typed into whatever app you're using. Speech is
transcribed on your own PC. Optional AI polish can reformat selected text with local
rules/Ollama or a cloud provider you explicitly choose.

## Download

**[Get the latest REMsound for Windows here ->](../../releases/latest)**

1. Download the zip and unzip it anywhere.
2. Double-click `INSTALL.bat` to copy REMsound into your user folder and create
   Desktop/Start Menu shortcuts.
3. Launch REMsound, hold **Right Ctrl** or click the orb, and talk.

> Windows SmartScreen will warn once because the app is not code-signed.
> Click **More info -> Run anyway**.

The first dictation downloads the speech model (~75 MB) one time only. After that,
normal dictation works offline.

## Privacy

- Microphone audio never leaves your computer.
- Optional cloud polish sends only the text you choose to reformat, never audio.
- Optional update checks only query GitHub Releases for the latest public version.
- API keys and personal shortcuts live in your local `config.json`, not in this repo.

## Requirements

- Windows 10/11, 64-bit
- A microphone

*This repository hosts release downloads only.*

---

<details>
<summary>Maintainer notes (release process)</summary>

- Built from the private source repo (`lJazzpahlol/REMsound`) - see its
  `ARCHITECTURE.md` for the full packaging recipe (bundled Python runtime,
  bytecode-only app, sanitized config).
- The zip asset is **always named `REMsound-win64.zip`** so the
  `/releases/latest/download/REMsound-win64.zip` URL used by the website and app
  updater never breaks. Versions live in the tag (vX.Y.Z).
- Publish: `gh release create vX.Y.Z REMsound-win64.zip --repo lJazzpahlol/remsound-download --title "REMsound X.Y"`.

</details>
