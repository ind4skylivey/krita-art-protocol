---
type: tracker
---

# 📈 Roadmap Progress Tracker

## 🏁 Milestones
- [ ] **Day 07:** First clean lineart piece.
- [ ] **Day 15:** First complete head with Shadow System 1-2-3.
- [ ] **Day 30:** Character with atmospheric lighting.
- [ ] **Day 45:** Material study (Metal/Leather/Skin).
- [ ] **Day 60:** Portfolio piece ready.

## 📊 Summary
```dataview
TABLE status, phase, week
FROM "01-CORE-ROADMAP"
WHERE type = "roadmap-day"
SORT day ASC
```

## 📅 Daily Logs
```dataview
LIST
FROM "06-PROGRESS"
WHERE type = "daily-log"
SORT day DESC
```

## 🧠 Techniques Unlocked
```dataview
TABLE difficulty, artist
FROM "02-TECHNIQUES"
WHERE type = "technique"
```
