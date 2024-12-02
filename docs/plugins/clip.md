---
title: Clipboard Manager
parent: Plugins
nav_order: 1
---

# Clipboard Manager


The Clipboard Manager allows users to store and reuse copied content, enhancing productivity. It detects different types of text, such as URLs, email addresses, math expressions, and code. Select an entry and press `Enter` to paste it.

<img src="{{ "/assets/images/Plugin_Clip.png" | prepend: site.baseurl | prepend: site.url}}"/>

## Entry Types
To try out the different types of entries, you can copy the following list items:

- Plain text: Hello World
- Email addresses: mailadress@provider.com
- URLs: https://maps.app.goo.gl/qZRNZJkDTBcgfEd96
- Math: f(x)=x^2, f:\mathbb{R}\mapsto\mathbb{R}
- Code: `console.log('Hello World')`
- Images:

<img src="https://images.pexels.com/photos/1714205/pexels-photo-1714205.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">

Different Entry types offer different actions after pressing the menu buttons.

### Actions by Entry Type
#### URL Entries
These actions are available for entries recognized as URLs.

* **Paste as Scientific Reference**
    
  Generates a formatted scientific citation from the URL metadata and pastes it into the clipboard. Requires title, author, and publication date.

* **Paste as BibTeX**

  Converts URL metadata into a BibTeX entry and pastes it into the clipboard. Requires title and author information.

* **Open Link in Browser**

    Opens the URL in the system's default web browser.

* **Insert with Link Text**

	Inserts the URL as an HTML anchor tag with alternative text.

* **Paste as Markdown**

	Formats the URL with alternative text as a Markdown link and pastes it into the clipboard.

#### Email Entries
These actions are available for entries identified as email addresses.

* **Send Mail to [email address]**

	Opens the default email client to compose a message to the email address.
#### Math Entries
These actions are for entries containing mathematical expressions.

* **Paste as Unicode**

	Converts the math expression into a readable Unicode format and pastes it into the clipboard.
#### Files and Images
These actions are for entries that include file paths or image data.

* **Open with Default Application**

	Opens the file or image using the system's default application.

* **Open with ...**

	Prompts the user to select an application to open the file or image.

* **Show in File Explorer**

	Opens the file's location in the system's file explorer.

#### General Text Entries
   These actions apply to all text entries.

* **Paste as Plain-text**

	Pastes the content as plain text without any formatting.

* **Paste as Markdown**

	Converts HTML content into Markdown format and pastes it.

## Tips
Use the star icon to favorite clipboard entries. Favorited entries will remain saved even after restarting your system. You can delete entries by pressing the trashcan icon.


## Keyboard Shortcuts
You can quickly access the Clipboard Manager by pressing `Super` + `V` by default. You can adjust this hotkey in the Settings.

Access the context menu by pressing `Shift`+`Enter` clicking the three dots, or right-clicking on the entries. The menu provides different actions based on the type of clipboard entry.

Press `Alt` along with the numbers `1-9` to paste a specific entry. Indicators will appear while you hold `Alt`.