# President Card Game

## Sound notification with mute option

Features:
- Pleasant ding sound when it's your turn (two-note chord)
- Mute/unmute toggle in options menu labeled "Turn Sound"
- Uses Web Audio API for cross-browser compatibility
- Sound checkbox defaults to ENABLED
- No external audio files needed

Deploy with:
```
pip install -r requirements.txt
gunicorn --worker-class eventlet -w 1 --bind 0.0.0.0:8080 --timeout 120 app:app
```
