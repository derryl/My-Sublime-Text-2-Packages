# HTML code formatter for Sublime Text 2
#### [Sublime Text 2](http://www.sublimetext.com/2)
#### [HTML Tidy](http://tidy.sourceforge.net/)

## About
This is a Sublime Text 2 plugin allowing you to clean and tidy up your HTML code. 

It uses a version of `tidy`, which comes bundled with PHP 5.

On OS X and Linux it will use `/usr/bin/php`. Windows depends on `tidy.exe` (bundled) or `php.exe` being available in your `PATH`. See requirements below. *Windows support is still beta.*

Dedicated to Jeffrey Way @envatowebdev

## Usage
`ctrl + shift + P` and type `Tidy HTML`, or you can set up your own keybinding as shown below.

## Customize
You can customize a growing number of options in HtmlTidy.sublime-settings.

Open `Preferences -> Package Settings -> HtmlTidy -> Settings - Default` to see the available options.

Then open `Preferences -> Package Settings -> HtmlTidy -> Settings - User` (which will be empty on the first time), copy the default settings and start to modify them.

To set up a custom keybinding, you can insert the following line into your `Default.sublime-keymap`:

`{ "keys": ["ctrl+alt+t"], "command": "html_tidy"}`

## Requirements

On OS X and Linux you need to have PHP5 installed at `/usr/bin/php`. This should be the case at nearly every modern system.

For Windows, The bundled `win/tidy.exe` is used. If you delete it,you need to have PHP5 installed somewhere where HtmlTidy can find it, i.e. in your `PATH`. If you can run `php.exe -v` from the windows command line, all should be fine. If not, and you are sure you have PHP installed, please contact me or file an issue.

## Install

### Package Control

The easiest way to install this is with [Package Control](http://wbond.net/sublime\_packages/package\_control).

 * If you just went and installed Package Control, you probably need to restart Sublime Text 2 before doing this next bit.
 * Bring up the Command Palette (Command+Shift+p on OS X, Control+Shift+p on Linux/Windows).
 * Select "Package Control: Install Package" (it'll take a few seconds)
 * Select HtmlTidy when the list appears.

Package Control will automatically keep HtmlTidy up to date with the latest version.

If you have some problems or improvements with it, contact me via GitHub.
