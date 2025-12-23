Public API Documentation

If you change the public API documentation, make sure to keep both the source spec and the hosted docs in sync.

Checklist
- Update the source OpenAPI spec: `server/api/publicApi/documentation/openapi.yaml`.
- Sync the hosted docs in the `beautifulai/beautifulai-docs` repo (GitHub Pages serves `docs.beautiful.ai` from that repo).
- Verify the docs site loads the latest spec (the Swagger UI config points at `https://docs.beautiful.ai/openapi.yaml` in `server/api/publicApi/documentation/swagger-initializer.js`).

Notes
- If the docs hostname or path changes, update `server/api/publicApi/documentation/swagger-initializer.js`.
- Keep the static Swagger UI assets in this folder unchanged unless you intentionally upgrade Swagger UI.
