# shell-todo

A TODO list manager written in Bash. 

```
todo COMMAND [OPTIONS]
```
## Configuration

Environment variables:

* `SHELL_TODO_DIR` - The root directory for `todo` files. Defaults to `${HOME}/.config/shell-todo`

## Commands

Complete notes on `todo` subcommands.

### Command: add

Adds a new todo list item. The current date is automatically recorded.

Options:

```
-m MESSAGE     (required) the text of the todo item
-p PRIORITY    priority 1-9
-d DUE_DATE    due date for this item
```

### Command: show

Options:

```
-v            turn on verbose output
INTEGER       show entry with given ID verbosely
```

### Command: remove

Removes an entry with a given ID

Options:

```
INTEGER      The ID of the entry to be removed
```

### Command: mark (unmark)

Marks or unmarks an entry with a given ID. Mark will add a checkmark and unmark will remove it.

Options:

```
INTEGER      The ID of the entry to be marked (unmarked)
```

### Command: switch

Switch the currently selected todo list. If no PROJECT is specified then the list of active PROJECTS is listed with teh currently selected PROJECT marked with a star.

Options:

```
PROJECT        switch to this PROJECT
```