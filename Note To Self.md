
Any list containing #noteToSelf will appear here

```dataview
TABLE without ID 
	regexreplace(rows.L.text, "#noteToSelf", "") as "Note to Self"
FROM #noteToSelf 
FLATTEN file.lists as L
WHERE contains(L.text, "#noteToSelf")
SORT file.name desc
GROUP BY file.name
```

