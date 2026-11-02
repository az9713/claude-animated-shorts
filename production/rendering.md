# Shared rendering and sound workflow

The three films use Three.js scenes rendered through Remotion at 30 fps. Flat character drawings receive scene tint and shading, while painted 3D scenery carries world ink, atmospheric depth and selective focus blur.

Compositor order: scene → world ink → lens prepass → lens main pass → bloom, neutral tone map and grade → captions and audio.

The 1080×1920 composition is rendered at 4/3 scale to 1440×2560. Word timings drive caption changes, character actions, camera keys and sound cues. Narration uses an ElevenLabs library voice; music and effects are synthesized locally. Every export receives metadata, decoded-frame, timing and audio-level checks, alongside sampled visual review.

The repository is a finished-media showcase and production journal. It does not distribute the full editing environment, installed font files, API credentials or private reference footage. The MIT source notice is retained in LICENSE.source.
