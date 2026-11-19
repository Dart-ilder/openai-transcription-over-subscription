# OpenAI Transcription over Subscription

Live speech-to-text from OpenAI with **partial transcripts while you speak** and a final transcript when you stop. This approach uses the dictation backend of the ChatGPT web app and authenticates with `codex login` through your ChatGPT subscription, rather than using a separately billed OpenAI API key. It worked on the tested account, but it is unofficial and availability is not guaranteed across plans or over time.

This repository documents how to reproduce the approach for your own transcription client. It is not a ready-to-run proxy.

## Tested on CachyOS with OpenWhispr

I tested this on CachyOS with OpenWhispr 1.11.0. A local adapter connected OpenWhispr's existing streaming client to ChatGPT dictation. The widget showed partial text while I spoke and inserted the final transcript after I stopped. OpenWhispr is one example, not a requirement.

## For a coding agent

Read [AGENTS.md](AGENTS.md) for the step-by-step workflow. Discover the current WebSocket in the web composer's DevTools, verify that partial text arrives while recording, test with public audio, then bridge the results into the user's transcription client. The guide includes the OpenWhispr example. Do not replace a working backend until the bridge passes an isolated test.

Search terms: OpenWhispr live transcription, ChatGPT browser dictation, Codex login, Deepgram-compatible streaming, Linux voice typing.
