# President Card Game

## Complete rewrite of player joining logic

FIXED: Player joining now transfers all cards and state from CPU player before deletion
- Deep copy of hand performed
- All player state (role, passed, finished_position) transferred
- Debug logging added to trace hand transfers

Deploy with:
```
pip install -r requirements.txt
python app.py
```

Check Fly.io logs for "[DEBUG]" messages to verify hand transfers are working.
