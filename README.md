# President Card Game

## FIXED: Toggle button + Working Sound + Restart

Features:
✓ "⚙ Options" button to open/close options panel
✓ Options panel hidden by default
✓ "🔊 Turn Sound" checkbox to mute sound
✓ Ding sound plays when it's your turn
✓ "🔄 Restart Hand" button to restart with options
✓ Play log at bottom left
✓ Console logging for debugging

How to use:
1. Click "⚙ Options" button to open panel
2. Toggle "🔊 Turn Sound" to mute/unmute
3. Click "🔄 Restart Hand" to apply options
4. Click × or toggle button again to close panel

Debug:
Open browser console (F12) to see detailed logs for sound, restart, and socket events.

Deploy:
```
pip install -r requirements.txt
gunicorn --worker-class eventlet -w 1 --bind 0.0.0.0:8080 --timeout 120 app:app
```
