# PMI Summit 2026 capture

Lead capture page for the Process Street booth at the PMI Summit
(Omni Nashville, September 16-19 2026).

Badge photos, voice notes and typed notes are posted to an n8n workflow which
transcribes them, extracts the useful fields and appends them to the team's
tracking sheet.

Hosted as a static page rather than served from n8n, because n8n stamps webhook
responses with a `Content-Security-Policy: sandbox` that omits
`allow-same-origin`. That makes the document an opaque origin, which blocks
getUserMedia, localStorage and IndexedDB: no microphone and no offline queue.

Source of truth for this file is the vault at
`04-Process-Street/Visits/pmi-capture/pmi_app.html`.
