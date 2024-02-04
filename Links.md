
```dataview
TABLE rows.bullets.text as "🔗 Links"
FROM "Daily Notes"
FLATTEN file.lists as bullets
WHERE meta(bullets.section).subpath = "🔗 Links"
SORT file.name desc
GROUP BY file.name
```
