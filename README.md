## Yosi Shemer — agent systems that have to be right, not just fluent

[LinkedIn](https://www.linkedin.com/in/yossi--shemer) · Israel · Hebrew and English · open to AI / agent-engineering roles

I build pipelines where the model is allowed to write and the code decides what survives:
every quote located in its source, every number labeled `[measured]` or `[estimated]`, every
gate a test that can fail. The interesting part of an agent system is not the demo; it is what
the thing costs, what it silently breaks, and how you would know either way.

**Currently:** volunteer AI research advisor to a rare-disease literature effort (CCHS /
*PHOX2B*), and shipping the video-to-brief tools below.

**How I work:** verification first, honest measurement, small real commits. Claude Code and
OpenAI Codex co-author much of this work and are credited in the commit trailers; the design
decisions, the gates, and the numbers are mine to defend.

### Pinned, in reading order

1. **[talkbrief](https://github.com/yosishe/talkbrief)** — a YouTube talk becomes a
   slide-by-slide brief, and every quote is **mechanically verified** against the transcript
   before you see it. The model never writes a timestamp; code locates each quote (digit-exact)
   and stamps the second. One real-model run on a 60-minute talk: 351/354 quotes grounded, the
   3 misses flagged in amber, none dropped `[measured]`. 55 offline tests in CI. Hebrew/RTL
   output. MIT.
2. **[token-efficient-skill-optimizer](https://github.com/yosishe/token-efficient-skill-optimizer)**
   — audits AI skills and system prompts for what they actually cost per trigger, under a hard
   rule: no task-success loss, no safety weakening. It can tell you *not* to optimize, and did:
   a pilot that came back at −0.7% was published at −0.7%. 27 rules over 42 machine-checked
   sources; a `[measured]` claim with no data file behind it fails CI. MIT.
3. **[cchs-tagging-method](https://github.com/yosishe/cchs-tagging-method)** — the case study
   behind the CCHS work. *The LLM extracts, the code decides*: controlled vocabularies, MeSH/GO
   anchoring, and a quote gate that found 195/195 pilot quotes verbatim in their source PDFs
   `[measured]`. Method and numbers only; the data belongs to the research collaboration.
4. **[visual-video-summarizer](https://github.com/yosishe/visual-video-summarizer)** — a
   Claude Code skill that turns a video into an illustrated HTML page, Hebrew (RTL) by default.
   Frames are chosen by candidate ID and pixel-verified on re-grab; the engine is scored on a
   committed benchmark, not eyeballed. MIT.
5. **[neuroflow](https://github.com/yosishe/neuroflow)** — a Hebrew RTL daily-planning web app
   (React, TypeScript, Vite). The one product here that is not a pipeline: 120 unit tests and a
   production build in CI `[measured]`, bidi-correct layout, guest mode with optional Supabase sync.

### Elsewhere

- [skills-il/developer-tools#27](https://github.com/skills-il/developer-tools/pull/27) — the
  skill optimizer submitted to the Israeli developer-skills catalog, with the negative-trigger
  cases its checklist asked for.
- Hebrew / RTL document generation (PDF, DOCX, PPTX with correct bidi) runs through most of the
  work above; it is a narrow niche that is genuinely hard and very often done badly.

### Background

Computer Science graduate · data science certificate · based in Israel. Most client- and
research-facing work lives outside this profile; happy to walk through any of it.
