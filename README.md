<p align="center"><strong>PWE Codex</strong> is a coding agent that runs on your computer, by <a href="https://pakwone.com">Pakwone Application</a>.</p>

> **PWE Codex is a Pakwone-branded build of [OpenAI Codex CLI](https://github.com/openai/codex)**, used under the Apache License 2.0.
> Pakwone Application is not affiliated with, sponsored by or endorsed by OpenAI. See [NOTICE](NOTICE) and [LICENSE](LICENSE).
> The original README is kept as [UPSTREAM_README.md](UPSTREAM_README.md).

---

## What it does

PWE Codex reads your project, writes and edits code, runs commands and tests, and explains what it did, all from your terminal. It asks before it runs anything risky, and it works inside a sandbox by default.

## Build from source

Requires the Rust toolchain (`rustup`), which picks the right version from `codex-rs/rust-toolchain.toml`.

```bash
git clone https://github.com/quantumnurobot/pwe-codex.git
cd pwe-codex/codex-rs
cargo build --release -p codex-cli --bin codex
./target/release/codex          # starts PWE Codex
```

On Windows the program is `target\release\codex.exe`. You can copy it anywhere on your `PATH` and rename it `pwe-codex`.

## Sign in

The first time it starts, PWE Codex asks you to sign in with ChatGPT or an OpenAI API key, exactly like Codex CLI. Your usage is billed by OpenAI under your own account.

## What changed from Codex CLI

- The app shows **PWE Codex** in its header and output.
- A `pwe-codex` command name is added to the npm launcher.
- Everything else is upstream Codex CLI. To pick up OpenAI's updates, pull from `openai/codex` and re-apply these changes.

## License

Apache License 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
