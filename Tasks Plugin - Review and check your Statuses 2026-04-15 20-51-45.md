# Review and check your Statuses

## About this file

This file was created by the Obsidian Tasks plugin (version 7.23.1) to help visualise the task statuses in this vault.

If you change the Tasks status settings, you can get an updated report by:

- Going to `Settings` -> `Tasks`.
- Clicking on `Review and check your Statuses`.

You can delete this file any time.

## Status Settings

<!--
Switch to Live Preview or Reading Mode to see the table.
If there are any Markdown formatting characters in status names, such as '*' or '_',
Obsidian may only render the table correctly in Reading Mode.
-->

These are the status values in the Core and Custom statuses sections.

| Status Symbol | Next Status Symbol | Status Name | Status Type | Problems (if any) |
| ----- | ----- | ----- | ----- | ----- |
| `space` | `x` | Todo | `TODO` |  |
| `x` | `space` | Done | `DONE` |  |
| `/` | `x` | In Progress | `IN_PROGRESS` |  |
| `-` | `space` | Cancelled | `CANCELLED` |  |
| `space` | `x` | incomplete | `TODO` | Duplicate symbol '`space`': this status will be ignored. |
| `x` | `space` | complete / done | `DONE` | Duplicate symbol '`x`': this status will be ignored. |
| `-` | `space` | cancelled | `CANCELLED` | Duplicate symbol '`-`': this status will be ignored. |
| `>` | `x` | deferred | `TODO` |  |
| `/` | `x` | in progress, or half-done | `IN_PROGRESS` | Duplicate symbol '`/`': this status will be ignored. |
| `!` | `x` | Important | `TODO` |  |
| `?` | `x` | question | `TODO` |  |
| `R` | `x` | review | `TODO` |  |
| `+` | `x` | Inbox / task that should be processed later | `TODO` |  |
| `b` | `x` | bookmark | `TODO` |  |
| `B` | `x` | brainstorm | `TODO` |  |
| `D` | `x` | deferred or scheduled | `TODO` |  |
| `I` | `x` | Info | `TODO` |  |
| `i` | `x` | idea | `TODO` |  |
| `N` | `x` | note | `TODO` |  |
| `Q` | `x` | quote | `TODO` |  |
| `W` | `x` | win / success / reward | `TODO` |  |
| `P` | `x` | pro | `TODO` |  |
| `C` | `x` | con | `TODO` |  |

## Loaded Settings

<!-- Switch to Live Preview or Reading Mode to see the diagram. -->

These are the settings actually used by Tasks.

```mermaid
flowchart LR

classDef TODO        stroke:#f33,stroke-width:3px;
classDef DONE        stroke:#0c0,stroke-width:3px;
classDef IN_PROGRESS stroke:#fa0,stroke-width:3px;
classDef CANCELLED   stroke:#ddd,stroke-width:3px;
classDef NON_TASK    stroke:#99e,stroke-width:3px;
classDef ON_HOLD     stroke:#00f,stroke-width:3px;

1["'Todo'<br>[ ] -> [x]<br>(TODO)"]:::TODO
2["'Done'<br>[x] -> [ ]<br>(DONE)"]:::DONE
3["'In Progress'<br>[/] -> [x]<br>(IN_PROGRESS)"]:::IN_PROGRESS
4["'Cancelled'<br>[-] -> [ ]<br>(CANCELLED)"]:::CANCELLED
5["'deferred'<br>[&gt;] -> [x]<br>(TODO)"]:::TODO
6["'Important'<br>[!] -> [x]<br>(TODO)"]:::TODO
7["'question'<br>[?] -> [x]<br>(TODO)"]:::TODO
8["'review'<br>[R] -> [x]<br>(TODO)"]:::TODO
9["'Inbox / task that should be processed later'<br>[+] -> [x]<br>(TODO)"]:::TODO
10["'bookmark'<br>[b] -> [x]<br>(TODO)"]:::TODO
11["'brainstorm'<br>[B] -> [x]<br>(TODO)"]:::TODO
12["'deferred or scheduled'<br>[D] -> [x]<br>(TODO)"]:::TODO
13["'Info'<br>[I] -> [x]<br>(TODO)"]:::TODO
14["'idea'<br>[i] -> [x]<br>(TODO)"]:::TODO
15["'note'<br>[N] -> [x]<br>(TODO)"]:::TODO
16["'quote'<br>[Q] -> [x]<br>(TODO)"]:::TODO
17["'win / success / reward'<br>[W] -> [x]<br>(TODO)"]:::TODO
18["'pro'<br>[P] -> [x]<br>(TODO)"]:::TODO
19["'con'<br>[C] -> [x]<br>(TODO)"]:::TODO
1 --> 2
2 --> 1
3 --> 2
4 --> 1
5 --> 2
6 --> 2
7 --> 2
8 --> 2
9 --> 2
10 --> 2
11 --> 2
12 --> 2
13 --> 2
14 --> 2
15 --> 2
16 --> 2
17 --> 2
18 --> 2
19 --> 2

linkStyle default stroke:gray
```


## Sample Tasks

Here is one example task line for each of the statuses actually used by tasks, for you to experiment with.

The status symbols and names in the task descriptions were correct when this file was created.

If you have modified the sample tasks since they were created, you can see the current status types and names in the group headings in the Tasks search below.

> [!Tip] Tip: If all your checkboxes look the same...
> If all the checkboxes look the same in Reading Mode or Live Preview, see [Style custom statuses](https://publish.obsidian.md/tasks/How+To/Style+custom+statuses) for how to select a theme or CSS snippet to style your statuses.

- [ ] Sample task 1: status symbol=`space` status name='Todo'
- [x] Sample task 2: status symbol=`x` status name='Done'
- [/] Sample task 3: status symbol=`/` status name='In Progress'
- [-] Sample task 4: status symbol=`-` status name='Cancelled'
- [>] Sample task 5: status symbol=`>` status name='deferred'
- [!] Sample task 6: status symbol=`!` status name='Important'
- [?] Sample task 7: status symbol=`?` status name='question'
- [R] Sample task 8: status symbol=`R` status name='review'
- [+] Sample task 9: status symbol=`+` status name='Inbox / task that should be processed later'
- [b] Sample task 10: status symbol=`b` status name='bookmark'
- [B] Sample task 11: status symbol=`B` status name='brainstorm'
- [D] Sample task 12: status symbol=`D` status name='deferred or scheduled'
- [I] Sample task 13: status symbol=`I` status name='Info'
- [i] Sample task 14: status symbol=`i` status name='idea'
- [N] Sample task 15: status symbol=`N` status name='note'
- [Q] Sample task 16: status symbol=`Q` status name='quote'
- [W] Sample task 17: status symbol=`W` status name='win / success / reward'
- [P] Sample task 18: status symbol=`P` status name='pro'
- [C] Sample task 19: status symbol=`C` status name='con'

## Search the Sample Tasks

This Tasks search shows all the tasks in this file, grouped by their status type and status name.

```tasks
path includes {{query.file.path}}
group by status.type
group by status.name
sort by function task.lineNumber
hide postpone button
short mode
```
