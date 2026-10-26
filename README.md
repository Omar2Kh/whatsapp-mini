# WhatsApp Mini — One-to-One Messaging System

## Overview

WhatsApp Mini is a Software Engineering course project that explores the requirements, design, and testing strategy for a simplified one-to-one text messaging system.

The project focuses on defining the system's scope, specifying key messaging features, designing a modular server architecture, and planning test cases. It is a documentation and design project, not a fully implemented messaging application.

## Project Scope

The proposed system covers four core features:

- **Send and Receive Messages:** Support text messaging between two users.
- **Chat History:** View previously exchanged messages.
- **Reply to Messages:** Reply to a specific message in the conversation.
- **Delete for Everyone:** Define rules for deleting a message for both participants.

Features outside this simplified scope are not included in the current project.

## Requirements

The project documents functional requirements, quality requirements, and feature-specific rules.

### Functional Requirements

- Users should be able to send and receive text messages.
- Users should be able to view their chat history.
- Users should be able to reply to a specific message.
- Users should be able to delete eligible messages for everyone according to the defined rules.

### Delete for Everyone

The feature was specified using the WRSPM approach and four software rules (S1–S4). The proposed deletion window is **900 seconds (15 minutes)**.

The rules describe the intended behavior of the feature; they have not yet been validated through a running implementation.

## Architecture

The proposed architecture uses a modular server design.

- **Message Service:** Responsible for message-related operations and the authoritative writer of message state.
- **Node.js:** Proposed server-side technology.
- **SQLite:** Proposed database for storing application data.

These technologies are part of the design proposal and have not yet been used in a completed implementation. PostgreSQL was considered as an alternative if concurrency requirements justify it.

An Architecture Decision Record (ADR 001) documents the architecture decision.

## Testing Plan

The project includes a test plan with **8 planned test cases** covering expected system behavior.

It also defines a performance target of **95% of requests completing within 1.5 seconds under 20 concurrent sessions**.

These are planned tests and target values, not measured results. Test execution remains pending because the application has not been implemented.

## Project Management

Project tasks and the project lifecycle were organized in Linear, with linked issues used to track the planned work.

## Project Status

**Current status: Requirements, design, and test planning completed; implementation and test execution pending.**

Completed work includes:
- Requirements and scope documentation.
- Workflow and system design.
- Delete for Everyone specification using WRSPM.
- Modular architecture proposal and ADR.
- Test-case design and performance target definition.
- Project task planning in Linear.

Not yet completed:
- Working application and source code.
- Database integration.
- Execution of the planned tests.
- Verification of the performance target.

## Repository Contents

- `docs/` — Project report, diagrams, requirements, architecture decisions, and test documentation.
- `README.md` — Project overview, scope, design, test plan, and current status.

## Team

A two-person team course project completed as part of Software Engineering coursework at Assiut University.

## Disclaimer

This repository documents the analysis and design of a proposed messaging system. It does not currently contain a working WhatsApp clone or a tested backend implementation.
