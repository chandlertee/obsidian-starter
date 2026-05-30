# obsidian-starter

A small, opinionated starter for Obsidian. Four community plugins, a handful of templates, and a few Dataview-powered index pages. Designed to be cloned, set up once, and used as a daily-notes / PKM base.

## What's in here

- **`Templates/`** — the working templates. `Person Template.md` and `Meeting Template.md` use Dataview to surface mentions, tasks, and meetings on each person's page. Wikilink someone in any note and their Person page picks it up.
- **`Templates/Periodic/`** — daily, weekly, and monthly note templates. Ships with a clean default (Focus / Notes / Reflection) and a `(Gamified)` variant in the same folder that uses an RPG framing (Campfire Prep, Long Rest, Quests, Allies, Traps). Point Periodic Notes at whichever you prefer.
- **`Atlas/`** — Map-of-Contents pages built on Dataview. `People Map` lists every Person note with company / role / location columns; `Meetings Map` lists every meeting by date. Both update automatically as you add notes.
- **`Cheatsheets/`** — quick reference (Markdown Basics).
- **`Home.md`** — vault landing page with Atlas list + an open-tasks query.

## Plugins

Install these from Community Plugins:

- **Templater** — date math and dynamic title insertion in templates.
- **Dataview** — query engine. Powers the Person, Meeting, Atlas, and Home queries.
- **Calendar** — sidebar calendar for jumping between periodic notes.
- **Periodic Notes** — daily, weekly, and monthly note support. Replaces Obsidian's core Daily Notes.

## Setup

1. **Calendar**
   - In Calendar settings, toggle on `Show Week Numbers`.

2. **Periodic Notes**
   - Toggle on Daily Notes, Weekly Notes, and Monthly Notes (Quarterly and Yearly are off by default).
   - For each, set:
     - Daily: template `Templates/Periodic/Daily Note Template`, folder `Journal/Daily`
     - Weekly: template `Templates/Periodic/Weekly Note Template`, folder `Journal/Weekly`
     - Monthly: template `Templates/Periodic/Monthly Note Template`, folder `Journal/Monthly`
   - Turn off the core **Daily Notes** plugin: Obsidian Settings → Core Plugins → toggle Daily Notes off.

3. **Templater**
   - Set Template folder location to `Templates`.
   - Toggle on `Automatic jump to cursor`.
   - Toggle on `Trigger Templater on new file creation` (so periodic notes auto-populate).
   - Folder Templates:
     - Add `People` → `Person Template`. Creating `People/Alice` will scaffold a Person note.
     - Add `Meetings` → `Meeting Template`. Same idea for meetings.
   - Turn off the core **Templates** plugin: Obsidian Settings → Core Plugins → toggle Templates off.

4. **Dataview**
   - Toggle on `Automatic task completion tracking`.
   - Toggle on `Use emoji shorthand for completion`.
   - Toggle on `Recursive sub-task completion`.
   - Toggle on `Enable inline Dataview` if you want `=` queries mid-paragraph.

### Optional

- **Use the Gamified periodic templates.** In Periodic Notes settings, point Daily / Weekly / Monthly at the `(Gamified)` files instead of the defaults.
- **Templater file titles.** Obsidian Settings → Appearance → toggle off `Show inline title`. The template's H1 (which Templater fills with the file title) then serves as the visible title without duplication.
- **Hide Templates from search and graph.** Obsidian Settings → Files and Links → Excluded Files → add `Templates`.

## How the Dataview pieces fit together

The Person template's Mentions, Tasks, and Meetings sections all use the same idea: Dataview's `[[]]` shorthand for "the current note." Any note that wikilinks the person shows up under Mentions; tasks naming them show up under Tasks; meetings linking them show up under Meetings. No special inline fields. Just wikilink people in your daily notes and the views populate.

The Atlas pages do the same for whole folders. Drop in a Person note, and `Atlas/People Map.md` lists them on the next refresh.
