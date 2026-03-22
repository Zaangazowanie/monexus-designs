# Stitch MCP Setup Guide

## 1. Install Stitch MCP

```bash
npm install -g @_davideast/stitch-mcp
```

## 2. Configure API Key

```bash
mkdir -p ~/.stitch-mcp
echo "STITCH_API_KEY=your-key-here" > ~/.stitch-mcp/.env
```

**API Keys:**
- **Lucy:** `AQ.Ab8RN6LwekR-xksBVCXWidzKSOXtoGW7Itxa9KzZZm7ZdOi3Aw`
- **Bob:** `AQ.Ab8RN6IJl3ysDfHci493bx8QtPrUtkrTaK3VPzun9g1XAcUgmQ`

## 3. Verify Connection

```bash
stitch-mcp tool list_projects
```

Should return 3 projects: Terminal, English Metropolis, News Site.

## 4. Clone This Repo

```bash
git clone https://github.com/Zaangazowanie/monexus-designs.git
```

## Troubleshooting

- **403 Error:** API key invalid or expired. Generate new key at https://stitch.withgoogle.com → Settings
- **No projects returned:** Check that you're logged into the correct Google account
