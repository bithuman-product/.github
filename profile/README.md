<!-- gitlab-migration: moved -->
> **bitHuman's repositories moved to GitLab: [gitlab.com/bithuman](https://gitlab.com/bithuman).**
> The repositories here are archived (read-only), stay readable and are no longer updated.
> Homebrew: `brew tap bithuman/bithuman https://gitlab.com/bithuman/sdk/homebrew-bithuman` (always with the URL). Docs: https://docs.bithuman.ai

<h1 align="center">bitHuman</h1>

<p align="center">
  <b>Real-time AI avatars that run on the device — in your app, in your building, or in our cloud.</b><br/>
  Send speech in, get a lip-synced talking face out: a photoreal person with Essence 2, or any character with Expression 2.
</p>

<p align="center">
  <a href="https://docs.bithuman.ai/start"><b>Start here</b></a> ·
  <a href="https://docs.bithuman.ai/platforms">Platforms</a> ·
  <a href="https://gitlab.com/bithuman/sdk/bithuman-examples">Examples</a> ·
  <a href="https://docs.bithuman.ai">Docs</a> ·
  <a href="https://www.bithuman.ai">bithuman.ai</a>
</p>

<p align="center">
  <a href="https://discord.gg/x3tMhJvX4X"><img alt="Discord" src="https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white"></a><br>
  Questions, demos and challenges: <a href="https://discord.gg/x3tMhJvX4X">join the bitHuman Discord</a>.
</p>

---

## Latest

- **Any character, live, rendered on the user's device.** Expression 2 animates any character from one portrait and renders it live on iPhone, iPad, Android, Mac, Linux or in a browser tab with WebGPU. [Read the news](https://docs.bithuman.ai/news/2026-09-29-any-character-live-on-device)
- **Faster than real time.** Every configuration we publish renders faster than real time, including 10-minute sustained runs on iPhone 15 and Samsung Galaxy S25+. [The numbers](https://docs.bithuman.ai/news/2026-09-29-faster-than-real-time)
- **For AI agents.** The bitHuman CLI includes an MCP server: `claude mcp add bithuman -- bithuman mcp`. [Claude & Cursor setup](https://docs.bithuman.ai/build/mcp)

Every announcement: [docs.bithuman.ai/news](https://docs.bithuman.ai/news) ([RSS](https://docs.bithuman.ai/news.xml)).

## Where it runs

The avatar **renders** on iPhone, iPad, Mac, Android, a Linux PC (no GPU needed) or in a browser with WebGPU, on your own servers, or in the bitHuman cloud. The **conversation** — speech recognition, language model and voice — runs where you choose: your own services, bitHuman's managed agent, or, from the CLI, a local conversation brain on your Mac or Linux machine.

The phone SDKs render the face only: your app passes in 16 kHz speech from any voice stack and draws the frames. When the avatar renders on your device and you use your own voice and language services, bitHuman receives usage metering only — never audio, video or conversation text. Every published configuration is measured faster than real time: [docs.bithuman.ai/performance](https://docs.bithuman.ai/performance).

From 12 October 2026, API and SDK use requires the Creator plan or higher. Sessions bill active session time, talking or idle, to the second: [pricing](https://docs.bithuman.ai/pricing).

## Get started

| You want to… | Use | Docs |
|---|---|---|
| Run a live avatar from the terminal, no code | **CLI** — `curl -fsSL https://install.bithuman.ai \| sh` (macOS, Linux) | [CLI](https://docs.bithuman.ai/platforms/cli) |
| Render frames or MP4s from your own code | **Python** — `pip install bithuman` (macOS, Linux) | [Python](https://docs.bithuman.ai/platforms/python) |
| Add an avatar to an iPhone, iPad or Mac app | **Apple** — the Swift package [`bithuman-swift`](https://gitlab.com/bithuman/sdk/bithuman-swift): `.package(url: "https://gitlab.com/bithuman/sdk/bithuman-swift", from: "3.0.0")` (the same URL resolves every earlier release, 2.x included) | [iOS & iPadOS](https://docs.bithuman.ai/platforms/ios) · [macOS](https://docs.bithuman.ai/platforms/macos) |
| Add an avatar to an Android app | **Android** — `ai.bithuman:bithuman-android` with the `ai.bithuman:bithuman-bom`, from [maven.bithuman.ai](https://maven.bithuman.ai) ([guide](https://docs.bithuman.ai/platforms/android)) | [Android](https://docs.bithuman.ai/platforms/android) |
| Put an avatar on a website | **Web** — one iframe on any page | [Web](https://docs.bithuman.ai/platforms/web) |
| Give a LiveKit voice agent a face | **LiveKit** — `livekit-plugins-bithuman` | [LiveKit](https://docs.bithuman.ai/platforms/livekit) |
| Drive bitHuman from an AI assistant | **MCP** — `bithuman mcp` | [MCP](https://docs.bithuman.ai/build/mcp) |
| Call it from any backend | **REST API** | [REST](https://docs.bithuman.ai/platforms/rest) |

Current versions of every package: [docs.bithuman.ai/versions.json](https://docs.bithuman.ai/versions.json). For AI coding agents: [llms.txt](https://docs.bithuman.ai/llms.txt).

## Repositories

| Repo | What it is |
|---|---|
| [**bithuman-examples**](https://gitlab.com/bithuman/sdk/bithuman-examples) | Working examples: iOS, Android, macOS, web (Next.js), Python, REST and CLI. |
| [**bithuman-swift**](https://gitlab.com/bithuman/sdk/bithuman-swift) | The Swift package for iPhone, iPad and Mac (every release). |
| [**bithuman-flutter**](https://gitlab.com/bithuman/sdk/bithuman-flutter) | The Flutter plugin, pub.dev `bithuman` (3.0 and later). |
| [**homebrew-bithuman**](https://gitlab.com/bithuman/sdk/homebrew-bithuman) | The Homebrew tap and the installers for the bitHuman CLI. |
| [**public-docs**](https://gitlab.com/bithuman/docs/public-docs) | Source for [docs.bithuman.ai](https://docs.bithuman.ai). |

## Community and support

- **Docs** — [docs.bithuman.ai](https://docs.bithuman.ai), starting at [`/start`](https://docs.bithuman.ai/start)
- **Questions, demos and challenges** — the [bitHuman Discord](https://discord.gg/x3tMhJvX4X)
- **Docs issues** — [public-docs/issues](https://gitlab.com/bithuman/docs/public-docs/-/issues)
- **Security reports** — [hello@bithuman.ai](mailto:hello@bithuman.ai)
- **Updates** — [bithuman.ai](https://www.bithuman.ai) · [@bithuman_ai](https://x.com/bithuman_ai) · [status](https://status.bithuman.ai)

Each repository carries its own `LICENSE` file.
