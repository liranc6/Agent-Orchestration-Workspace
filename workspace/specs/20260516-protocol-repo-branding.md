# Spec: New Communication Protocol Repository Naming

## Purpose
Define a marketing-friendly, product-focused name for the new external repository that houses the A2A communication standard for Agent Orchestration Workspace.

## Recommendation
- Primary repo name: `Agent-Orchestration-Protocol`
- Positioning: "A2A communication standard for structured agent orchestration."

## Why this name
- `Agent-Orchestration` links directly to the existing AOW brand.
- `Protocol` clearly signals a standardized communication layer, not an application or runtime.
- The combination supports developer trust, discoverability, and long-term extensibility.

## Scope and boundary
The new repo should be dedicated to the communication standard and should not include:
- orchestration runtime code
- task execution logic
- agent business logic
- workflow tracking engine

It should include:
- protocol definitions for structured agent messaging
- shorthand and status code guidelines
- message format examples and templates
- glossary of terms and acronyms
- recommended repository-based shared-state conventions
- integration guidance for AOW and other orchestration systems

## Marketing angle
Use the new repo name to present it as the protocol layer behind operational AI team collaboration:
- "A lean, operational messaging standard for AI agents coordinating through shared repo artifacts."
- "Inspired by military, aviation, medicine, and trading-room communication, built for multi-agent workflows."
- "Reduces context inflation and coordination overhead with compact, protocolized A2A messaging."

## Suggested tagline
- "Agent-Orchestration-Protocol: a standard for efficient A2A communication in long-running AI workflows."

## Implementation notes
- After the user provides the repo link, update AOW references and README copy to point to the new repository.
- Keep `process/communication_protocol/` in AOW as a compatibility pointer until the external repo is live.
- The external repo should be referenced from AOW docs as the authoritative source for protocol rules.

## Approval criteria
- Name clearly communicates orchestration and protocol scope.
- Repo is positioned as a standalone communication standard.
- Scope isolation is obvious: this repo is not the AOW engine, it is the A2A protocol standard.
- Marketing copy is concise and aligned with the user’s LinkedIn narrative.
