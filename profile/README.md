# bitHuman

Build AI avatars with real-time lip sync — running on your own hardware. Two avatar engines (**Essence** for CPU-only `.imx` avatars, **Expression** for AI-generated facial animation) and three runtime surfaces (**Python**, **Apple Silicon Swift**, **Cloud REST API**). Full product docs at **[docs.bithuman.ai](https://docs.bithuman.ai)**.

This page is the index for the public source repos in this org. Pick the row that matches what you're building.

## Where to start

| I want to… | Go to | Notes |
|---|---|---|
| Browse runnable examples & docs source | **[bithuman-sdk-public](https://github.com/bithuman-product/bithuman-sdk-public)** | Python, Swift, CLI, and REST examples (`Examples/`) plus the Mintlify source for [docs.bithuman.ai](https://docs.bithuman.ai) (`docs/`). |
| Embed the on-device Swift SDK | **[bithuman-sdk-public](https://github.com/bithuman-product/bithuman-sdk-public)** | Public SwiftPM binary package — `import bitHumanKit`. Mac M3+ / iPad M4+ / iPhone 16 Pro+. |
| Run a working Mac / iPad / iPhone / CLI reference | **[bithuman-apps](https://github.com/bithuman-product/bithuman-apps)** | Source-available reference apps + the canonical Swift SDK source (under `SDK/`) they consume. Clone, build, talk to an avatar in 30 seconds. |
| Install the Mac CLI | **[homebrew-bithuman](https://github.com/bithuman-product/homebrew-bithuman)** | `brew install bithuman-product/bithuman/bithuman-cli` — voice + video chat from Terminal. |
| Install the Python SDK | [PyPI: `bithuman`](https://pypi.org/project/bithuman/) | `pip install bithuman`. SDK source is private (signing material is baked in); issues + changelog are tracked in [bithuman-sdk-public](https://github.com/bithuman-product/bithuman-sdk-public). |
| Use the cloud platform (REST API) | [docs.bithuman.ai](https://docs.bithuman.ai) | No SDK or local runtime needed — agent management over HTTPS. |

## How the pieces fit

```
            docs.bithuman.ai  ←  bithuman-sdk-public/docs/  (Mintlify source)
                     │
                     │  examples + docs + Swift binary distribution
                     ▼
              bithuman-sdk-public  ◄──────  bithuman-apps
              (public SwiftPM,             (Mac / iPad / iPhone /
               Examples, docs)              CLI reference apps +
                     ▲                       Swift SDK source under SDK/)
                     │ swift-v* tag → xcframework release ──────┐
                     │                                           │
              bithuman-sdk  (private monorepo)                   │
              (Python SDK + daemon binaries)                     │
                     │                                           │
                     ├──────►  PyPI: bithuman   (pip install bithuman)
                     │                                           │
                     └─────── homebrew-bithuman  ◄───────────────┘
                              (brew install bithuman-cli)        CLI binary
                                                                 built from
                                                                 bithuman-apps/CLI
```

## Two avatar engines, briefly

- **Essence** — CPU-only, pre-built `.imx` model from a photo or video. Gestures, animal mode, full body. No idle timeout.
- **Expression** — AI-generated facial animation from any face image. Runs on NVIDIA GPU (cloud or self-hosted) or on-device Apple Silicon M3+.

Comparison: [docs.bithuman.ai/getting-started/models](https://docs.bithuman.ai/getting-started/models).

## Status & support

- **Releases**: [bithuman-sdk-public/releases](https://github.com/bithuman-product/bithuman-sdk-public/releases) for the Swift SDK; [PyPI history](https://pypi.org/project/bithuman/#history) for the Python SDK.
- **Issues / questions**: file in [bithuman-sdk-public/issues](https://github.com/bithuman-product/bithuman-sdk-public/issues) — covers both Swift and Python SDKs.
- **Status & updates**: [bithuman.ai](https://www.bithuman.ai) · [@bithumanAI](https://x.com/bithumanAI).

## License

Each repo carries its own license — most are MIT or source-available with a build-and-run grant. See the `LICENSE` file in each repo.
