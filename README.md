# obsidian-templates

"`templater`" templates I use for obsidian and zettelkasten.

## Plugins

- [Calendar](obsidian://show-plugin?id=calendar): https://github.com/liamcain/obsidian-calendar-plugin
- [Periodic Notes](obsidian://show-plugin?id=periodic-notes): https://github.com/liamcain/obsidian-periodic-notes
- [Templater](obsidian://show-plugin?id=templater-obsidian): https://github.com/SilentVoid13/Templater

## Setup

- Put the templates into a separate template folder that you will link in the plubins.
- Create a folder for your periodic notes

### Templater

- Disable built-in core template plugin
- Enable "Trigger Tamplater on new file creation"

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
- I have a folder name `000-Periodic Notes` so all my periodic notes sort to the top of the folder view
  - If you want subfolders for each kind of periodic note, and still have the notes count properly with the Calendar plugin
    - You can overide the year formating with the [square brackets] to specify exact folder/file name
    - Daily Notes
      - Format: `/YYYY/[Daily Notes]/MM/YYYY-MM-DD`
      - Template: `ze-templates/template-periodic-010-daily_notes.md`
      - Folder: `000-Periodic Notes`
    - Weekly Notes
      - Format: `/YYYY/[Weekly Notes]/YYYY-[W]WW`
      - Template: `ze-templates/template-periodic-020-weekly_notes.md`
      - Folder: `000-Periodic Notes`
    - Monthly Notes
      - Format: `/YYYY/[Monthly Notes]/YYYY-MM`
      - Template: `ze-templates/template-periodic-030-monthly_notes.md`
      - Folder: `000-Periodic Notes`
    - Quarterly Notes
      - Format: `/YYYY/YYYY-[Q]Q`
      - Template: `ze-templates/template-periodic-040-quartly_notes.md`
      - Folder: `000-Periodic Notes`
    - Yearly Notes
      - Format: `/[Yearly Notes]/YYYY`
      - Template: `ze-templates/template-periodic-050-yearly_notes.md`
      - Folder: `000-Periodic Notes`
