# image-generation-mcp — leftover

Human creates the GitHub repo (`shotah/image-generation-mcp`) and `git init`. Do not `git init` / `gh` from the agent.

## Follow-ups (not this binary)

- Yard ingest: gantree `PACKAGES` + `HOST_SHAPE.image` so the console can grant `image`.
- ai-gantry: when MCP returns `ImageContent`, skip stuffing base64 into the model context and `SendPhoto` on Telegram/Discord/Slack. Today the JSON summary survives truncation; the picture does not auto-send.
- Extra `IMAGE_PROVIDER` backends (OpenAI, etc.) behind the existing `Provider` interface. Keep server id `image` and tools `photo_generate` / `photo_edit`.

## Do not

- Fold into `google-mcp` (Workspace OAuth cannot call Nano Banana)
- Name tools `image_*` (double prefix)
- Live API in unit tests
