# CargoWall Hello World

[![View Action Graph](https://img.shields.io/badge/View-Action%20Graph-blue)](https://app.actionforge.dev/github/sebastianrath/cargo-test/main/.github/workflows/graphs/cargowall-hello-world.act)

Demonstrates [CargoWall](https://github.com/code-cargo/cargowall-action) eBPF-based network firewall via an [Actionforge](https://www.actionforge.dev) graph.

## What it does

On every push to `main`, the Actionforge graph executes CargoWall in `enforce` mode — activating eBPF egress filtering on the GitHub Actions runner. It then curls an allowed host (`github.com`) followed by a blocked host (`example.com`) to demonstrate that CargoWall blocks unauthorized egress.

## Files

- `.github/workflows/cargowall.yml` — GitHub Actions workflow
- `.github/workflows/graphs/cargowall-hello-world.act` — Actionforge graph
