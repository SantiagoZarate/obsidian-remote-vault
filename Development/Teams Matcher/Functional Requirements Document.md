## Funcional Requirements
```dataview
TABLE
	id,
	priority,
	type
FROM "Development/Teams Matcher/Requisitos" 
WHERE
	id != NULL
	AND type = "Functional"
SORT id ASC
```

### Non-Functional Requirements
```dataview
TABLE
	id,
	priority,
	type
FROM "Development/Teams Matcher/Requisitos" 
WHERE
	id != NULL
	AND type != "Functional"
SORT id ASC
```
