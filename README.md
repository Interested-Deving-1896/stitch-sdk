[update-readmes]   Mode: rewrite — migrating to template structure...
# stitch-sdk

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/stitch-sdk)

<!-- AI:start:what-it-does -->
_Description pending._
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install


```bash
npm install @google/stitch-sdk
```

To use `stitchTools()` with the [Vercel AI SDK](https://sdk.vercel.ai/), install `ai` as well:

```bash
npm install @google/stitch-sdk ai
```

## Usage

<!-- Add usage examples here. This section is yours — the AI will not modify it. -->

## Configuration


### Environment Variables

| Variable | Required | Description |
|---|---|---|
| `STITCH_API_KEY` | Yes (or use OAuth) | API key for authentication |
| `STITCH_ACCESS_TOKEN` | No | OAuth access token (alternative to API key) |
| `GOOGLE_CLOUD_PROJECT` | With OAuth | Google Cloud project ID |
| `STITCH_HOST` | No | Override the MCP server URL |

### Explicit Configuration

```ts
import { Stitch, StitchToolClient } from "@google/stitch-sdk";

const client = new StitchToolClient({
  apiKey: "your-api-key",
  baseUrl: "https://stitch.googleapis.com/mcp",
  timeout: 300_000,
});

const sdk = new Stitch(client);
const projects = await sdk.projects();
```

| Option | Type | Default | Description |
|---|---|---|---|
| `apiKey` | `string` | `STITCH_API_KEY` | API key |
| `accessToken` | `string` | `STITCH_ACCESS_TOKEN` | OAuth token |
| `projectId` | `string` | `GOOGLE_CLOUD_PROJECT` | Cloud project ID |
| `baseUrl` | `string` | `https://stitch.googleapis.com/mcp` | MCP server URL |
| `timeout` | `number` | `300000` | Request timeout (ms) |

Authentication requires either `apiKey` or both `accessToken` and `projectId`.

## CI

<!-- AI:start:ci -->
_CI documentation pending._
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/stitch-sdk`](https://github.com/Interested-Deving-1896/stitch-sdk) and mirrored through:

```
Interested-Deving-1896/stitch-sdk  ──►  OpenOS-Project-OSP/stitch-sdk  ──►  OpenOS-Project-Ecosystem-OOC/stitch-sdk
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
_Contributors pending._
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
[Apache-2.0](https://github.com/Interested-Deving-1896/stitch-sdk/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
