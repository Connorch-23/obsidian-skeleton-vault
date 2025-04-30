---
type: daily note
---
### [[<% tp.date.now("MM-DD-YYYY", -1, tp.file.title,"MM-DD-YYYY") %>|Yesterday]]
### [[<% tp.date.now("MM-DD-YYYY", 1, tp.file.title,"MM-DD-YYYY") %>|Tomorrow]]

# Agenda



# Meetings
```dataview
TABLE file.frontmatter.start as "Start time", summary AS "Summary"
FROM "Extras/Meetings" where contains(file.name, this.file.name)
SORT file.frontmatter.date 
```

# Notes from today
```dataview
TABLE 
  file.name as "Name", 
  file.mtime as "Modified", 
  file.inlinks as "Inlinks", 
  file.outlinks as "Outlinks", 
  file.tags as "Tags"
WHERE file.cday = this.file.cday
  and !contains(file.path, "Daily Notes") 
  and !contains(file.path, "Extras/Meetings")

```