---
type: dashboard
status: active
current_phase: 1
---

# 🎨 Digital Art Mastery Roadmap: Krita & Shadows

> [!abstract] Current Status
> **Current Phase:** [[Phase-1-Fundamentals]]
> **Main Goal:** Digital Transition & Shadow System 1-2-3
> **Days Completed:** `$= dv.pages('"06-PROGRESS"').where(p => p.status == "🟢 Completed").length` / 60

## 📅 Quick Navigation
| Phase | Focus | Status |
|------|---------|--------|
| [[Phase-1-Fundamentals]] | Setup & Motor Adaptation | 🟡 In Progress |
| [[Phase-2-Advanced-Shadows]] | 1-2-3 System & Color | 🔴 Pending |
| [[Phase-3-Specialization]] | Materials & Atmosphere | 🔴 Pending |
| [[Phase-4-Mastery]] | Final Portfolio | 🔴 Pending |

## 🚀 Today's Session
```dataview
TABLE WITHOUT ID file.link AS "Day", duration, focus
FROM "01-CORE-ROADMAP"
WHERE type = "roadmap-day" AND status = "🟡 pending"
SORT day ASC
LIMIT 1
```

## 🛠️ Tools & Techniques
- [[Shadow-System-123]] (Core)
- [[Krita-Setup]] (Arch/Huion Config)
- [[Brushes-Presets]]

## 📊 Visual Progress
```dataview
TASK
FROM "01-CORE-ROADMAP"
WHERE type = "roadmap-day" AND status = "🟡 pending"
GROUP BY week
```

---
**Quick Resources:** [[Shortcuts-Reference]] | [[Troubleshooting]] | [[Artist-Database]]
