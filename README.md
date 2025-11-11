# President Card Game

## Fly.io Deployment Fix

Fixed Issues:
- Port changed from 5000 to 8080
- Quote matching fixed
- fly.toml included for Fly.io

Deploy:
```bash
flyctl deploy -a presidentfly --config fly.toml
```

Features:
✓ Sound notifications with mute toggle
✓ Play log (collapsible)
✓ Options panel (collapsible)
✓ Wild card options
✓ Card swapping
✓ CPU players

Local testing:
```bash
pip install -r requirements.txt
python app.py
```

Then visit http://localhost:8080
