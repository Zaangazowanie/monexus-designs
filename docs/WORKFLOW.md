# Stitch Workflow Guide

## Generate a Screen

```bash
stitch-mcp tool generate_screen_from_text \
  --id 7009023910723487578 \
  --prompt "Dark terminal interface showing live news feeds in a grid layout" \
  --device DESKTOP
```

## Edit Existing Screens

```bash
stitch-mcp tool edit_screens \
  --id 7009023910723487578 \
  --screenIds "123,456" \
  --prompt "Make the sidebar collapsible"
```

## List Screens in Project

```bash
stitch-mcp tool list_screens --id 7009023910723487578
```

## Export Screen

1. Open Stitch web UI: https://stitch.withgoogle.com
2. Navigate to project → screen
3. Export → Download HTML/CSS
4. Save to `monexus-designs/<project>/screens/`

## Design → Deploy Flow

1. Generate design in Stitch
2. Export HTML/CSS
3. Convert to React components (use `react:components` skill)
4. Integrate into Next.js/React app
5. Deploy via PM2

## Best Practices

- **DESIGN.md:** Each project has a DESIGN.md synced from Stitch design tokens
- **Shared tokens:** Use `shared/tokens/` for consistent colors, typography, spacing
- **Screenshots:** Save thumbnails to `assets/` for documentation
