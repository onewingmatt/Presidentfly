# President Card Game

## SOUND DEEP DIVE - FIXED!

Root cause found and fixed:
- Server was NOT emitting 'your_turn' events
- Added your_turn emission to app.py
- Improved socket listeners in HTML
- Added fallback from 'update' events
- Added TEST SOUND button to verify sound works

Changes:
1. app.py: Added socketio.emit('your_turn') after plays
2. HTML: Added multiple listeners (your_turn, update, cpu_turn)
3. HTML: Added 🔊 Test Sound button to test manually

How to test:
1. Open options panel (⚙ button)
2. Click 🔊 Test Sound button to test sound works
3. Toggle "🔊 Turn Sound" to mute
4. When it's your turn, sound should play automatically

Deploy:
```
pip install -r requirements.txt
gunicorn --worker-class eventlet -w 1 --bind 0.0.0.0:8080 --timeout 120 app:app
```
