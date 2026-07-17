# AI2ORBIT Drive Throughput Tester

Serverless web app that benchmarks **Google Drive upload throughput across N parallel channels (pipes)**.

- Sign in with Google (browser OAuth, `drive.file` scope only — touches only its own `AI2ORBIT_Throughput` folder).
- Generate synthetic test data (or pick a file), split it across 1–64 parallel upload streams.
- Live per-channel MB/s + aggregate throughput, speed-up vs a single pipe, and pipe efficiency (shows where the link saturates).
- **DEMO mode** runs the full UI with a simulated transport — no sign-in needed, for a quick look.

Live: https://anirudhatalmale6-alt.github.io/ai2orbit-drive-throughput/

## Setup (one time)
1. Google Cloud Console → APIs & Services → enable **Google Drive API**.
2. Credentials → **OAuth client ID** → Web application.
3. Authorized JavaScript origin: `https://anirudhatalmale6-alt.github.io`
4. Paste the Client ID into the app and sign in. No client secret needed.

(c) 2026 AI2ORBIT Co.
