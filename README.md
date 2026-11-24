# Redirect v2 — free focus web prototype

## Install / host
Open index.html in a browser or serve the folder on localhost. For Android and location features, deploy the files to a GitHub Pages repository root, then enable Pages in Settings → Pages (main / root). Use Chrome's Install or Add to Home screen option. All data remains local; no subscription or account.

## New blocking rules
Edit a distraction in Block list. By default existing v1 distractions always require a task. Enable one or more conditions: weekly time window (including overnight), daily allowed launches, daily estimated minutes, or location inside/outside a saved radius. Any matching rule triggers the gate. Hard daily caps are enabled by default; turn them off if tasks should grant temporary access beyond the limits. Other rules allow task-earned reward windows. Counts reset at local midnight.

<<<<<<< main
Location: use current location or enter coordinates manually, plus radius. HTTPS and browser permission are required. When a location check is needed, tap Open again after the check completes. Unknown or uncertain location triggers the gate. No background tracking. Use Settings to refresh or retry location.
=======
## Core flow
- Add alternatives in Tasks: link, Android deep link, local PDF, or offline task. Choose self-confirmation or a minimum timer plus confirmation.
- Add distractions in Block list. Choose their individual reward duration.
- Tap Open on a distraction in Today, or use Try the blocking screen. Start an alternative and open its resource. Return and confirm completion (after the minimum timer if applicable).
- Open the distraction during the reward window. A subsequent launch from Redirect after expiry requires another task.
- Activity records self-confirmed completions. Settings can export/import metadata; PDF bytes are excluded and must be reattached after import.
>>>>>>> origin/main

Usage: each launch via Redirect starts an elapsed-time session. Tap Stop on Today upon returning. Launching another distraction stops the previous session. These are estimates, not active app time; launches and usage outside Redirect are invisible. A hard cap applies at the next launch, not by closing an external app.

## Existing features
Tasks can be website links, supported Android deep links, PDFs or offline activities. Choose self-confirmation or minimum time plus confirmation. Complete a task through the gate to earn an app-specific reward unless a hard daily cap is active. History records completed tasks. Existing v1 browser storage is retained when updating the same origin. Backups include task and block settings and completion history; PDF bytes and daily usage/launch counters are not included.

## Boundaries
This is a web prototype, not device-wide blocking. It cannot intercept installed apps, monitor actual foreground usage, enforce limits outside Redirect, or track background geofences. Native Android integration is required for those features. Browser checks are subject to permissions. Task completion remains self-reported.
