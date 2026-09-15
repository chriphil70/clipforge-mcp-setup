# ClipForge MCP Integration Guide

Equip Claude Desktop, Cursor, or any custom AI agent with automated video processing capabilities.

ClipForge handles video trimming, MP3 extraction, watermarking, and 9:16 vertical re-framing over a managed API.

## Quickstart for Claude Desktop

1. Open your `claude_desktop_config.json` file.
2. Add the `clipforge` server configuration:

```json
{
  "mcpServers": {
    "clipforge": {
      "command": "npx",
      "args": ["-y", "@apify/mcp-server", "--actor-id", "budding_retrograde/clipforge"],
      "env": {
        "APIFY_TOKEN": "YOUR_APIFY_TOKEN"
      }
    }
  }
}
