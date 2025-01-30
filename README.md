# obsidian-starter
Cheatsheets and personal templates for Obsidian

### Setup 
1. Install Community Plugins
	1. Calendar
		1. Go to Calendar plugin settings and toggle on `Show Week Numbers`
	2. Periodic Notes
		1. After installation, toggle on the Daily Notes option
			1. Set the Daily Note template to `Templates/Periodic/Daily Note Template`
			2. Set the Note Folder location to `Journal/Daily` or other if desired
		2.  Toggle on the Weekly Notes option
			1. Set the Weekly Note template to `Templates/Periodic/Weekly Note Template`
			2. Set the Note Folder location to `Journal/Weekly` or other if desired
		3. Toggle on the Monthly Notes option
			1. Set the Monthly Note template to `Templates/Periodic/Monthly Note Template`
			2. Set the Note Folder location to `Journal/Montly` or other if desired
		4. Toggle off the Daily Notes core plugin
			1. Go to Obsidian Settings -> Core Plugins
			2. Toggle Daily Notes to Off
	3. Templater
		1. Set Template folder location to `Templates` or other desired location
		2. Toggle on `Automatic jump to cursor`
		3. Toggle on `Trigger Templater on new file creation`
			1. This will allow Templater to convert template tags when a new note is created, e.g., when a new Daily Note is created
		4. Update Templater Folder Templates
			1. In the plugin settings, find Folder Templates
			2. Add the `People` Directory to trigger the `People Template`
			3. This allows you to use Ctrl+O (Cmd+O), type in `People/Chandler` to create a new note in the People directory, and automatically trigger the People template
			4.  Add the `Meetings` Directory to trigger the `Meeting Template`
		5. Turn off the Templates core plugin
			1. Go to Obsidian Settings -> Core Plugins
			2. Toggle Templates to Off
	4. Dataview
		1. Toggle on `Automatic task completion tracking`
		2. Toggle on `Use emoji shorthand for completion`
		3. Toggle on `Recursive sub-task completion`
#### Using Templater for File Titles
1. Disable `Show inline title` in Obsidian Settings
	- Go to Obsidian Settings -> Appearance
	- Scroll down to Interface
	- Toggle to Off

#### Optional
- Remove `Templates` from Graph View and Search by adding the directory to Excluded Files in Obsidian Settings -> Files and Links -> Excluded Files