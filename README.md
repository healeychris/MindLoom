# MINDLOOM FEATURES (v1.29.0)

MAPPING AND EDITING

Mind map canvas with unlimited nodes, add child (Tab) and add sibling (Enter)
Edit in place (F2), delete, duplicate subtree, detach a branch as its own root
Copy, cut and paste whole branches (Ctrl+C, Ctrl+X, Ctrl+V), including between maps
Undo and redo
Collapse and expand branches, collapse all, expand all
Cross-links between any two nodes, with labels
Dependencies: "Depends on" and "Needed by", with cycle protection, arrows, and "Waiting on" badges
Multi-select
Snap to grid and lane bands
Curved or straight connectors

NODE DETAILS

Status: To do, Ongoing, Completed, Blocked, Awaiting and others. The date an item was completed is recorded, so reports show when work finished
Due dates and start dates, with quick buttons (Today, Tomorrow, +1 week, +2 weeks, +1 month) that work on whichever date field you click
Owner and tags
Notes and a movable details panel (drag its title bar, double-click to reset)
Optional sections, opened with buttons in the details panel (open by default when the node has content):
  Tags
  Checklist: tick-off items inside a node, with a count shown on the node
  Progress: % complete, shown as a bar on the node
  Repeat: recurring tasks (every n days, weeks, months or years). Completing one rolls its dates forward, ticks the checklist off and resets progress
Bookmarks, with quick jump

LAYOUT AND VIEWS

Horizontal tree and vertical tree, for the whole map or a single branch
Balanced tree (both sides), with the root in the middle and branches split left and right, for large maps
Tidy layout
Fit All, Centre, zoom, and a minimap
Focus Roots, to show only the roots you choose
Outline view (indented list)
Timeline (Gantt style)
Date Axis (next to Agenda and Timeline on the toolbar), which lays the map out along a calendar with months and quarters (Q1 to Q4). See DATE AXIS below.
Agenda (key A): a side panel grouping your tasks into Overdue, Due today, Next 7 days and Under way, with an owner filter. Tick a task to complete it, and tick checklist items inline
Board (kanban), with columns by status
Status report (key R): a ready-to-send summary, printable, with:
  A Red, Amber or Green health line that says what drove it
  An optional headline you type, which goes into the copy, download and print
  Changes since the last report: newly completed, newly overdue, newly blocked, date changes, new and removed items. Copy, Download and Print each save a snapshot for next time
  Against baseline: what has slipped, what is earlier, and what is on plan (see DATE AXIS)
  Sections for Overdue, Blocked, Awaiting, Waiting on prerequisites, Critical path, Due soon and Completed, with days overdue and checklist or progress on each line, and items that fit several sections written out once
  Filters by owner and project, for the whole map or a selected branch (root trees hidden with Focus are left out)
  Completion counted on tasks, not group headings, with a second figure that allows for checklists and progress
  Workload by owner
  Copy formatted (pastes as real headings and bullets into Outlook, Teams, Gmail or Word), Copy Markdown, Download .md and Print
Statistics and legend
Presentation mode

DATE AXIS

Critical path view: show only critical items with their context, with critical links highlighted
Slide view: a clean, labelled-lane layout for PowerPoint, with non-critical items dimmed, a legend, and high-resolution PNG export
Bars for items with a start and due date, markers for items with one date, grouped in swimlanes by workstream
Quarter and month headings, month gridlines, alternate quarter shading, and a Today line
Zoom buttons for Q1, Q2, Q3, Q4 and the whole Year, plus a Today button
Fold or unfold lanes, one at a time (the - and + button on a lane bar) or all at once (Fold lanes)
Lines setting: Off, Selected (only the selected node's links) or All
Bars coloured by workstream, with a status stripe on the left of each bar (Settings: Date Axis Bar Colours)
Nodes with no date are hidden, unless something dated sits beneath them. A button shows how many are hidden and brings them back
Lane names pinned to the left edge, and bar names that stay readable when the start of a bar is off-screen
Drag a bar to change its dates, or drag its ends to change the start or due date
Baselines (Baseline button, or Settings > Baselines): save every start and due date as a named plan, up to five. A dashed ghost then shows where each moved bar was planned, with the slip in days (+12d, -5d). The ghosts appear in PNG export and print, and the report lists what slipped
Automatic tidy so that nodes never overlap, and switching the axis off puts every node back where it was

FINDING THINGS

Search (/)
Filter bar (Ctrl+F)
Hide Completed
Saved Views (toolbar button), which store a named combination of filters, layout and view, and can be recalled at any time
Command palette (Ctrl+K), with recent commands, searches every action

DATES

Shift dates for a node, or for a branch plus its linked nodes, by a number of days

FILES AND SAVING

Saved automatically in the browser (localStorage), with rolling backups and a Restore backup option
The app always opens on a fresh map; your previous map is kept under File > Restore backup ("last session")
Save, Save As and Load as a JSON file. The file records its format and version (currently 4), and keeps baselines and the report snapshot. Older files open normally; older versions of MindLoom ignore the new parts and would drop them if they saved the file
Auto-save to your file, using the File System Access API, with the save status shown
Export to CSV, Markdown and PNG
Import from CSV and Markdown
Print (Ctrl+P)

SETTINGS AND INTERFACE

Light and dark theme
Hover popups on or off (off by default)
Highlight Selection: fade everything unrelated to the selected node and show only its own links and dependencies
Grouped toolbar with menus: File, Edit, View, Link, Tidy, Settings
Close (×) buttons on every panel
Phone layout: quick-action bar at the bottom (add, child, sibling, link, views)
Works fully offline as a single HTML file with no dependencies

DEMO DATA

Five built-in demos, including the Annual Roadmap, which uses the Date Axis. Open About, click the version number 5 times, then choose Demo data.
