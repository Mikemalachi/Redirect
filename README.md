# Redirect v1 — free focus web prototype

## Try it
Open `index.html` in a modern browser, or serve the folder with `python -m http.server 8000` and visit `http://localhost:8000`. Local file browsers may restrict storage, PDFs and app links; HTTPS hosting is recommended.

## GitHub Pages
1. Create a GitHub repository and upload the contents of this folder to the repository root (not the ZIP itself).
2. In Settings → Pages, choose Deploy from a branch, select `main`, `/ (root)`, and Save.
3. Visit the published site. On Android Chrome, use the browser menu to install or add it to the home screen if available.

## Core flow
- Add alternatives in Tasks: link, Android deep link, local PDF, or offline task. Choose self-confirmation or a minimum timer plus confirmation.
- Add distractions in Block list. Choose their individual reward duration.
- Tap Open on a distraction in Today, or use Try the blocking screen. Start an alternative and open its resource. Return and confirm completion (after the minimum timer if applicable).
- Open the distraction during the reward window. A subsequent launch from Redirect after expiry requires another task.
- Activity records self-confirmed completions. Settings can export/import metadata; PDF bytes are excluded and must be reattached after import.

Example alternatives are offline placeholders: edit them to add your own course URLs, hymn links or PDF files. Android deep links only work if the target app supports the supplied link and browser allows it; ordinary website links are a fallback.

## Boundaries
This is a local-first web prototype, not a system app blocker. It cannot detect or intercept independent app launches, measure active app usage, enforce screen time, prevent changing device time, or close external apps at the end of rewards. Its timer measures wall-clock elapsed time, and task completion is self-reported. No account or server is required. A native Android integration is the next step for genuine blocking and foreground usage tracking, subject to OS permissions and limitations.
