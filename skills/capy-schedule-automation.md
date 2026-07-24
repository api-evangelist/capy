---
name: Schedule a recurring Capy automation
description: Create, inspect, and manually trigger a recurring or webhook-triggered coding automation on a Capy project.
api: openapi/capy-openapi-original.json
operations: [listProjects, listAutomations, createAutomation, getAutomation, updateAutomation, triggerAutomation, deleteAutomation]
---

# Schedule a recurring Capy automation

Use this to set up recurring agent work (daily cleanups, weekly dependency bumps, nightly builds) on a project.

## Auth
`Authorization: Bearer capy_xxxx`. Base URL `https://capy.ai/api/v1/`.

## Steps
1. **Pick a project.** Call `listProjects`; keep the target `projectId`.
2. **List existing automations.** Call `listAutomations` for the project to avoid duplicates.
3. **Create the automation.** Call `createAutomation` with the `projectId`, a `name`, the agent `prompt`, `triggerType` (cron / webhook / integration), a `cron` + `timezone` for scheduled runs, and the `baseBranch` / `agentType` / `model`.
4. **Verify.** Call `getAutomation` to confirm `enabled`, `cron`, and (for webhook triggers) `webhookUrl` / `hasWebhookSecret`.
5. **Test it now.** Call `triggerAutomation` to run it on demand without waiting for the schedule.
6. **Adjust or remove.** Use `updateAutomation` to change the prompt/schedule/enabled flag, or `deleteAutomation` to remove it.

## Conventions
- Errors use the `{ "error": { "code", "message" } }` envelope; `422 validation_error` details invalid fields.
- No idempotency contract — check `listAutomations` before re-creating on a failed/timed-out `createAutomation`.
