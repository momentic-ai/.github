# Momentic

Mo is an AI QA engineer. Point it at your app on web, iOS or Android and get
bugs back, each with a recording and reproduction steps.

## Get started

Start Mo from your coding agent (Claude Code, Cursor, Codex, Copilot and
others). In your project root:

```bash
npm install -g qa
qa login
qa skills
```

`qa skills` asks which agents to set up and installs the `mo-qa` skill for
them. Then ask your agent for a bug bash:

```text
/mo-qa bug bash the cart on https://staging.example.com/cart.
Do not place an order.
```

The agent writes the brief, starts the session, follows it and exports the
report. It can also fix the bugs Mo finds and recheck them.

You can also start a session from [the app](https://app.momentic.ai/mo) or by
mentioning `@momentic-ai` on a pull request
([GitHub setup](https://momentic.ai/docs/mo/integrations/github)). Mo needs a
Momentic account: [sign up](https://momentic.ai/mo). See the
[quickstart](https://momentic.ai/docs/mo/quickstart).

Momentic also runs plain-English end-to-end tests. They live as YAML files in
your repo and run locally or in CI.

## QA Bench

[QA Bench](https://momentic.ai/qa-bench) runs Mo, Codex, Claude Code and Devin
against 20 product areas of Gitea, Metabase, Twenty and Saleor, then grades
their bug reports against 1,396 human-reviewed bug labels. With 60 minutes per
area, Mo found about 269 labeled bugs at 84% precision. The next best agent
found about 86.

[Write-up](https://momentic.ai/blog/qa-bench) |
[Code](https://github.com/momentic-ai/qa-bench) |
[Dataset](https://huggingface.co/datasets/momentic/qa-bench)

## Repositories

- [qa-bench](https://github.com/momentic-ai/qa-bench): the QA Bench harness, fixtures and results.
- [qa](https://github.com/momentic-ai/qa): the CLI for Mo.
- [skills](https://github.com/momentic-ai/skills): agent skills and MCP servers for coding agents.
- [cli](https://github.com/momentic-ai/cli): the Momentic CLI. Write, run and repair web tests from your terminal.
- [mobile-cli](https://github.com/momentic-ai/mobile-cli): the Momentic CLI for iOS and Android tests.
- [examples](https://github.com/momentic-ai/examples): example projects and CI setups.

[momentic.ai](https://momentic.ai) | [Docs](https://momentic.ai/docs) | [X](https://x.com/momenticai) | Y Combinator W24
