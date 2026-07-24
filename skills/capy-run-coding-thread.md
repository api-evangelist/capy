---
name: Run a Capy coding thread
description: Start a Capy captain thread on a project, send it a coding instruction, poll for progress, and read the agent's messages.
api: openapi/capy-openapi-original.json
operations: [listProjects, createAndStartThread, getThread, sendThreadMessage, listThreadMessages, stopThread]
---

# Run a Capy coding thread

Use this to delegate a coding task to a Capy captain agent and follow it to completion.

## Auth
All requests: `Authorization: Bearer capy_xxxx`. Base URL `https://capy.ai/api/v1/`.
Generate a token at capy.ai/settings/tokens.

## Steps
1. **Pick a project.** Call `listProjects` and choose the `id` of the repo workspace you want the agent to work in.
2. **Start the thread.** Call `createAndStartThread` with the `projectId` and your task prompt (optionally attach existing project `tags`). It creates the captain thread and immediately begins execution; keep the returned thread `id`.
3. **Follow progress.** Poll `getThread` on the thread `id`; watch `status` (`active`/`idle`/`archived`) and `runState`/`waitingOn`.
4. **Read output.** Call `listThreadMessages` (cursor pagination: `limit`, `cursor` -> `items`/`nextCursor`/`hasMore`) to read what the agent has said and any generated diffs/tasks.
5. **Steer if needed.** Call `sendThreadMessage` to reply with clarifications or follow-up instructions; the thread resumes.
6. **Stop if needed.** Call `stopThread` to halt an actively running thread.

## Conventions
- Errors: non-2xx returns `{ "error": { "code", "message", "details"? } }`. Handle `401 unauthorized`, `422 validation_error`, `429 too_many_requests` (back off).
- No idempotency key: do not blindly retry `createAndStartThread` / `sendThreadMessage` on timeout — check state with `getThread` first.
