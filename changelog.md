
## [0.5.0] - 2025-12-13
### Updated
- Removed ActiveTab permissions because we actually didn't need it.
- Added support for Firefox. This is the first version (0.5.0) that has been uploaded to the Mozilla Developer Hub, pending approval by the Mozilla security team.
- **Calendar:** 
	- Fixed bug where empty/erased notes were showing up in the grid, even if the note had 0 characters in it. 
- **Notes (side panel)**
	- Fixed bug: Empty/erased notes were showing up in the grid, even if the note had 0 characters in it (similar bug as the calendar since both are linked).
	- Fixed bug: Really long strings of text (e.g. an API key) were breaking the note flyout panel. 
	- Changed the date sorting language to be more clear.
- **Popup**
	- Redesigned popup entirely. Added some visual feedback once successfully adding a todo item. 
	- Better color/theme management so it matches your defined color scheme
- To Do
	- Changed "Done" to "Completed", based on user feedback, this was clearer language.
- **Draw**
	- Better canvas/art sizing to work on screens big and small. Still refining this. 
### Added
- Timezone planner: 
	- Added better differentiation between each day on the actual timeline. 11pm and 12am receive a special styling to indicate end of day/beginning of day.
- Bookmarks:
	- New emoji selector when adding a bookmark. I've included [Emojimart](https://github.com/missive/emoji-mart) which will likely be used elsewhere in the app (future plans for adding emoji elsewhere)
### Known Issues
- Unable to add hyperlinked text (CMD+K) when creating a To do item.
- Unfinished features exist in the codebase, but hidden: RSS reader and Date calculator
- Strange behavior when searching for tags while the **tag dropdown menu** is anchored from a position lower than itself. 
- Ongoing: **UI polish** needed in various places.
- Note input **inherits page styling** from pasted sources. Not sure why it's doing that.

## [0.4.0] - 2025-12-02 (Beta Release)
### Added
- Finally decided on a name: Tabba
- Launched to Chrome Web Store 🎉
- Did some testing + support for Microsoft Edge

### Known Issues
- Unable to add hyperlinked text (CMD+K) when creating a To do item.
- Unfinished (Alpha) features: RSS reader and Date calculator
- Design a better Popup (e.g. when you click the extension icon in the toolbar).
- Ongoing: UI polish needed in various places.

## [0.3.0] - 2025-11-29
### Added
- Core features of the extension:
	- Replaces default new tab screen
	- Always remembers your last-selected tab.
	- No user account required
	- All user data is stored on the user's local browser ([IndexedDB](https://web.dev/articles/indexeddb)) and not synced anywhere. Some settings are stored in chrome.storage.local for quick access (settings, last-selected tool, etc.)
	- Limited 3rd party dependencies: Currently just [Phosphor Icons Web](https://github.com/phosphor-icons/web). Absolutely no data tracking, analytics, etc.
- Calendar 
	- Hour-based grid with year/quarter/month/week views
- Notes
	- Hour-based note taking: Clicking an hour and typing creates a new note for that hour. 
	- Notes auto-save after a few seconds
	- Add tags to a note
	- Set a Note as "starred"
	- View all notes in a flyout panel
		- Notes are grouped by year → day → time
		- Sort notes
		- Filter notes by tag/starred status
- Tags
	- Added tagging functionality.
	- Tags are shared between Notes and To do items
	- Tag names can be edited in-situ or via Settings
- To do
	- Simple todo list: Add items and mark items as Done
	- Delete items
	- Sort options:
		- Manual (drag and drop)
		- Created: newest first or oldest first
	- Create filtered lists with Tags
- Symbols 
	- Copy/paste symbols
- Bookmarks
	- Save URLs as a clickable bookmark
	- When inputting a URL, the favicon is rendered, or replaced with an emoji
- Symbols
	- Click to copy and paste symbols
	- Optional: Remembers your Most Frequently used symbols for easy access (top row)
	- Search for symbols by name or keyword
	- Change the size of the grid
- Draw
	- Pixel/bitmap-inspired drawing tool (for relaxation and stress relief)
	- Change color and size (1x1 or 4x4) of the drawing tool
	- Change size of pixel grid
	- Export to PNG (1080x1080)
	- Save drawings to Gallery
	- Create folder of drawings in Gallery. Folder card thumbnails are dynamically generated showing the first 3 drawings of any folder.
	- Delete/bulk delete
- Settings
	- Basic settings panel for customization and config
	- Import/export data for backup. When importing, you now see a Success screen with the # of items successfully imported. 
	- Added some basic stats in the "Data" tab
- Hotkey support: 
	- `Esc` to close dialogs/panels
	- \` + 1, 2, 3, etc. to switch between tool tabs
- Date calculator (ALPHA)
	- Add/subtract dates
	- Count days in between two dates
	- Need to do more testing and ensure calculations are correct.
- RSS (ALPHA)
	- Basic RSS reader, but lacking many critical features. Not quite ready for the public use yet.
	- If this becomes too feature-intensive, might remove feature.
	- Use at your own risk.
- Time (BETA)
	- Simple analog clock
	- Mini hidden easter egg can be found by clicking the clock center.


## [0.2.0] - 2025-11-09
### Added
- Basic note taking
- Revamped design system to work off of variables, more scaleable
- Refreshed design



## [0.1.0] - 2024-11-02
### Added
- Clock/calendar grid: Designed and figured out the basic structure of how I want it to look/work.
- Settings:
	- Set custom hours on the calendar grid
	- Color customization: Set accent color, change grid colors