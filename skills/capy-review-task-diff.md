---
name: Inspect a Capy task and its diff
description: Find the tasks produced by a Capy thread and pull the current code diff for review before merging.
api: openapi/capy-openapi-original.json
operations: [listThreads, getThread, getTask, getTaskDiff]
---

# Inspect a Capy task and its diff

Use this to review the code a Capy agent generated before it becomes a pull request.

## Auth
`Authorization: Bearer capy_xxxx`. Base URL `https://capy.ai/api/v1/`.

## Steps
1. **Find the thread.** Call `listThreads` (filter by `projectId`, `status`, `branch`, or `prNumber`) or use a known thread `id`.
2. **Read the thread.** Call `getThread` to see its `tasks[]` and `pullRequests[]`.
3. **Get the task.** Call `getTask` with the task UUID or human identifier (e.g. `SCO-123`) for status and metadata.
4. **Pull the diff.** Call `getTaskDiff` to retrieve the current code diff for that task; review it before creating/merging a PR.

## Conventions
- Task IDs accept both UUID and human-identifier (`SCO-123`) forms.
- List calls are cursor-paginated (`limit` + `cursor` -> `items`/`nextCursor`/`hasMore`).
- Errors: `{ "error": { "code", "message" } }`; `404 not_found` for a bad task/thread ID.
