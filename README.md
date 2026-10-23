<!-- GitHub profile README | Vamsha Vardhan -->

<div align="center">

<img width="100%" src="./anime-banner.png" alt="Anime-inspired illustration of a developer building late into the night" />

Vamsha Vardhan
Developer · Open-source builder · Curious about the systems behind the product
I turn annoying, fragile developer problems into tools people can actually use.

GitHub · LinkedIn · npm · Devpost
</div>

🌙 About me
Hey, I’m Vamsha, a developer from India. I like building software, but I’m just as interested in the parts most people don’t see: the data pipeline behind an AI feature, the configuration that keeps a service from breaking, or the small tool that saves someone an hour of repetitive work.

I started with full-stack products and kept following the problems underneath them. That curiosity has taken me from visual browser automation to environment analysis, terminal tooling, and now Rust-powered web data infrastructure.

There’s a common thread in my work: take something unreliable or unnecessarily difficult, understand why it’s difficult, then make the better path feel obvious.
I’m not trying to collect technologies. I’m trying to build useful things, understand them deeply, and make them dependable enough that other people want to use them.

📖 My builder’s arc
Chapter	What I worked on	What it taught me
Build the product	Full-stack apps and ScrapeFlow, a visual browser automation platform	A product has to make the workflow understandable, not just make the code run.
Fix the friction	envguard and getgrabkit, small tools for common developer annoyances	A focused tool can save time every day when it has good defaults and clear feedback.
Build the foundation	Crawlingo, a Rust-powered web crawling and dataset engine	Data infrastructure needs speed, resilience, documentation, and a friendly developer experience.


⚔️ Featured projects
Crawlingo
My main open-source build: a Rust-powered web crawling and dataset engine for developers who need useful, structured data from the web without building a new scraping stack for every project.

Web pages change. Selectors break. Data arrives in formats that are awkward to use. Crawlingo is my attempt to bring those rough edges into one developer-friendly tool.
- Selector matching can use saved DOM fingerprints to help recover when a page changes.
- An async Rust core keeps the crawling engine efficient.
- SDKs are available for Python, Node.js/TypeScript, and Rust.
- Structured results can be written as JSON, CSV, or Parquet.
- Sessions, rate limits, monitoring, and change notifications support automated workflows.
What I’m learning by building it: performance is only one part of a good infrastructure tool. Good defaults, readable docs, clear errors, and a setup that doesn’t fight you matter just as much.

Repository · Documentation · npm package
// The goal: useful data, without a fragile pile of one-off scripts.
let result = Dataset::new("https://example.com", session)
    .with_field(DatasetField::new("title", "h1"))
    .build_async()
    .await?;
envguard
An offline environment-variable linter that looks at what a codebase actually reads, then checks that against the project’s environment configuration.
- Finds variables referenced in code but missing from the environment file.
- Flags keys that are configured but no longer used.
- Supports checks for values such as URLs, ports, and enums.
- Runs locally and in CI; it checks key names without printing secret values.
I like this project because its problem is small, common, and expensive when ignored. A missing variable can turn a clean deploy into a late-night debugging session; envguard makes that class of mistake easier to spot.

Repository · npm package
getgrabkit
A deterministic terminal UI for selecting files from a GitHub repository and downloading the useful subset. It grew from a practical developer annoyance: sometimes you need a few specific files from a repo, not another full checkout and a manual cleanup.

Repository · npm package
ScrapeFlow
An earlier full-stack product build: a visual workflow canvas for browser automation and web data extraction. It brings together drag-and-drop workflow design, browser actions, AI-assisted extraction, scheduling, and run history.

ScrapeFlow taught me to think beyond “does the code work?” A product also has to show what happened, protect credentials, and give the user a way to recover when a run fails.

Repository
🧭 How I like to build
Start with the friction. What is the actual pain? Who has it, and how often?

Understand the failure mode. Happy-path demos are easy. I want to know what happens with missing inputs, changing pages, invalid config, slow services, and unclear errors.

Choose the simplest useful design. I like thoughtful systems, not complexity for its own sake.

Make it usable by someone else. Good names, examples, docs, safe defaults, and actionable errors are part of the product.

Ship, listen, improve. Real use reveals what a local test can’t. I want my projects to get better through feedback, not just bigger through features.
notice a problem → understand the edge cases → build the smallest useful fix
                 → test it in the real world → document it → improve it
🎒 My engineering toolbox
These are technologies I’ve used across projects—not a claim to know every corner of every tool.
- Languages and systems: Rust Go Python TypeScript Java
- Product and backend: Next.js React Node.js PostgreSQL MongoDB Redis
- Build and ship: Docker AWS Linux GitHub Actions
🏆 A little proof of the reps
6×	400+	3
Hackathon wins	DSA problems solved	npm packages published


Hackathons taught me to move from an idea to a working system under pressure. Problem solving taught me to stay with a difficult bug or concept longer than is comfortable. Shipping packages is teaching me a different lesson: the work isn’t finished when it runs on my machine; it’s finished when someone else can install it, understand it, and get value from it.
🌌 Current quest
I’m putting most of my builder energy into Crawlingo: making the core more useful, making the SDK experience clearer, and learning what it takes for an ambitious open-source project to become dependable infrastructure.

I’m especially interested in the space where web data, automation, and AI systems meet. AI features are only as useful as the information and infrastructure behind them; I want to help build that foundation.
✉️ Let’s connect
I’m open to thoughtful conversations and collaborations around open source, developer tools, backend systems, web data, and AI infrastructure. If you find a rough edge in one of my projects, tell me. If you have an idea worth building, tell me that too.
<div align="center">


GitHub · LinkedIn · npm packages
Build useful things. Make them dependable. Let people decide if they’re good.
</div>
