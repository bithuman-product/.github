# bitHuman

Build AI avatars with real-time lip sync — running on your own hardware. Two models (**Essence** for CPU-only `.imx` avatars, **Expression** for AI-generated facial animation) and three runtime surfaces (**Python**, **Apple Silicon Swift**, **Cloud REST API**). Full product docs at **[docs.bithuman.ai](https://docs.bithuman.ai)**.

This page is the index for the public source repos in this org. Pick the row that matches what you're building.

## Where to start

| I want to… | Go to | Notes |
|---|---|---|
| Browse runnable examples & docs source | **[bithuman-examples](https://github.com/bithuman-product/bithuman-examples)** | Python + Swift examples, LiveKit plugin samples, self-hosted GPU recipes. Mintlify source for docs.bithuman.ai. |
| Embed the on-device Swift SDK | **[bithuman-kit-public](https://github.com/bithuman-product/bithuman-kit-public)** | Public SwiftPM binary package — `import bitHumanKit`. Mac M3+ / iPad M4+ / iPhone 16 Pro+. |
| Run a working Mac / iPad / iPhone reference app | **[bithuman-apps](https://github.com/bithuman-product/bithuman-apps)** | Source-available example apps that consume the SDK. Clone, build, talk to an avatar in 30 seconds. |
| Install the Mac CLI / desktop app | **[homebrew-bithuman](https://github.com/bithuman-product/homebrew-bithuman)** | `brew install bithuman-product/bithuman/bithuman-cli` — voice + video chat from Terminal. |
| Install the Python SDK | [PyPI: `bithuman`](https://pypi.org/project/bithuman/) · [bithuman-python-sdk-public](https://github.com/bithuman-product/bithuman-python-sdk-public) | `pip install bithuman`. Source is private (signing material is baked in); the public repo hosts the README, changelog, and issue tracker. |
| Use the cloud platform (REST API) | [docs.bithuman.ai/platform](https://docs.bithuman.ai/platform) | No SDK or local runtime needed — agent management over HTTPS. |

## How the pieces fit

```
                       docs.bithuman.ai  ←  bithuman-examples (Mintlify source + runnable code)
                              │
        ┌─────────────────────┼──────────────────────────┐
        │                     │                          │
   Python SDK            Swift SDK                  Cloud REST API
        │                     │
   pip install         brew install bithuman-cli
   bithuman                   │
   (private source            │
    → PyPI wheels)      ┌─────┴──────┐
                        │            │
                  bithuman-kit  bithuman-apps
                  -public       (reference Mac /
                  (binary       iPad / iPhone apps
                  SwiftPM       consuming the SDK)
                  package)
```

## Two models, briefly

- **Essence** — CPU-only, pre-built `.imx` model from a photo or video. Gestures, animal mode, full body. No idle timeout.
- **Expression** — AI-generated facial animation from any face image. Runs on NVIDIA GPU (cloud or self-hosted) or on-device Apple Silicon M3+.

Comparison: [docs.bithuman.ai/getting-started/models](https://docs.bithuman.ai/getting-started/models).

## Status & support

- **Releases**: see each repo's [Releases page](https://github.com/bithuman-product/bithuman-kit-public/releases).
- **Issues / questions**: file in the repo closest to the problem. For the Python SDK, use [bithuman-python-sdk-public/issues](https://github.com/bithuman-product/bithuman-python-sdk-public/issues) (the SDK source is private; the public repo is the issue + changelog tracker).
- **Status & updates**: [bithuman.ai](https://www.bithuman.ai) · [@bithumanAI](https://x.com/bithumanAI).

## License

Each repo carries its own license — most are MIT or source-available with a build-and-run grant. See the `LICENSE` file in each repo.
