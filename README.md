# President Card Game

## FIXED: Play Log Now Works!

Changes:
1. app.py: Added play_made emissions to on_play handler
2. app.py: Added play_made emissions to on_pass handler
3. HTML: Improved play_made listener
4. HTML: Enhanced addPlayLogEntry function
5. Play log now shows all plays in chronological order

Play Log Features:
- Shows player name and cards played
- Shows PASS actions in red
- Keeps last 100 entries
- Newest plays at top of list
- Located at bottom left
- Collapsible

How to use:
1. Play log appears automatically at bottom left
2. Click "Play Log" header to collapse/expand
3. All plays are logged in real-time

Deploy:
```
pip install -r requirements.txt
gunicorn --worker-class eventlet -w 1 --bind 0.0.0.0:8080 --timeout 120 app:app
```
