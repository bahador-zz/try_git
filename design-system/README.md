# Coolchy Design System — Review Workflow

## How this works

1. **Round 1** (`rounds/round-1.html`): 100 design *concepts* (style, motif, palette,
   suggested product) spanning current Etsy/POD trends — not rendered images yet.
2. Open the HTML file in any browser (just double-click it, no server needed).
3. For each card: click **Like**, **Pass**, or **Later**, and optionally type notes.
   Progress auto-saves to your browser's local storage as you go.
4. When done, click **Export Feedback (.json)** — this downloads a JSON file.
5. Send that JSON file back so the next batch of 25 can be generated from your
   "Like"/"Later" picks and notes.
6. Designs you mark **Like** in later rounds get rendered as real images via
   `gpt-image-1` (medium quality) once an OpenAI API key is wired in.

## Files

- `rounds/round-1.html` — the 100-concept review gallery (self-contained, no deps).
- `feedback/` — exported feedback JSON files land here once you send them back.
