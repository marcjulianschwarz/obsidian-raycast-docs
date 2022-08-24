# Preferences

## Search Note

### Excluding Folders

This text field can be filled with a comma-separated list of folders that should be excluded from the search.

For example hiding the folders `References`, `These Notes should be excluded` and `Another Folder` can be excluded with the following list:

```
References, These Notes should be excluded, Another Folder
```

### Hide Content

Activating one of these options will hide them from Quick Look and in all [Copy and Paste](search-note-command/copy-note) actions. The YAML frontmatter and LaTeX options will hide the entire content while hiding links will only remove the brackets around links.

- Hide YAML frontmatter
- Hide LaTeX
- Hide Links (`[[some link]]` -> `some link`)

### Template for Append Action

The template for the Append Action supports all templates.

```
- {timestamp} [URL]({content})
```

If action is invoked with the content `https://www.raycast.com` then the appended text will look like this:

```
- 1661326048 [URL](https://www.raycast.com)
```

### Template for Append Selected Text Action

### Show Detail

Enabeling this option will show the notes content on the right side.

![Search Command Detail](/img/search_command_detail.png)

### Show Metadata

Enabeling this option will show the notes metadata on the right side.

It consists of:

- Character Count
- Word Count
- Reading Time (in minutes)
- Creation Date
- File Size
- Note Path
- A list of tags (if note contains tags)
- A link to open a URL (if note contains `url` key in YAML frontmatter)

:::warning Show Detail has to be activated

The metadata will only be visible when the **Show Detail** option has been enabled.

:::


### Search Content

Enabeling this option will make Raycast search through the entire content of every note in your vault. This makes it easier to find notes where the title of it is unknown.


### Primary Action

- Quick Look
- Open in Obsidian
- Open in new Pane