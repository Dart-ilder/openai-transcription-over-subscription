# ChatGPT dictation in OpenWhispr: an agent field guide

Goal: show live partial transcripts in the OpenWhispr desktop widget using the same dictation feature as the ChatGPT web composer. This repository is a reproducible investigation guide, not a ready-to-run proxy. It intentionally does not pin a private upstream URL: discover and verify the current protocol instead of assuming an old capture still applies.

On CachyOS with OpenWhispr 1.11.0, the approach worked in a manual test. At the time of testing, a Codex ChatGPT login was sufficient for a direct connection, without browser cookies or a separate paid API key. This is not official or guaranteed subscription coverage.

## For a coding agent

Read [AGENTS.md](AGENTS.md). In short: inspect the web composer's dictation in DevTools, verify that partial text arrives while recording, test with public audio, then bridge the streamed results into an existing OpenWhispr provider. Do not replace a working backend until the bridge passes an isolated test.

Search terms: OpenWhispr live transcription, ChatGPT browser dictation, Codex login, Deepgram-compatible streaming, Linux voice typing.
