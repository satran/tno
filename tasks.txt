# Tasks
Tasks are stuffs you want to do. A task consists of a title and a body. The format is as such:

    * [STATE] TITLE PROPERTIES 
      BODY

### STATE
- ` `: the task is pending
- `x`: the task is done
You can add custom state to show progress of a task. For example you can simulate a Kanban board using the following states: [ ], [doing], and [x].

### TITLE
Title can be any string. 

### PROPERTIES
Properties are key:value pairs. No space is allowed in both key or value. Here are some predefined keys:
- due: when a task is due
- done: when a task was competed. 

### BODY
Body is all text that is indented by a minimum of 2 spaces. Two spaces allow it to be nicely aligned to `[`. Body can contain nested tasks.

### Example

The following shows an example task.
```
* [ ] Write the spec for tasks due:31/12/2018
  Ensure the spec is defined in markdown so I can generate HTML files.
  * [x] Write a draft
  * [ ] Define syntax
```

