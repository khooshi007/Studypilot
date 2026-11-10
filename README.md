# StudyPilot desktop

A Windows app that runs StudyPilot in its own window.

## Build the .exe (on a Windows computer)

1. Install Node.js LTS from https://nodejs.org.
2. Open this folder in a terminal (PowerShell or Command Prompt).
3. Run:

       npm install
       npm run build:win

4. The installer appears in `dist\` as `StudyPilot Setup 1.0.0.exe`. Run it to install StudyPilot.

To test without building, run `npm install` then `npm start`.

## Using it

Open Settings, paste your Claude API key, and click Save key. Get a key at console.anthropic.com. Notes, results, and progress are stored on your computer, and the key is sent only to Anthropic.

## Notes

- The app is the same as the StudyPilot web artifact, with one change: it uses your API key instead of the artifact's built-in AI access.
- Updates to the web app do not reach the desktop copy automatically. Copy the new `app/index.html` in.
- Windows may show a SmartScreen warning because the installer is not code-signed.
- Versions of Electron and electron-builder are pinned loosely. If `npm install` fails, update them in package.json.
