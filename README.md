# eplus

<!-- three.ws:badges -->
[![GitHub stars](https://img.shields.io/github/stars/nirholas/eplus?style=flat&logo=github)](https://github.com/nirholas/eplus/stargazers) [![Last commit](https://img.shields.io/github/last-commit/nirholas/eplus?style=flat)](https://github.com/nirholas/eplus/commits) [![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat)](https://github.com/nirholas/eplus/pulls) [![AI agent friendly](https://img.shields.io/badge/AI%20agents-AGENTS.md%20%2B%20llms.txt-6d5dfc?style=flat)](https://github.com/nirholas/eplus/blob/HEAD/AGENTS.md)
<!-- /three.ws:badges -->


### A fast, light, open chat UI

### Key features:

- 🔌 Multiple providers, plug in your API keys (stored entirely locally) and you're good to go

  - Local models (through Ollama)
  - OpenRouter (which lets you use ALL models across many providers: OpenAI, Anthropic, OSS, 50+ others)
  - OpenAI
  - Anthropic
  - Mistral
  - Groq

- 🛠️ Tool use
  - Check out `server/toolfns/toolfns.go`. You only need to write functions. The function comment is the description the model receives, so it knows what to use. Click the `Sync` button in the web UI to refresh your tools.
- 🖼️ Multimodal input: upload, paste, or share links to images
- 🎨 Image generation using DALL-E 3
- 📝 Multi-shot prompting. Also edit, delete, regenerate messages, whatever. The world is your oyster
- ⚡ Pre-filled responses (where supported by provider)
- 🌐 Support for all available models across all providers
- 🔄 Change model mid-conversation
- 🔐 Sync chats and keys across devices, end-to-end encrypted. Self-hosted, or use our hosted instance.
- 🔗 Conversation sharing (if you choose to share, your conversation has to be stored on an external server for the share link to be made available. Self-hosted share options coming soon. No, I will not view any of your stuff.)
- 🌿 Branching conversation history (like the left-right ChatGPT arrows that you can click to go back to a previous response)

### Privacy:

- Completely private and transparent. All your conversation history and keys are stored entirely locally, and kept only in your browser, on your device.

## How to install?

If you don't want to use tools, you don't need to install anything. A hosted instance is available at: https://eplus.chat

If you want to use tools, proceed below.

## Single binary:

The eplus tool server is available prebuilt as a single binary. [Download prebuilt package from the releases page.](https://github.com/nirholas/eplus/releases)

Download the binary for your platform, then run it, which will start the tool server:

```
./eplus-darwin-amd64
Tool server running at http://localhost:8081
```

Go back to https://eplus.chat, head over to Settings -> Tool calling, and click the "Refresh tools" button. You should be good to go!

### Building client and server locally:

1. Clone the repository
2. Install and start the client: `npm i && npm run dev`. The client will be accessible at http://localhost:5173
3. Install and start the server: `cd server && go generate ./... && go build && ./server -password foobar`. The server will be accessible at http://localhost:8081. You can plug this into the server address in the chat UI along with the password you selected.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=nirholas/eplus&type=Date)](https://www.star-history.com/#nirholas/eplus&Date)

<!-- three.ws:growth -->
## Support the project

If eplus saves you time, **[star it on GitHub](https://github.com/nirholas/eplus)**. Stars are how other developers and AI agents find the repositories worth trusting, and they cost you one click.

Know someone who would use it? [Post on X](https://twitter.com/intent/tweet?text=eplus%3A%20Fast%2C%20light%2C%20open-source%20chat%20UI%20with%20bring-your-own%20API%20keys%20for%20Ollama%2C%20OpenRouter%2C%20OpenAI&url=https%3A%2F%2Fgithub.com%2Fnirholas%2Feplus) · [Share on Bluesky](https://bsky.app/intent/compose?text=eplus%3A%20Fast%2C%20light%2C%20open-source%20chat%20UI%20with%20bring-your-own%20API%20keys%20for%20Ollama%2C%20OpenRouter%2C%20OpenAI%20https%3A%2F%2Fgithub.com%2Fnirholas%2Feplus) · [Share on LinkedIn](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fnirholas%2Feplus) · [Submit to Hacker News](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fnirholas%2Feplus&t=eplus%3A%20Fast%2C%20light%2C%20open-source%20chat%20UI%20with%20bring-your-own%20API%20keys%20for%20Ollama%2C%20OpenRouter%2C%20OpenAI) · [Share on Reddit](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fnirholas%2Feplus&title=eplus%3A%20Fast%2C%20light%2C%20open-source%20chat%20UI%20with%20bring-your-own%20API%20keys%20for%20Ollama%2C%20OpenRouter%2C%20OpenAI)

## Built for AI agents too

Coding agents and LLM tooling can read this repo directly: [AGENTS.md](./AGENTS.md), [llms.txt](./llms.txt), [llms-full.txt](./llms-full.txt). Point an agent at `https://github.com/nirholas/eplus` and it has the context it needs.

## More from the same author

- [All repositories by nirholas](https://github.com/nirholas/nirholas#readme): the full catalog, grouped by topic
- [three.ws](https://three.ws): the platform for 3D AI agents with Solana wallets, a skill marketplace and x402 payments
- Questions or ideas: [open an issue](https://github.com/nirholas/eplus/issues) or [start a discussion](https://github.com/nirholas/eplus/discussions)

## Contributors

[![Contributors](https://contrib.rocks/image?repo=nirholas/eplus)](https://github.com/nirholas/eplus/graphs/contributors)

<!-- /three.ws:growth -->
