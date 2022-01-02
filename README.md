# obsidian-templates

"`templater`" templates I use for obsidian and zettelkasten.

## Plugins

- Disable built-in core template plugin
- Install
  - [Calendar](obsidian://show-plugin?id=calendar): https://github.com/liamcain/obsidian-calendar-plugin
  - [Periodic Notes](obsidian://show-plugin?id=periodic-notes): https://github.com/liamcain/obsidian-periodic-notes
  - [Templater](obsidian://show-plugin?id=templater-obsidian): https://github.com/SilentVoid13/Templater

## Setup

### Calendar

- Enable "Show week number" so you can create a weekly note by clicking on the week number
  - Notes will be auto created with the files you specify in `Periodic Notes`
    - My calendar week numbers are not labeled accoring to ISO 8601,
      but when I click on the week number to create the note,
      the template creates the correctly named ISO week number.
  - You can maybe fix the calendar week numbering by overriding the locale setting?

### Periodic Notes

- Enable all the notes under the `Periodic Notes` plugin settings and point to these template files
- I kept the default file format names, exept for the "Weekly Notes" section
  - Weekly Notes Format uses `WW` for ISO week number: `YYYY-[W]WW`
