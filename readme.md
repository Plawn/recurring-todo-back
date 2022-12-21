
## Entities

### Task
```yaml
id: ID
name: string
description: string
parentTaskId: ID
```

### TaskProgressPoint
```yaml
id: ID
date: Date
taskId: ID
percentage: int(0 - 100)
```

### User

```yaml
id: ID
name: string
email: string
mainTaskId: ID
```

## Actions

### Create Task

### Update Task progress

### Delete Task for future

### Get progress of task


## How to 

- Each connection
- check if progress point was created for today
- if yes -> nothing
- if not
    - get all points for yesterday and creates the points for today


## Main view

- list of task with their progress

```yaml
# payload
task:
    id: ID
    name: string
    progress: int
    subTasks: [...task]
```