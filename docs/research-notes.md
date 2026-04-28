# tmux for OpenCUA: Open Session Interface

## Purpose

This document records the research framing behind the static GitHub Pages site. The project studies how tmux can be adapted for OpenCUA as a durable terminal substrate for agentic work.

## Research Question

How can an open CUA stack use tmux while preserving inspectable boundaries between observation, planning, and shell execution?

## Working Thesis

The adapter turns tmux into a transparent systems boundary, where every pane event and command result can be replayed, filtered, and audited.

## Design Claims

- A minimal session schema records window, pane, prompt, and command-output regions.
- Open logs allow external evaluators to inspect action ordering.
- Terminal observation is normalized before it reaches the policy layer.

## Evaluation Lens

- Schema stability across shells
- Auditability of command sequences
- Interoperability with external task harnesses


## Threats to Validity

- Terminal state can be over-instrumented, causing an adapter to measure artifacts of the harness rather than real agent behavior.
- A final successful artifact may hide poor recovery behavior, repeated command attempts, or fragile focus management.
- Agent-specific adapters can become difficult to compare unless trace schemas remain explicit and documented.

## Hero Image Prompt Summary

A 700x500 academic technical illustration for tmux adaptation research with OpenCUA, emphasizing terminal panes, agent traces, reproducible evaluation, and a serious research discussion style. The generated image was copied into `docs/assets/hero.png` and normalized to 700x500 pixels.
