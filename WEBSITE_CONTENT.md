# Personal Website — Full Content & Background

> This document contains all the text, data, and background context needed to build the site.
> Sections marked **[NEEDS CONFIRMATION]** require Rokas to verify or fill in.

---

## SECTION 1: HERO

### Text

**Name:** Rokas Tarasevičius

**One-liner:** "I build things that work."

**Intro paragraph:**

I'm a 22-year-old engineer from Lithuania, finishing my final year of Artificial Intelligence at King's College London. I've been programming robots since I was 12, won a world championship at 15, and have spent the last three years shipping production AI systems in the music industry. I like building things that solve real problems for real people.

### Links

- **Email:** rokas.tarasevicius@gmail.com
- **LinkedIn:** [NEEDS CONFIRMATION — exact URL]
- **X / Twitter:** [NEEDS CONFIRMATION — handle, or omit if inactive]
- **Phone:** +44 7354 540206 [NEEDS CONFIRMATION — include on site or not?]

### Background notes

- Born ~2003/2004 (22 years old as of 2026)
- From Kaunas, Lithuania (GitHub location says Kaunas; brainstorm says Vilnius — **[NEEDS CONFIRMATION]**)
- Now based in London
- Photo: **[NEEDS CONFIRMATION — do you have a headshot to use?]**

---

## SECTION 2: CURRENTLY

### Text

**Now:**

- Final year, BSc Artificial Intelligence at King's College London — graduating summer 2026
- Previously Engineering Lead at Stage/Salt, where I spent nearly three years building AI systems for the music copyright industry
- Exploring what to build next

### Background notes

This section should be easy to update over time. It's the "what I'm doing right now" pulse of the site. Swap the bullets as life changes.

---

## SECTION 3: THINGS I'VE BUILT

This is the core of the site. Each project should be a short narrative, not a bullet list. Stories > specs.

---

### 3A: Stage / Salt — Music Copyright Infrastructure

**Role progression:**
- Data Engineering Intern → Junior Data Engineer → Forward Deployed Engineer → Engineering Lead
- Nov 2022 – Nov 2025 (~3 years)
- Companies: TeleSoftas → Stage → Salt → Connex (all related entities in the music data space)

**Narrative text:**

I joined a music-tech company as a data engineering intern when I was 19 and still in my first year of university. Over the next three years I worked my way up to Engineering Lead.

The company builds infrastructure for music copyright — matching songs to their rightful owners so royalties get paid correctly. It sounds straightforward, but the data is a mess: hundreds of proprietary formats from labels, publishers, and collecting societies, each with their own schemas, edge cases, and legacy quirks.

**What I shipped:**

- **Customer onboarding, 1 → 4:** When I arrived, we had one customer. I was the engineer who onboarded Concord Publishing, MLC (the Mechanical Licensing Collective), PPL (Phonographic Performance Limited), and helped build on the Connex platform for Universal Music. Each customer meant learning an entirely new domain, building custom matching logic, and delivering under pressure.

- **The PPL overnight build:** When PPL came in for a proof-of-concept, I built an NLP-based classifier overnight — stayed up through the night and demoed it at 9am the next morning. We won the deal. **[NEEDS CONFIRMATION — is this story accurate? Adjust details if needed]**

- **AI copyright agents:** I designed and built LLM-driven copyright verification agents using RAG pipelines and multi-step reasoning. These agents achieve near-human accuracy on complex copyright matching tasks that previously required weeks of manual verification by domain experts.

- **Platform v2:** Led the team that redesigned the entire metadata-matching platform from scratch. The new architecture lets us deploy a proof-of-concept environment for a new customer in hours instead of weeks.

- **Royalty statement AI:** Built an AI-driven system that ingests hundreds of highly proprietary royalty statement formats (from labels, publishers, CMOs) and unifies them into a single schema — removing a major operational bottleneck.

- **AI-native culture shift:** Drove the org's shift toward AI-native development. Ran company-wide workshops on agent-driven engineering, coached teams on repo restructuring patterns, and delivered measurable productivity gains across both Stage and Salt.

**Tech used:** Python, TypeScript, Snowflake, Postgres, AWS (Lambda, Step Functions, S3), FastAPI, LangChain, LangGraph, Docker, Kubernetes, Terraform, Dagster

**Company links:**
- Stage: [NEEDS CONFIRMATION — URL]
- Salt: [NEEDS CONFIRMATION — URL]
- Connex: [NEEDS CONFIRMATION — URL]

---

### 3B: Here Comes Another Bubble

**Tagline:** Build your AI startup. Try not to die.

**URL:** [herecomesanotherbubble.com](https://herecomesanotherbubble.com)

**Narrative text:**

A satirical browser game where you play as an AI startup founder navigating Silicon Valley. You hire engineers, ship features, raise funding rounds, and desperately try to IPO before the bubble pops and takes your valuation with it. Named after the 2007 song about the Web 2.0 bubble.

The game features 5 founder archetypes (Technical Hacker, Visionary Hustler, Balanced Generalist, Ex-BigTech Corporate Refugee, Academic Researcher), 7 market segments with distinct economics, 100+ randomized events, and a Bubble Index that inflates valuations on the way up and wipes them out on the way down. It has a deliberately skeuomorphic Web 2.0 aesthetic — glossy buttons, layered shadows, and a design that looks like it was built in 2007, on purpose.

**Tech:** React 19, TypeScript, Zustand, Tailwind CSS, Vite, Vitest (320 tests)

**Contributors:** Built with Paulius Dovidaitis.

**Why it matters:** Ships as a complete product. Shows personality, humor, and range beyond "serious" engineering work.

---

### 3C: COVID Canteen System

**Narrative text:**

During COVID lockdowns, students at my high school couldn't leave their classrooms to get food. I built a food ordering system that let 800 students order meals from their phones — a real system solving a real problem, built while I was still in school.

**[NEEDS CONFIRMATION — more details? What tech? Was it a web app? Mobile? How long did it take? Is it still running?]**

---

### 3D: Options Probability Heatmap

**Narrative text:**

A financial visualization tool that shows where a stock price is likely to be at each options expiration date. It pulls real-time options data from Yahoo Finance, calculates implied volatility using the Black-Scholes model, generates probability distributions using a log-normal model, and renders everything as an interactive heatmap.

**Tech:** React 18, TypeScript, D3.js v7, Vite, Express.js (API proxy), Vitest (27 tests)

**URL:** [NEEDS CONFIRMATION — is it deployed anywhere?]

---

### 3E: OracleGen — AI Test Oracle Generation

**Narrative text:**

A multi-agent system that automatically generates test oracles — the "expected behavior" part of a test case — for code. Built as a university research project using LangGraph.

The system uses 6 specialized agents: a tentative oracle generator, a requirement engineer, a panel of 4 expert reviewers (specification expert, edge case specialist, functional validator, algorithmic analyst), a curator, and a self-refinement agent. Oracles are validated by actually executing them against generated implementations. If they fail, the system automatically refines them.

Evaluated on the LiveCodeBench dataset. Achieves 85% task-level accuracy (Pass@1).

**Tech:** Python, LangGraph, LangChain, Streamlit (dashboard), OpenAI API

---

### 3F: AI Adaptive Learning Platform

**Narrative text:**

An AI-powered educational platform built for a Human-AI Interaction coursework at King's College London. Upload PDF course materials and the system automatically parses them, generates summaries, creates adaptive quizzes, provides an AI tutor chatbot that gives hints without revealing answers, and even generates short educational videos with text-to-speech and synchronized subtitles.

**Tech:** Python, FastAPI, React 18, TypeScript, Mistral AI, LlamaCloud/LlamaParse, ElevenLabs (TTS), FFmpeg, Zustand, Vite

---

### 3G: Hackathon Projects

#### Codex 2022 — Riga, Latvia (WINNER)

**Project:** Parcel Tracking System for Latvian Post

Built an MVP hardware + software solution for tracking post parcels using BLE-equipped chips with distinct MAC addresses. The software side included an Android app for carriers to detect and update package locations, and a web app for end users to track deliveries in real time.

**Tech:** Android (Kotlin/Java), Flask (Python), BLE hardware

#### Junction 2022 — Helsinki, Finland

**Project:** Smart Energy Manager

At one of Europe's largest on-site hackathons, our team built a proof-of-concept for predicting and visualizing total electricity costs and potential savings per device for Finnish households and businesses, based on real-time variable energy price predictions. The app also suggests optimal electricity usage schedules for each device.

**Tech:** [NEEDS CONFIRMATION — what stack was used?]

**Team:** [NEEDS CONFIRMATION — team members?]

---

### 3H: Robotics — 2016 to Present

**Narrative text:**

I started programming robots when I was 12 — LEGO Mindstorms, FIRST LEGO League competitions. For four years I was the head programmer of my FLL team. We won the national championship every year from 2016 to 2019, and in 2019 we became FLL World Champions at the Championship in Detroit.

Since then I've been mentoring younger teams. I've coached students to FLL and FTC world championships, teaching them PID controllers, accelerometer-based robot positioning, and computer vision.

**[NEEDS CONFIRMATION — what specific teams have you mentored to worlds? Any names/details you'd want to include?]**

---

### 3I: Other Projects (lighter mentions)

These can be a simple grid or list with one-liner descriptions. Not full narratives.

| Project | Description | Link |
|---------|-------------|------|
| **Hazelnut Farmer Simulator** | A tile-based farming game — plant nut trees, harvest them, expand your land, build bridges. Deployed and playable. | [hazelnut-farmer-sim.vercel.app](https://hazelnut-farmer-sim.vercel.app/) |
| **Knowledge Manager** | A decentralized organizational knowledge management agent — event-driven architecture pulling from GitHub, Slack, Email, Confluence, Notion to give each employee a personalized knowledge agent. | Private |
| **KCL Year 3 Revision Notes** | Comprehensive LaTeX revision notes for 6 final-year AI modules. Published on GitHub, used by classmates. | Public repo |

**[NEEDS CONFIRMATION — include Tiro (Swift iOS app), ShortFormAI, personal-runway calculator, or upwork freelance work?]**

---

## SECTION 4: TRACK RECORD

### Competition Wins

| Year | Achievement | Location |
|------|-------------|----------|
| 2019 | **FLL World Champion** — 1st Place Champion's Award, FIRST LEGO League World Championship | Detroit, USA |
| 2018 | **FLL World 2nd Place** — Strategy and Innovation Award, FIRST LEGO League World Championship | Detroit, USA |
| 2019 | **National FLL Champion** — 1st Place Champion's Award (4th consecutive year: 2016, 2017, 2018, 2019) | Lithuania |
| 2022 | **Codex Hackathon Winner** | Riga, Latvia |
| 2022 | **Junction Hackathon** — participant at one of Europe's largest on-site hackathons | Helsinki, Finland |

### Science Olympiads

| Year | Achievement | Location |
|------|-------------|----------|
| 2018 | **IJSO Bronze Medal** — International Junior Science Olympiad | Gaborone, Botswana |
| 2019 | **National Chemistry Olympiad — 3rd Place** | Lithuania |

### Academic

| Detail | Value |
|--------|-------|
| **Degree** | BSc Artificial Intelligence, King's College London (2023–2026) |
| **IB Score** | 43/45 |
| **IB Highlights** | Computer Science HL: 7, English B HL: 7, Maths AA HL: 6, Physics SL: 7, Lithuanian Lit SL: 7, Economics SL: 6 |
| **High School** | Kaunas Jesuit High School (2014–2022) |

### Background notes

- FLL = FIRST LEGO League — a global robotics competition for students aged 9-16. Teams design, build, and program autonomous robots, plus complete a research project. National → regional → world championship pipeline.
- Champion's Award = the top overall award at FLL, given to the team that best embodies the program's values across robot performance, project, and core values.
- IJSO = International Junior Science Olympiad — a multi-disciplinary science competition (physics, chemistry, biology) for students under 16. Bronze medal = top third of competing countries.
- Junction = Europe's largest hackathon, held annually in Helsinki. 1500+ participants.
- Codex = A hackathon in Riga, Latvia.

---

## SECTION 5: ABOUT

### Text

I'm Lithuanian, grew up in Kaunas, and moved to London in 2023 for university. I've been programming since I was 12 — started with LEGO Mindstorms robots, moved to competitive robotics, then into data engineering and AI.

I worked full-time as an engineer through most of university, starting as an intern and ending up leading a team. I like hard problems, tight deadlines, and building things that actually get used by real people.

When I'm not coding, I mentor younger robotics teams — a few of them have made it to world championships.

**[NEEDS CONFIRMATION — anything else to add? Hobbies, interests, guitar/music mentioned in brainstorm? Keep it short.]**

---

## SECTION 6: FOOTER / LINKS

### Links to include

- **Email:** rokas.tarasevicius@gmail.com
- **LinkedIn:** [NEEDS CONFIRMATION — URL]
- **X / Twitter:** [NEEDS CONFIRMATION — handle]
- **herecomesanotherbubble.com** (deployed project)
- **hazelnut-farmer-sim.vercel.app** (deployed project)

### Links explicitly NOT included

- GitHub (intentional — curated portfolio tells a better story)
- STEVE / steveai.pm (omitted for now per instruction)
- YC or accelerator signals

---

## SECTION 7: TECHNICAL SKILLS

_Can be a dedicated section, a sidebar, or woven into project descriptions. Included here for completeness._

### By category

**Languages:** Python, TypeScript, JavaScript, SQL, Java, Swift, LaTeX

**AI / ML:** LangChain, LangGraph, RAG pipelines, PyTorch, TensorFlow, Pandas, Spark, Mistral AI, OpenAI API, LlamaCloud/LlamaParse, ElevenLabs

**Data:** Snowflake, Postgres, Dagster, ETL/ELT pipelines

**Cloud & Infra:** AWS (Lambda, Step Functions, S3), GCP, Docker, Kubernetes, Terraform, CI/CD

**Web:** React (18/19), Next.js, Vite, FastAPI, Flask, Express.js, GraphQL, Zustand, Tailwind CSS, D3.js, CSS Modules

**Tools:** Git, Cursor, Scrum/Agile

---

## SECTION 8: FULL TIMELINE (for reference, not necessarily displayed)

| Period | Role / Activity |
|--------|-----------------|
| 2014–2022 | Kaunas Jesuit High School, IB programme (43/45) |
| 2016–2019 | FLL head programmer — 4x national champion, world champion 2019 |
| 2018 | IJSO Bronze Medal, Botswana |
| 2019 | National Chemistry Olympiad 3rd place |
| 2020–present | Mentoring FLL/FTC robotics teams |
| Sep 2022 – Feb 2023 | Data Engineering Intern @ TeleSoftas |
| Mar 2023 – Sep 2023 | Junior Data Engineer @ TeleSoftas |
| Sep 2023 – present | BSc Artificial Intelligence @ King's College London |
| Nov 2022 | Codex 2022 hackathon winner (Riga) |
| Nov 2022 | Junction 2022 hackathon (Helsinki) |
| Nov 2023 – Jun 2025 | Forward Deployed Engineer @ Stage / Salt / Connex |
| Jul 2025 – Nov 2025 | Engineering Lead @ Stage / Salt |
| ~2020 | COVID canteen system for 800 students |
| 2025–2026 | Various side projects (Here Comes Another Bubble, Options Heatmap, OracleGen, etc.) |
| 2026 | Graduating KCL, exploring what's next |

---

## DESIGN DIRECTION (for the developer)

- **Single-page site.** Scroll-based sections, not multi-page routing.
- **Narrative-driven.** Stories and paragraphs, not resume bullet points. The PPL overnight story communicates more than "Forward Deployed Engineer, 2022–2024."
- **Clean, fast, typographic.** Well-written text on a minimal layout beats fancy animations. Think personal blog aesthetic, not SaaS landing page.
- **Age is an asset.** The fact that a 22-year-old has this track record is unusual. The site should let that speak for itself without being explicit about it.
- **Easy to update.** The "Currently" section and project list should be trivially editable so the site stays alive.
- **No GitHub links.** The curated portfolio is the point. Raw repos don't tell the story.
- **Mobile-first.** Most people will open this from a link in a Twitter bio or application form on their phone.
- **Dark mode optional.** [NEEDS CONFIRMATION — preference?]
- **Domain:** [NEEDS CONFIRMATION — what domain? rokastarasevicius.com? something else?]
- **Deployment:** Vercel or Cloudflare Pages (fast, free, easy).
