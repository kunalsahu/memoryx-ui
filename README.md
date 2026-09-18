# MemoryX Enterprise Console

React/Vite UI for the MemoryX API. No dummy business data is used: screens show API results, empty states, loading states, or errors.

## Run
1. `npm install`
2. `cp .env.example .env` (optional)
3. `npm run dev`
4. Open **System** in the UI and save API base URL, bearer token, and tenant ID.

## Backend requirements
- MemoryX FastAPI must be reachable from the browser.
- Configure CORS on FastAPI for the Vite origin (normally `http://localhost:5173`).
- The UI sends `Authorization: Bearer <token>` and `x-tenant-id`.

## Implemented workspaces
Overview, Memory Explorer, Search, Vector Search, Upload, Lineage, Memory Intelligence, Health, Duplicates, Conflicts, Knowledge Gaps via full Intelligence run, Promotion, Archival, Recommendation Execution/Approval, Cognitive Workspace, Context Assembly, Reflection, Learning, MetaMemory Topics/Signals, Summaries/Lifecycle, Ethics/PII, Audit, Telemetry, Tenants/User context, API Keys, and System configuration.

## Security
Bearer token is stored in browser localStorage for local development convenience. For production, use an appropriate secure authentication/session architecture rather than persisting long-lived privileged tokens in localStorage.
# memoryx-ui
