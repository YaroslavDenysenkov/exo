
# 🗂 All Properties Dashboard

This note dynamically lists all YAML properties used in your vault.

---


```dataview
TABLE project, length(rows) as "Count"
FROM ""
WHERE project
GROUP BY project
```

## Projects
```dataview
TABLE WITHOUT ID
FROM ""
WHERE project
GROUP BY project
SORT project ASC
```
