# SVG-comic-reader

The SVG comic reader is an SVG file that allows you to read comics using a bit of Java-Script embedded into the file. It is licensed with GPL 3.0.

I made this file because I was annoyed with how most online comic reading things have you reload the webpage each time. Furthermore, it is difficult to show spreads, or to allow showing the whole page in one go. It has had a plain HTML based ancestor before it, but eventually I wanted to upgrade to SVG, because that is more scalable and easier to edit with Inkscape to boot. The Javascript is raw javascript, not because I hate myself, but because the file should be possible to be completely stand-alone.

## Features:

It has several features, including:

* Easy editing with Inkscape: Every layer in the ‘pages’ layer in Inkscape is automatically determined to be a new page!
* Using SVG’s scaling to have the whole application scaled to the whole viewport. With that, it’s retina-proof.
* Automatically showing one or two pages depending on the aspect ratio of the webbrowser viewport. So that if you read on a tablet, portrait mode will give you 1 page, and landscape mode 2 pages!
* Allowing users to change the amount of pages visible at once, or let them turn off auto mode.
* Left to Right and Right to Left, fully configurable.
* Skipping to a certain page.
* First and Last page buttons
* Big buttons for skipping pages for touch based devices.
* Switching pages with the left and right keys on your keyboard.
* Taking meta-data from the Inkscape properties dialogue to fill up the info box with important information like the author, the date of publishing and of course a summary.
* Raw javascript, so no weird libraries from god-knows-where.

## How to use:

* Get the newest version of Inkscape!
* Open the file with Inkscape.
* In the pages layer, you can see a bunch of hidden layers. Each layer directly under the pages layer will become a new page, so just add a sublayer for that.
* When adding images, it is best to ‘embed’ them, so that the SVG will be standalone. Of course, you might have reasons to want to easily access the pages on your server, so ‘linking’ them is also perfectly possible, just make sure you keep the relative paths.
* You can edit the UI elements to look prettier. Just do not delete them or rename their ID.
* For meta-data, use the document properties and then go into Meta-data.
* Also check the license section. The file is marked with ‘GPL3.0’, which is necessary for you to edit the example content legally, but you might want to change it as it affects the images you put in.
* When done, upload to a webserver. Sadly, there are no services that allow you to upload SVGs with javascript to use like this file is used, so you will need to get hosting for this.
* If you wish to embed the SVG, use the object or frame tags, not the img tag, as that blocks javascript.
* Open in any of the recent webbrowsers(this file was made for webbrowsers 3 years ago, so that’s recent enough), and enjoy.