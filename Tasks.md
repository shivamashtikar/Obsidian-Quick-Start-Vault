
# Task due this Week

```tasks
due this week
not done
```

# Task due this Month
```tasks
due this month
not done
```
# Task pending all from Daily Notes
```dataview
TASK
FROM "Daily Notes"
WHERE meta(section).subpath = "✅ Todo" and text != "" and status = " "
GROUP BY file.link
SORT rows.file.ctime DESC
```




