---
creation date: 2024-04-28 23:43
para: project
domain:
  - "[[Personal Development]]"
start-date: 2024-04-28
by-when: 2025-05-31
achieve-date:
---
# Get a Driver Licence
## Desired outcome
- Get a driver licence by Feb 2025

## Action Plan
1. Apply (by Aug 2024)
2. Take written test (by Sep 2024)
3. Practice driving (Oct 2024 - Jan 2025)
4. Take road test (by Feb 2025)

---
## All files
```dataview
Table without id type as Type, rows.file.link as File
FROM "1 Projects/Get a Driver Licence"
WHERE file.name != this.file.name
FLATTEN type
GROUP BY type
SORT type, file.name
```

## Linked notes
```dataview
Table sort(rows.file.link) as File
FROM [[]]
WHERE !contains(file.folder, this.file.name)
GROUP BY file.folder as Folder
```
