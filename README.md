# MINDLOOM FEATURES (v1.62.0)

https://healeychris.github.io/MindLoom/

USER GUIDE: see the docs folder (index.html), published with GitHub Pages. It covers every feature with screenshots,
step-by-step recipes, example maps (docs/examples) and a technical reference.


WHAT'S NEW IN 1.62.0

Zones: labelled, coloured boxes behind the nodes, for layers or groups such as a Windows CA or Security controls
  Add one from Tidy > Zones > Add zone, or right-click empty canvas, or select nodes and choose Zone around selection
  Drag the title bar to move the zone with the nodes inside it. Drag the corner to resize. Double-click the title to rename
  Right-click the title for Fit to contents, Tidy contents, colour and Delete zone. The nodes are never deleted with a zone
  Tidy (whole map) arranges each zone's nodes inside that zone and the rest of the map as usual
  Zones appear in PNG and SVG exports. A map with no zones is saved exactly as before. See "Zones" in the User Guide

EARLIER IN 1.61.2

Two new Tidy layouts, for the whole map or the selected branch (Tidy menu, and the right-click Tidy branch menu):
  Radial (fan out): the top node in the middle, branches fanning out around it like a classic mind map. Good for presenting a topic
  Layered flow: columns from left to right, so whatever leads to a node (its parent, dependencies and cross-links) sits to its left. Good for processes
Right-click menu is more compact on a mouse, and has a Tidy branch menu in the Branch section
Map files made by other tools can ask to be tidied when opened ("tidyOnOpen"). Your own maps are never rearranged on open

EARLIER IN 1.61

When done (right-click a top-level node): choose what happens to the completed items in that list only. Click again for the next choice
  Keep: they stay where they are (as before)
  Move to Done: they move, with anything beneath them, into a folded Done node under the list. Nothing is lost. Set an item's status back and it returns
  Fade: they stay in place, dimmed and struck through
  Hide: they are hidden, for this list only
  Handy for a to-do list next to a plan on the same map. Hidden by Simple Menus. See "When done" in the User Guide

EARLIER IN 1.60

Continue last session reconnects your file (Edge and Chrome): Ctrl+S, auto-save and Shared map carry on writing to the file you last saved.
  The start screen card says which file. If the file changed after your last edit here, MindLoom opens the file instead and tells you
Drag a file onto the window to open it: a .json map opens, a .csv or .md file is imported into the open map
Deleting several nodes no longer asks first. A message says what was deleted, with an Undo button
The save badge reads "Not saved to a file" with a Save button until the map is in a file
The Date Axis shows a hint when nothing on the map has a date yet
A tidier About box: core features, shortcuts and tips on three tabs
One-page cheat sheet to print: docs/cheatsheet.html (or docs/MindLoom-cheatsheet.pdf), also linked from About and the User Guide
Behind the scenes: every undoable edit now goes through one route, and the app has a 650 KB size budget

EARLIER IN 1.58

Start screen: MindLoom opens on a gallery of ready-made maps. Pick one, choose Continue last session, or Open existing map. Untick Show on startup to skip it
Templates (File > New from template): Blank, Mind map, Programme roadmap, Risk and issue tree, Stakeholders and RACI, Workshop, Requirements trace and
  Application landscape. Save your own with File > Save as template. Each one opens laid out so you can see what the map is for
Map types: a chip beside the views sets the kind of map (Plan, Mind map, Workshop, Stakeholders, Application landscape). It tidies the toolbar to the
  views that suit that kind of map. Nothing is switched off: everything is still in the View menu and Ctrl+K
Workshop mode (Settings): capture a meeting live into an Inbox of sticky notes, then drag each one onto a theme
Coverage (View > Coverage): a docked panel that checks the map is connected the way you expect, for example every requirement has a test. Gaps are ringed on the map
Stakeholders and RACI: people as pills with initials and role, R, A, C and I links with letter badges, a key, a warning for a deliverable with no Accountable,
  and View > RACI matrix. Press R, A, C or I while drawing a link to set its type
Application landscape turns Application Mapping Structures on while you use it
Auto-save to file switches on by itself the first time you Save. Switching on Shared map now explains first that the file must be in a synced folder
Saved Views have moved off the toolbar (still in the View menu, and V). Presentation mode has been removed
All of the above is hidden by Simple Menus where it is a specialist feature, and off until you use it. See the User Guide

EARLIER IN 1.42

Shared map (File > Shared map, Edge and Chrome, off by default): people who keep one map file in a synced folder (OneDrive, for example)
  get each other's changes merged in automatically, about every 15 seconds and when they save
  Everyone opens the shared file, then switches Shared map on. The same field-by-field rules as Merge from file apply
  It waits while you type or drag, never adds Undo steps for others' changes, and leaves an unreadable file alone
  See "Shared map" in the User Guide

EARLIER IN 1.41

Merge from file (File > Import > Merge from file): combine another copy of a map, from a colleague or a OneDrive duplicate, into yours.
  A preview shows what will be added, updated or deleted before anything changes, and the merge is one undo step
  Item by item, field by field: if one person changes an owner and the other a due date, both changes are kept
  The same result whichever of you does the merge. Needs files saved by 1.40 or later for the best result
  Not merged: saved views, baselines, bookmarks, colour names and settings. Yours stay as they are
  See "Merging two copies of a map" in the User Guide

EARLIER IN 1.40

Nothing changes in how MindLoom looks or works. This release rebuilds the inside of the app so future updates are quicker and safer
Undo uses far less memory on large maps
File format 6: each node now carries an id, a last-changed time and (if you set your name) who changed it, and the map keeps a list
  of recently deleted nodes. This is groundwork for merging two people's copies of a map in a later release.
  Files from earlier versions open normally. MindLoom 1.38 and earlier open a format 6 file with a notice
Development (source files, build tool and tests) now lives in a separate repository; this one holds the app you download

EARLIER IN 1.38

Simple Menus (Settings): hides the specialist items from the menus and toolbar, off by default. Ctrl+K still finds every command
User Guide link: File > User Guide and the About screen open the online guide (only when clicked; MindLoom never goes online by itself)

EARLIER IN 1.37

Quick capture (key Q, or Edit > Quick capture): a one-line box that adds a task under an Inbox node without choosing where.
  Add #tags, an @owner and a trailing date (today, tomorrow, fri, +2w, 27/11) in the same line; a live preview shows
  what it understood and each capture is one undo step
Renamable colour categories: double-click a colour on the colour bar, or use View > Panels > Legend / Rename Colours.
  Pick a ready-made label set (Task status, RAG, Workstream) or Reset to the original names. Names are saved with the map
Export SVG (vector image, editable in PowerPoint or Inkscape) and Export presets (File > Export > Export Presets)
Details Layout (Settings): Classic, Sections or Property List for the details panel

APPLICATION MAPPING STRUCTURES (OPTIONAL, OFF BY DEFAULT)

Settings > Application Mapping Structures turns it on for the current map (saved in the file). While it is off
nothing changes on screen. When on:
  Link types on cross-links (builds from, deploys to, authenticates via, ...) with colours and a note
  Migration wave per node (Wave 1 to 8, stored as a tag)
  Impact view: right-click > Show impact, or View > Dependencies. Highlights everything that relies on a
    node (direct and indirect), what it relies on, and checks owners and wave order
  Dependency check: nodes with no links, no owner or no wave, and waves that look out of order
A relation reads "A relies on B": a dependency (A waits for B) or a cross-link drawn from A to B.

MAPPING AND EDITING

Mind map canvas with unlimited nodes, add child (Tab) and add sibling (Enter)
Edit in place (F2), delete, duplicate subtree, detach a branch as its own root
Add several nodes at once (Edit menu or right-click): paste or type a list, one node per line,
  indent to nest, then add as separate roots or under the selected node
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
Activity and comments (optional, off by default; Settings > Editing > Advanced Activity & Comments, saved per map). When on, each item keeps a history of changes to status, start date, due date and owner, plus typed comments. Moving a single due date asks for a reason (Dependency, Scope change, Resourcing, Client request, or your own). Open it with the speech-bubble button next to Dependencies in the details panel, or the comment chip on a node. Quick repeat edits merge into one entry, the newest 50 are kept per node, and the status report shows the reason for a moved date and the latest note. Settings > Editing > Your name signs entries (kept in the browser). Turning it off hides the history but keeps it in the file

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
Save, Save As and Load as a JSON file. The file records its format and version (currently 5), and keeps baselines, the report snapshot and the activity history. Older files open normally; older versions of MindLoom ignore the new parts and would drop them if they saved the file
Auto-save to your file, using the File System Access API, with the save status shown
Export to CSV, Markdown and PNG
Import from CSV and Markdown
Print (Ctrl+P)

SETTINGS AND INTERFACE

Light and dark theme
Hover popups on or off (off by default)
Highlight Selection: fade everything unrelated to the selected node and show only its own links and dependencies
Grouped toolbar with menus: File, Edit, View, Link, Tidy, Settings (grouped into Appearance, Editing and Planning, with the Date Axis options in their own submenu)
Close (×) buttons on every panel
Phone layout: quick-action bar at the bottom (add, child, sibling, link, views)
Works fully offline as a single HTML file with no dependencies

DEMO DATA

Five built-in demos, including the Annual Roadmap, which uses the Date Axis. Open About, click the version number 5 times, then choose Demo data.

UPDATES
About > "Check for updates" looks up the latest version on GitHub (reads version.json in this repo). It runs only when you click it; the app never checks by itself, so it stays fully offline otherwise. Maintainers: bump version.json when publishing a release.

RIGHT-CLICK MENU
Grouped as Edit details / Rename / Bookmark, then Add, Connect, Branch (collapse, copy, cut, paste, duplicate, shift dates, detach) and Delete.
