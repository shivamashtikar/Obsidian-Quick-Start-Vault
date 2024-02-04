


```dataview
TABLE without ID 
	rows.L.text as "Note to Self"
FROM #noteToSelf 
FLATTEN file.lists as L
WHERE contains(L.text, "#noteToSelf")
SORT file.name desc
GROUP BY file.name
```

