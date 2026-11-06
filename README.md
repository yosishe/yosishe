## Product & marketing: positioning, product specs, and prototypes I build with AI

Since 2019 I've worked with adults with special needs at an NGO, where I also coordinate shifts. Over
the past year I've built products for a business-consulting firm, a care facility and community
groups, with AI agents writing most of the code. I'm looking for a product or product-marketing role.

### Selected work

**Free IQ test funnel** · IQly × Arpeely AI Builder Challenge, 2026 · [live prototype](https://yosishe.github.io/iqly-flow/) · [repo](https://github.com/yosishe/iqly-flow)

People searching for a free IQ test expect to see their number, and in this category a sign-up gate
reads as a paywall trick. So I positioned the funnel on trust: it says up front what's free and blurs
nothing. **The success metric is verified accounts per visitor, not click-through**, so the whole
funnel is measured, not only the ad. The package has three A/B test designs with decision rules,
three ad creatives and a [measurement spec](https://github.com/yosishe/iqly-flow/blob/main/docs/MEASUREMENT-SPEC.md).
I set the constraints and chose the test bets; AI agents built the code, questions and creatives
([work log](https://github.com/yosishe/iqly-flow/blob/main/docs/AI-WORKLOG.md)).
*Status: a prototype, not run on live traffic. What I'd change: put "free" in the headline itself, not only in the line above it and the box below it.*

<p>
<img src="https://raw.githubusercontent.com/yosishe/iqly-flow/main/ads/ad-250x250.png" width="250" alt="250×250 ad: a sample puzzle question and a Start the test button">
&nbsp;
<img src="https://raw.githubusercontent.com/yosishe/iqly-flow/main/presentation/assets/control-partial-result.png" width="170" alt="Result screen: the number of correct answers is shown free, and a free email-only account unlocks the IQ range and rank">
</p>

**Audience messaging and a meeting coordinator** · business-consulting firm, 2026 · *private*

I sharpened three target audiences and wrote each one a message built on the value it gets. The
messages went to the client for approval, and I produced marketing videos to replace the text message
used before. I also built a meeting coordinator: you paste people's free-text replies about when they
can meet, and it extracts the times, picks who to follow up with next and drafts a summary in Hebrew.
*Status: the coordinator is in pilot.*

**Shift scheduling for a 24/7 care facility** · 2026 · *private*

The coordinators were happy with their paid scheduling tool; the reason to look at an alternative was
its cost. So the bar was everything they use today, plus fewer manual fixes after the automatic run.
I wrote the spec from a 48-minute recorded meeting with the coordinators and their screenshots;
requirements cite their source and are marked confirmed, inferred or open.
**The pilot's pass/fail criteria were written before any code: zero hard-rule violations, fewer manual
fixes than with the current tool, and coordinators willing to switch.**
*Status: built and tested, not piloted. The plan is a one-month run beside the current tool; nothing is approved yet.*

**Members site for a career-change community** · 2026 · *private*

A needs survey (N=19) found that 16 wanted lectures and only 3 wanted mentoring. **I dropped the
planned chatbot** and centred the site on events and a member directory, then settled the visual
identity and made a 22-second film for the launch.
*Status: online behind a member login; no public launch yet.*

These repos hold client, staff and member data, so they stay private. I'm glad to walk through the
specs, screens and decisions in an interview.

### Also

- **Landing page for an independent group facilitator, 2026.** Messaging based on previous cohorts, through to the live site.
- **[NeuroFlow](https://neuroflow-v2.vercel.app)**, a Hebrew day planner for people with ADHD (side project). Live, no account needed.
- **Rare-disease research, volunteer at Yad LeNeshima (CCHS), since 2026.** With the nonprofit's chief scientist, I'm building the data and tagging layer of an AI system for the research literature, and have turned results into decision decks over eight feedback rounds. Related course project: [evidence navigator](https://github.com/yosishe/cchs-evidence-navigator-zoomcamp), which finds the source passages behind a literature question.
- **AI lectures and workshops since 2024**, for non-technical audiences and for developers. [Kit from a September 2026 workshop](https://github.com/yosishe/personal-agent-starter).
- **FoodTech hackathon, Ben-Gurion University, 2023.** Our team aimed an alternative protein at omnivores squeezed by the cost of living, instead of the usual animal-welfare message. I wrote and delivered the pitch.

### How I build

I set the spec, the success metric and the decisions; AI agents write most of the code and keep the
decision log; I review what ships. My rule for AI features: the model reads the messy input and plain
code makes the decisions, so the result is predictable.

Israel · Hebrew and English · [LinkedIn](https://www.linkedin.com/in/yossi--shemer)

<p dir="rtl" lang="he">מחפש תפקיד בניהול מוצר או בשיווק מוצר. אפשר לכתוב לי בעברית או באנגלית.</p>
