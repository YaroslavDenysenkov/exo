
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Fit|Daily Fit]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Learn|Daily Learn]]
- [[<% tp.file.path(true).split("/").slice(0,-1).join("/") %>/<% tp.date.now("YY-MM-DD") %> Daily Me|Daily Me]]

<%*
const date = tp.date.now("YY-MM-DD");
const folder = tp.file.folder(true);

async function createNote(templateName, fileName) {
  const existing = app.vault.getAbstractFileByPath(`${folder}/${fileName}.md`);
  if (!existing) {
    const template = tp.file.find_tfile(templateName);
    await tp.file.create_new(template, fileName, false, folder);
  }
}

await createNote("Daily Fit Template",   `${date} Daily Fit`);
await createNote("Daily Learn Template", `${date} Daily Learn`);
await createNote("Daily Me Template",    `${date} Daily Me`);
%>

## Tasks
### Overdue
```tasks
not done
due before 2026-01-01
path does not include 80 Back Office/Templates
```

### Due today
```tasks
not done
due on 2026-01-01
path does not include 80 Back Office/Templates
```

### Due in the next two weeks
```tasks
not done
due after 2026-01-01
due before 2026-01-15
path does not include 80 Back Office/Templates
```

### No due date
```tasks
not done
no due date
path does not include 80 Back Office/Templates
```

### Done today
```tasks
done on 2026-01-01
path does not include 80 Back Office/Templates
```