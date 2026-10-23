<!-- GitHub profile README | Vamsha Vardhan -->

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=250&color=0:080B18,48:111827,100:2563EB&text=VAMSHA%20VARDHAN&fontColor=FFFFFF&fontSize=60&fontAlignY=38&desc=I%20build%20the%20tools%20behind%20better%20software.&descAlignY=58&descSize=18&animation=fadeIn" alt="Vamsha Vardhan — developer and open-source builder" />

### Developer · Open-source builder · Curious about the systems behind the product

**I turn annoying, fragile developer problems into tools people can actually use.**

<a href="https://github.com/Vamshavardhan50"><img src="https://img.shields.io/badge/GitHub-@Vamshavardhan50-111827?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://www.linkedin.com/in/vamshavardhan50"><img src="https://img.shields.io/badge/LinkedIn-Let's_connect-2563EB?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://www.npmjs.com/~vamsha50"><img src="https://img.shields.io/badge/npm-vamsha50-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm" /></a>
<a href="https://devpost.com/chintha-vamshavardhan50"><img src="https://img.shields.io/badge/Devpost-Hackathon_work-003E54?style=for-the-badge&logo=devpost&logoColor=white" alt="Devpost" /></a>

<br/><br/>
<img src="https://komarev.com/ghpvc/?username=Vamshavardhan50&style=flat-square&color=2563EB&label=profile+views" alt="Profile views" />

</div>

---

## Hey, I’m Vamsha.

I’m a developer from India who likes building software—and is just as interested in the parts most people don’t see: the data pipeline behind an AI feature, the configuration that keeps a service from breaking, or the small tool that saves a developer an hour of repetitive work.

I started with full-stack products and kept following the problems underneath them. That curiosity has taken me from visual browser automation to environment analysis, terminal tooling, and now Rust-powered web data infrastructure.

There’s a common thread in the things I make: **take something unreliable or unnecessarily difficult, understand why it’s difficult, then make the better path feel obvious.**

> I’m not trying to collect technologies. I’m trying to build useful things, understand them deeply, and make them dependable enough that other people want to use them.

## The work that best represents me

### [Crawlingo](https://github.com/Vamshavardhan50/crawlingo) — making web data less fragile

**Crawlingo is my main open-source build:** a Rust-powered web crawling and dataset engine for developers who need useful, structured data from the web—without building a new scraping stack for every project.

Web pages change. Selectors break. Data arrives in formats that are awkward to use. Crawlingo is my attempt to bring those rough edges into one developer-friendly tool.

- **A resilient extraction approach:** selector matching can use saved DOM fingerprints to help recover when a page changes.
- **A fast systems core:** async Rust for the crawling engine, with a focus on keeping the core efficient.
- **SDKs for more than one ecosystem:** Python, Node.js/TypeScript, and Rust interfaces.
- **Data that can move into real workflows:** structured results with JSON, CSV, and Parquet output.
- **Automation beyond one request:** configurable sessions, rate limits, monitoring, and change notifications.

What I’m learning by building it: performance is only one part of a good infrastructure tool. Good defaults, readable docs, clear errors, and a setup that doesn’t fight you matter just as much.

[![Explore Crawlingo](https://img.shields.io/badge/Explore_Crawlingo-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vamshavardhan50/crawlingo)
[![Crawlingo docs](https://img.shields.io/badge/Read_the_docs-2563EB?style=for-the-badge&logo=readthedocs&logoColor=white)](https://crawlingo-docs.vercel.app/)
[![Crawlingo on npm](https://img.shields.io/badge/Node.js_SDK-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/package/crawlingo)

```rust
// The goal: useful data, without a fragile pile of one-off scripts.
let result = Dataset::new("https://example.com", session)
    .with_field(DatasetField::new("title", "h1"))
    .build_async()
    .await?;
```

### [envguard](https://github.com/Vamshavardhan50/envguard) — catch configuration drift before it ships

**An offline environment-variable linter** that looks at what a codebase actually reads, then checks that against the project’s environment configuration.

- Finds variables referenced in code but missing from the environment file.
- Flags keys that are configured but no longer used.
- Supports configurable checks for values such as URLs, ports, and enums.
- Runs locally and in CI; it checks key names without printing secret values.

I like this project because its problem is small, common, and expensive when ignored. A missing variable can turn a clean deploy into a late-night debugging session; `envguard` makes that class of mistake easier to spot.

[![Explore envguard](https://img.shields.io/badge/Explore_envguard-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vamshavardhan50/envguard)
[![envguard on npm](https://img.shields.io/badge/Install_with_npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/package/envguard-bin)

### [getgrabkit](https://github.com/Vamshavardhan50/getgrabkit) — get just the files you need

A deterministic terminal UI for selecting files from a GitHub repository and downloading the useful subset. It’s built around a practical developer annoyance: sometimes you need a few specific files from a repo, not another full checkout and a manual cleanup.

[![Explore getgrabkit](https://img.shields.io/badge/Explore_getgrabkit-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vamshavardhan50/getgrabkit)
[![getgrabkit on npm](https://img.shields.io/badge/Install_with_npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/package/getgrabkit)

### [ScrapeFlow](https://github.com/Vamshavardhan50/ScrapeFlow) — product thinking meets automation

An earlier full-stack product build: a visual workflow canvas for browser automation and web data extraction. It brings together drag-and-drop workflow design, browser actions, AI-assisted extraction, scheduling, and run history.

ScrapeFlow taught me to think beyond “does the code work?” A product also has to make the workflow understandable, show what happened, protect credentials, and give the user a way to recover when a run fails.

[![Explore ScrapeFlow](https://img.shields.io/badge/Explore_ScrapeFlow-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vamshavardhan50/ScrapeFlow)

## A pattern across my projects

| Problem I notice | What I build | What I care about |
|---|---|---|
| Web extraction breaks as pages change | **Crawlingo** | Resilience, performance, useful data |
| App configuration drifts away from the code | **envguard** | Reliability, privacy, clear feedback |
| Getting a few files from a repo takes too many steps | **getgrabkit** | Developer experience, sensible defaults |
| Browser workflows are hard to build and inspect | **ScrapeFlow** | Product clarity, automation, observability |

Different projects, same instinct: **remove friction without hiding how the system works.**

## A little proof of the reps

<div align="center">

| 🏆 **6×** | 🧠 **400+** | 📦 **3** |
|:---:|:---:|:---:|
| Hackathon wins | DSA problems solved | npm packages published |

</div>

Hackathons taught me to move from an idea to a working system under pressure. Problem solving taught me to stay with a difficult bug or concept longer than is comfortable. Shipping packages is teaching me a different lesson: the work isn’t finished when it runs on my machine—it’s finished when someone else can install it, understand it, and get value from it.

## How I like to build

**Start with the friction.** What is the actual pain? Who has it, and how often?

**Understand the failure mode.** Happy-path demos are easy. I want to know what happens with missing inputs, changing pages, invalid config, slow services, and unclear errors.

**Choose the simplest useful design.** I like thoughtful systems, not complexity for its own sake.

**Make it usable by someone else.** Good names, examples, docs, safe defaults, and actionable errors are part of the product.

**Ship, listen, improve.** Real use reveals what a local test can’t. I want my projects to get better through feedback, not just bigger through features.

```text
notice a problem → understand the edge cases → build the smallest useful fix
                 → test it in the real world → document it → improve it
```

## My engineering toolbox

These are technologies I’ve used across projects—not a claim to know every corner of every tool.

**Languages & systems**

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

**Product & backend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Build & ship**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=111827)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

## What I’m focused on now

I’m putting most of my builder energy into **Crawlingo**: making the core more useful, making the SDK experience clearer, and learning what it takes for an ambitious open-source project to become genuinely dependable infrastructure.

I’m especially interested in the space where **web data, automation, and AI systems** meet. AI features are only as useful as the information and infrastructure behind them; I want to help build that foundation.

## GitHub, at a glance

<div align="center">

<img height="175" src="https://github-readme-stats.vercel.app/api?username=Vamshavardhan50&show_icons=true&theme=transparent&hide_border=true&rank_icon=github&title_color=60A5FA&text_color=94A3B8&icon_color=22D3EE" alt="Vamsha Vardhan's GitHub stats" />
<img height="175" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vamshavardhan50&layout=compact&theme=transparent&hide_border=true&langs_count=8&title_color=60A5FA&text_color=94A3B8" alt="Most used languages" />

<img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=Vamshavardhan50&bg_color=transparent&color=94A3B8&line=3B82F6&point=22D3EE&area=true&area_color=2563EB&hide_border=true" alt="GitHub contribution activity" />

</div>

## If any of this sounds like your kind of work

I’m open to thoughtful conversations and collaborations around open source, developer tools, backend systems, web data, and AI infrastructure. If you find a rough edge in one of my projects, tell me. If you have an idea worth building, tell me that too.

<div align="center">

[![Connect on LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-2563EB?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vamshavardhan50)
[![Follow on GitHub](https://img.shields.io/badge/Follow_on_GitHub-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vamshavardhan50)
[![See my npm packages](https://img.shields.io/badge/See_my_npm_packages-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/~vamsha50)

### Build useful things. Make them dependable. Let people decide if they’re good.

<sub>Vamsha Vardhan · India 🇮🇳</sub>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:2563EB,55:111827,100:080B18" alt="Footer" />

</div>
