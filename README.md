# iStudio assets

Media served over jsDelivr for **iStudio** (`istudio.genai.io.vn`).

## music/

Royalty-free tracks offered in the **Create** video maker
(<https://istudio.genai.io.vn/create/>). The picker reads
`public/create/music.json` in `genai-site/istudio-app`, which points at:

```
https://cdn.jsdelivr.net/gh/genai-assets/istudio@main/music/<slug>.mp3
```

### Adding a track

1. Drop the MP3 in this folder with a descriptive, slugified name
   (`midnight-drive.mp3` — the picker shows the name from `music.json`).
2. Add an entry to `music.json` in `istudio-app`:
   `{ "name": "Midnight Drive", "url": ".../music/midnight-drive.mp3" }`
3. Deploy `istudio-app` (the JSON ships with the Worker; the MP3s don't).

Keep files small (a 30-60s loop is plenty; the maker caps clips at 30s) and only
add music you own or that is licensed for redistribution — this repo is public.
