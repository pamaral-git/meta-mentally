# Meta Mentally — Private Personal Superintelligence

Forked from my repository https://github.com/pamaral-git/mentally  
Hackathon: Meta Global AI Developer Hackathon (Cerebral Valley), submission 4 Nov 2026, 9:00 PM ET | Finals: 9 Nov 2026 (Indie Developer — Theme: Build for Your World)

> I built Mentally as a single-file, offline-first wellbeing companion because wellbeing tools should not harvest your most vulnerable data. Meta Mentally evolves it into a private personal superintelligence using Meta's Muse models: local-first intelligence for your most sensitive reflection, and cloud Muse power for creative, abstracted tasks. Private by architecture, not by policy.


## Problem

Personal intelligence is incomplete without the mental and emotional aspect that shapes our lives.

[Mentally](https://github.com/pamaral-git/mentally) was built from lived experience: a safety plan app that is actually yours — private, self-hosted, free, no login, no tracking. **Meta Mentally** keeps that promise and extends it with Meta's newest models:
- **Private Reflection with local-hosted Muse Glimmer 30B** ◦ User journaling and safety plan drafting runs locally with Glimmer helping articulate warning signs, coping strategies, and reasons to live from the user's own words (Journal text never leaves the user's machine in Local Mode. This is the core feature)
- **Deep Reflection Session** ◦ Inspired by the [Nat Fridman-Alexander Wang idea of a single deep AI session](https://youtube.com/shorts/wwiTBL_hYIM) can surface patterns that normally take years of reflection to see. Meta Mentally offers this same guided structured reflection leveraging the user's context completely locally.
- **Voice Session** ◦ Local STT-ASR model or Muse Voice Transcribe (cloud, opt-in). Transcription is then processed by Glimmer locally.
- **Physical Grounding** ◦ SAM 3.1 grounding is opt-in cloud only, on user-approved photo. Local Mode uses text description only.

## Design

**Hybrid by Design**. Meta's Muse models are state-of-the-art but still large `Muse Glimmer 30B` the largest model everyday consumer model can run privately on consumer hardware with quantization, as `Muse Spark Open 816B-A42B` is too large for everyday consumers to run. Therefore we'll adopt the following architecture:
- **Local by Default** ◦ With `Muse Glimmer 30B` (llama.cpp on device), fallback to mixture of `Meta Llama models`, for on device safety plan, journal and reflection. Single HTML file exports and config live in a local directory, never in the cloud.
- **Cloud Hosted Opt-in** ◦ `Muse Spark`, `Muse Image`, `SAM 3.1` and `Muse Voice`, for abstracted, non-sensitive tasks only, user-approved.

What We Are Not Building:

> This is not Therapy, Diagnosis, treatment or replacement for professional support.

It is a personal companion for structured self-reflection, with the user in control.

> This is not a Wellness App disguised as a Cloud Data harvesting service.

It relies on a default Local Mode with no analytics, telemetry, trackers or third-party data sharing.

**This is, I believe an innovation to preserve wellbeing and sustainable engagement with Meta AI through trust, using Muse Code for the agentic coding development and Muse Wonder for ideation, design and exploration.**

---

Current State ◦ Still just a fork
