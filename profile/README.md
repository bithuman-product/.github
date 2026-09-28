<h1 align="center">bitHuman</h1>

<p align="center">
  <b>Real-time AI avatars that run on the device — in your app, in your building, or in our cloud.</b><br/>
  Send speech in, get a lip-synced talking face out: a photoreal person with Essence 2, or any character with Expression 2.
</p>

<p align="center">
  <a href="https://docs.bithuman.ai/start"><b>Start here</b></a> ·
  <a href="https://docs.bithuman.ai/platforms">Platforms</a> ·
  <a href="https://github.com/bithuman-product/bithuman-examples">Examples</a> ·
  <a href="https://docs.bithuman.ai">Docs</a> ·
  <a href="https://www.bithuman.ai">bithuman.ai</a>
</p>

---

## Where it runs

The avatar **renders** on iPhone, iPad, Mac, Android, a Linux PC (no GPU needed) or in a browser with WebGPU, on your own servers, or in the bitHuman cloud. The **conversation** — speech recognition, language model and voice — runs where you choose: your own services, bitHuman's managed agent, or, from the CLI, a local conversation brain on your Mac or Linux machine.

The phone SDKs render the face only: your app passes in 16 kHz speech from any voice stack and draws the frames. When the avatar renders on your device and you use your own voice and language services, bitHuman receives usage metering only — never audio, video or conversation text. Every published configuration is measured faster than real time: [docs.bithuman.ai/performance](https://docs.bithuman.ai/performance).

From 12 October 2026, API and SDK use requires the Creator plan or higher. Sessions bill active session time, talking or idle, to the second: [pricing](https://docs.bithuman.ai/pricing).

## Get started

| You want to… | Use | Docs |
|---|---|---|
| Run a live avatar from the terminal, no code | **CLI** — `curl -fsSL https://install.bithuman.ai \| sh` (macOS, Linux) | [CLI](https://docs.bithuman.ai/platforms/cli) |
| Render frames or MP4s from your own code | **Python** — `pip install bithuman` (macOS, Linux) | [Python](https://docs.bithuman.ai/platforms/python) |
| Add an avatar to an iPhone, iPad or Mac app | **Apple** — the Swift package from [`homebrew-bithuman`](https://github.com/bithuman-product/homebrew-bithuman): `Expression2`, `Essence2Kit` | [iOS & iPadOS](https://docs.bithuman.ai/platforms/ios) · [macOS](https://docs.bithuman.ai/platforms/macos) |
| Add an avatar to an Android app | **Android** — Maven Central: `ai.bithuman:expression2-android`, `ai.bithuman:essence2-android` | [Android](https://docs.bithuman.ai/platforms/android) |
| Put an avatar on a website | **Web** — one iframe on any page | [Web](https://docs.bithuman.ai/platforms/web) |
| Give a LiveKit voice agent a face | **LiveKit** — `livekit-plugins-bithuman` | [LiveKit](https://docs.bithuman.ai/platforms/livekit) |
| Drive bitHuman from an AI assistant | **MCP** — `bithuman mcp` | [MCP](https://docs.bithuman.ai/build/mcp) |
| Call it from any backend | **REST API** | [REST](https://docs.bithuman.ai/platforms/rest) |

Current versions of every package: [docs.bithuman.ai/versions.json](https://docs.bithuman.ai/versions.json). For AI coding agents: [llms.txt](https://docs.bithuman.ai/llms.txt).

## Repositories

| Repo | What it is |
|---|---|
| [**bithuman-examples**](https://github.com/bithuman-product/bithuman-examples) | Working examples: iOS, Android, macOS, web (Next.js), Python, REST and CLI. |
| [**homebrew-bithuman**](https://github.com/bithuman-product/homebrew-bithuman) | The Apple SDK (Swift Package Manager) and the Homebrew tap for the bitHuman CLI. |
| [**public-docs**](https://github.com/bithuman-product/public-docs) | Source for [docs.bithuman.ai](https://docs.bithuman.ai). |

## Community and support

- **Docs** — [docs.bithuman.ai](https://docs.bithuman.ai), starting at [`/start`](https://docs.bithuman.ai/start)
- **Questions** — the [Discord](https://discord.gg/ES953n7bPA)
- **Docs issues** — [public-docs/issues](https://github.com/bithuman-product/public-docs/issues)
- **Security reports** — [hello@bithuman.ai](mailto:hello@bithuman.ai)
- **Updates** — [bithuman.ai](https://www.bithuman.ai) · [@bithuman_ai](https://x.com/bithuman_ai) · [status](https://status.bithuman.ai)

Each repository carries its own `LICENSE` file.
