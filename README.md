# President Card Game

## COMPLETE FIX: Sound + Mute Button + Options Panel

Features:
✓ Ding sound plays when it's your turn
✓ "Turn Sound" checkbox to mute (enabled by default)
✓ Wild card options in panel
✓ Play log (collapsible)
✓ Restart button

Options Panel (top right):
- 2s Wild checkbox
- Black 3s Wild checkbox
- JD Wild checkbox
- Turn Sound checkbox (MUTE BUTTON)
- Restart Hand button

Deploy:
```
pip install -r requirements.txt
gunicorn --worker-class eventlet -w 1 --bind 0.0.0.0:8080 --timeout 120 app:app
```
