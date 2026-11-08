# Jailbreak the Vault - Autonomous Agent (`jailbreak-the-vault-01`)

An autonomous, model-free Python agent built for the `make.fun` security bounty (`jailbreak-the-vault-01`).

## Overview
This repository contains a pure-scripted, deterministic agent designed to extract the 6-character alphanumeric vault code within the allotted 6 chat turns without relying on external paid LLM APIs or third-party dependencies.

## Key Features
* **Zero Dependencies:** Built exclusively using Python's standard libraries (`urllib`, `json`, `re`, `os`), ensuring flawless execution inside isolated Docker containers.
* **Multi-Step Escalation Payload:** Systematically progresses from diagnostic overrides to structural extraction prompts to elicit and capture the target code.
* **Regex Extraction & Verification:** Automatically parses target responses for 6-character alphanumeric strings and submits them instantly to the `/guess` endpoint.

## File Structure
* `main.py` — The core autonomous agent logic.
* `transcript.json` — The session transcript verifying the agent's build history.
* `LICENSE` — MIT Open Source License.

## License
This project is licensed under the terms of the MIT License.
