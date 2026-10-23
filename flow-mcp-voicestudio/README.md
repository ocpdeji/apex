# flow-mcp + VoiceStudio upgrade

Adds [VoiceStudio](https://github.com/debpalash/VoiceStudio) to
[flow-mcp](https://github.com/GTAI-1/flow-mcp) as a premium narration engine. It is based on flow-mcp commit `84b548f`.

- `flow-mcp-voicestudio.zip`: the 6 changed files. Extract it into your flow-mcp folder, replacing the old files.
- `voicestudio.patch`: the same change as a git patch (`git am voicestudio.patch`).

After either one, run `npm run build` in the flow-mcp folder, then fully quit and reopen Claude.

## What it adds

- `flow_narrate` with `engine: "voicestudio"`: your cloned or designed voices, an engine and its built-in voices,
  language (646), personality, speed, quality (draft / balanced / studio) or exact steps, guidance, seed, finishing
  effect, denoise, exact length, bit depth, pronunciation dictionary, loudness levelling, and scripts up to 20,000
  characters.
- `flow_voice_clone`: a new voice from a 5-30 s recording (only with the speaker's permission).
- `flow_voice_design`: a new voice from a description, with a preview mode that saves nothing.
- `flow_voices`: also reports whether VoiceStudio is running, its voices, engines, personalities and effects, and
  how to install it.
- Flow Studio → Voice → **VoiceStudio ✦**: the same controls, a status light, and clone and design forms.
