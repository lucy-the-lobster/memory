# TOOLS.md - Local Notes

Skills define _how_ tools work. This file is for _your_ specifics — the stuff that's unique to your setup.

## What Goes Here

Things like:

- Camera names and locations
- SSH hosts and aliases
- Preferred voices for TTS
- Speaker/room names
- Device nicknames
- Anything environment-specific

## Examples

```markdown
### Cameras



### SSH

- home-server → 192.168.1.100, user: admin

### TTS

- Preferred voice: "Nova" (warm, slightly British)
- Default speaker: Kitchen HomePod
```

## Gmail / Google Workspace

- **Account**: lucylobster070@gmail.com
- **Tool**: `gog` CLI (https://gogcli.sh)
- **Services enabled**: Gmail, Calendar, Drive, Contacts, Docs, Sheets
- **Auth**: OAuth (file-based keyring)
- **Credentials**: `/home/mark/.config/gogcli/credentials.json`
- **Keyring**: `/home/mark/.config/gogcli/keyring/`

**Environment variables** (already in `~/.bashrc`):
```bash
export PYTHON_KEYRING_BACKEND=keyring.backends.file.PlaintextKeyring
export GOG_KEYRING_PASSWORD="gog2025"
export GOG_ACCOUNT=lucylobster070@gmail.com
```

**Quick commands**:
```bash
# Search recent emails
gog gmail search "in:inbox newer_than:7d" --max 10

# Send email
gog gmail send --to recipient@example.com --subject "Subject" --body "Message"

# Check calendar this week
gog calendar events primary --from "2026-02-15" --to "2026-02-22"
```

## Why Separate?

Skills are shared. Your setup is yours. Keeping them apart means you can update skills without losing your notes, and share skills without leaking your infrastructure.

---

Add whatever helps you do your job. This is your cheat sheet.
