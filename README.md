# Duet for macOS

[Download the latest release](https://github.com/MrBiscuit/duet-releases/releases/latest)

Public binary downloads for Duet. Application source remains in its private repository.

## Install

Apple Silicon (M1 or later), macOS 13 or newer. Open the DMG, drag Duet to Applications, and launch it. Download updates from the release page; this build has no automatic updater.

## Set up

- Choose Continue with ChatGPT and sign in with an account invited to the hosted Duet board. Downloading the app does not grant board membership.
- Settings (Command-comma) → This computer shows the projects folder and agent/GitHub readiness. The default projects folder is `~/Duet`.
- For Penny's local workflows, install Claude Code and sign in to your subscription, then authenticate its `coin-workflow` MCP connection via `/mcp`. Install and sign in to GitHub CLI (`gh`) to access private flow projects.
- Local automatic workflows currently support the board owner's Documentation and Component Fix flows. Invited collaborators can use the board. Codex readiness is displayed, but this build does not run Codex workflows.
- Allow microphone access when using Penny's voice input, and allow file access to your chosen projects folder when requested.

## Verification and limits

Duet 0.1.1 uses Developer ID Application signing with hardened runtime. See each release's verification record and SHA-256 checksums for Apple notarization and Gatekeeper results.

The packaged Mac app was launched, loaded its hosted sign-in screen, opened the OpenAI login handoff, quit and reopened. Signed-in board use, real workflow runs, fresh GitHub device sign-in, project download and microphone recording remain separate acceptance checks. Tested architecture: Apple Silicon; no Intel build is provided.
