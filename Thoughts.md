
```dataview
TABLE rows.bullets.text as "🧠 Thoughts"
FROM "Daily Notes"
FLATTEN file.lists as bullets
WHERE meta(bullets.section).subpath = "🧠 Thoughts"
SORT file.name desc
GROUP BY file.name
```
