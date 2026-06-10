# bitHuman

Real-time AI avatars with lip-synced video. Stream audio in, get a talking face out at 25 FPS — running on your hardware or ours.

Full product docs at **[docs.bithuman.ai](https://docs.bithuman.ai)**.

## Where to start

| You want to… | Start at | What you get |
|---|---|---|
| **Try it in 5 minutes** | [docs.bithuman.ai/getting-started/quickstart](https://docs.bithuman.ai/getting-started/quickstart) | `pip install bithuman` and run a working example end-to-end. |
| **Run runnable examples** | [bithuman-sdk-public](https://github.com/bithuman-product/bithuman-sdk-public) | Python, Swift, CLI, and REST examples plus integration recipes (LiveKit, Next.js, Java, Gradio, offline Mac). |
| **Embed the on-device Swift SDK** | [bithuman-sdk-public](https://github.com/bithuman-product/bithuman-sdk-public) | SwiftPM binary package — `import bitHumanKit`. Mac M3+ / iPad M4+ / iPhone 16 Pro+. |
| **Install the Mac CLI** | [homebrew-bithuman](https://github.com/bithuman-product/homebrew-bithuman) | `brew install bithuman-product/bithuman/bithuman-cli` — voice + video chat from Terminal, 100% on-device. |
| **Install the Python SDK** | [PyPI: bithuman](https://pypi.org/project/bithuman/) | `pip install bithuman`. Runs Essence avatars on any CPU (laptop, server, Raspberry Pi). |
| **Use the REST API** | [docs.bithuman.ai/api-reference](https://docs.bithuman.ai/api-reference) | No local runtime — manage avatars and sessions over HTTPS from any language. |
| **See a reference app** | [bithuman-sdk-public Examples](https://github.com/bithuman-product/bithuman-sdk-public/tree/main/Examples) | Runnable Python / Swift / CLI / REST examples that consume the SDK the same way any third-party app would. |

## Two avatar engines

| | **Essence** (start here) | **Expression** |
|---|---|---|
| **What it is** | Pre-built `.imx` file generated from a photo or video | Any face image, animated at runtime |
| **Hardware** | Any CPU — laptop, server, Raspberry Pi | NVIDIA GPU or Apple Silicon M3+ |
| **Best for** | Voice agents, kiosks, 24/7 displays, getting started | Apps where users supply their own face |

Comparison and pricing: [docs.bithuman.ai/getting-started/models](https://docs.bithuman.ai/getting-started/models).

## Status & support

- **Releases** — Swift SDK on [GitHub Releases](https://github.com/bithuman-product/bithuman-sdk-public/releases), Python SDK on [PyPI](https://pypi.org/project/bithuman/#history), CLI on the [Homebrew tap](https://github.com/bithuman-product/homebrew-bithuman/releases).
- **Issues & questions** — file in [bithuman-sdk-public/issues](https://github.com/bithuman-product/bithuman-sdk-public/issues) (covers both Swift and Python SDKs) or join the [Discord](https://discord.gg/ES953n7bPA).
- **Security reports** — email [hello@bithuman.ai](mailto:hello@bithuman.ai). See each repo's `SECURITY.md` for scope.
- **Status, updates, blog** — [bithuman.ai](https://www.bithuman.ai) · [@bithuman_ai](https://x.com/bithuman_ai).

## License

Each repo carries its own license — most are MIT or source-available with a build-and-run grant. See the `LICENSE` file in each repo.
