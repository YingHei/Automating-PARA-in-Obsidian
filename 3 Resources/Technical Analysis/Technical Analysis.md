---
para: resource
---
# Technical Analysis

```dataview
Table without id (subtopic + " (" + length(rows.file.link) + ")") as "Subtopic", sort(rows.file.link) as File
FROM "3 Resources/Technical Analysis"
WHERE file.name != this.file.name
FLATTEN subtopic
GROUP BY subtopic
SORT subtopic
```

## Linked notes
```dataview
Table sort(rows.file.link) as File
FROM [[]]
WHERE !contains(file.folder, this.file.name)
GROUP BY file.folder as Folder
```
