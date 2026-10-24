# flow-mcp upgrades

Based on upstream commit `84b548f`. **Use the latest zip for the full project.**

- **`flow-mcp-studio-x.zip`** — the latest, complete project with Studio X: 15 production types (micro-drama,
  documentary, Bible story, UGC, YouTube, Shorts, TikTok, Reels, product ad, explainer, animated, trailer, podcast,
  music montage, custom), 12 platform presets (TikTok, YouTube, Reels, LinkedIn…), pause/cancel, video-to-video
  import, QA stage, VoiceStudio engine, and the Drama Studio pipeline.
- `flow-mcp-COMPLETE.zip` — the previous complete project (Drama Studio + VoiceStudio, micro-drama only).
- `flow-mcp-drama-studio.zip` / `drama-studio.patch` — the Drama Studio upgrade as a changeset.
- `flow-mcp-voicestudio.zip` / `voicestudio.patch` — the earlier VoiceStudio-only upgrade.

To install the full project:

1. Extract **flow-mcp-studio-x.zip**. You'll get a folder called `flow-mcp`.
2. Copy its contents into your flow-mcp folder, replacing the files that already exist.
3. In PowerShell:
   ```
   cd D:\SW\INSTAL\flow-mcp2
   Remove-Item -Recurse -Force dist
   npm install
   npm run build
   ```
4. Fully quit Claude and reopen it. The Drama tab shows the new production type and platform pickers.
