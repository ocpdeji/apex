# flow-mcp upgrades

These upgrades are for [flow-mcp](https://github.com/GTAI-1/flow-mcp), based on commit `84b548f`.

- **`flow-mcp-drama-studio.zip`** is the latest upgrade. It has the VoiceStudio engine and the Drama Studio, which
  makes a whole micro-drama from a title and an idea. It contains every changed file: extract it into your flow-mcp
  folder and replace the old files. `drama-studio.patch` is the same change as git patches (`git am drama-studio.patch`).
- `flow-mcp-voicestudio.zip` / `voicestudio.patch` are the earlier VoiceStudio-only upgrade, already included above.

After extracting, run these in the flow-mcp folder, then fully quit and reopen Claude:

```
npm install
npm run build
```
