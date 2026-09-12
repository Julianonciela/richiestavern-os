# Connect Hermes Desktop to VPS — Quick Setup

## PowerShell (run as admin if needed)

```powershell
# 1. Find your Hermes install
cd C:\Users\julia\AppData\Local\hermes

# 2. Connect to the VPS gateway
hermes gateway login https://69.62.66.247:8787

# 3. Verify connection
hermes status
```

After this, your Desktop and WebUI share:
- Same memory (what Hermes knows about Juliano, Richie's Tavern, etc.)
- Same skills (auto-fix, vinci-audit-delivery, etc.)
- Same cron jobs (briefs, competition watch)
- Same sessions (continue from Desktop what you started in WebUI)

## Autonomous bot army (already running on VPS)

| Job | Schedule | Delivers to |
|---|---|---|
| RT-OS Daily Brief | Every day 8am UTC | Telegram |
| Paso Robles Competition Watch | Every 6 hours | Telegram |
| RT-OS Checklist Reminder | Every day 9am UTC | Telegram |

## Spawn a bot from Desktop

```powershell
# Quick research task (returns result, then exits)
hermes chat -q "Check the RT-OS checklist and tell me what's blocked"

# Long autonomous mission (hours)
hermes chat -q "Build 3 new Academy lessons about hospitality, save to /workspace/rt-os/academy/"
```

## Profile isolation (optional)

```powershell
# Create a dedicated profile for Richie's Tavern work
hermes profile create richie
hermes profile use richie
hermes gateway login https://69.62.66.247:8787
```

This keeps Richie's Tavern conversations separate from VINCI/client work.