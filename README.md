<div align="center">
	<h1 align="center">z-startpage</h1>
	<p align="center"><img width=100% src="https://github.com/user-attachments/assets/c378a230-444b-4033-8f26-2eb1d0296049"></p>

This is an custom interactive start page for browsers, based on [Excalith Start Page](https://github.com/excalith/excalith-start-page).

</div>

## Demo

You can explore the working version [here](https://z-startpage.vercel.app/). 

> [!IMPORTANT]
> This is a demo version and will be updated regularly, which might break your configurations. It is not recommended for daily browsing. Please refer to the [Excalith wiki page](https://github.com/excalith/excalith-start-page/wiki/Getting-Started) for more information. Note that the Docker option will not work with z-startpage.

## Features

- Filter links by typing in the prompt
  - Quickly filter links by typing in the prompt. Hitting <kbd>Enter</kbd> will open all filtered links at once
  - If nothing filtered, the text in prompt will use the default search engine for searching your input
- Launch websites directly from the prompt. Just type the URL (ie. `github.com`)
- Search websites with custom commands. For example, type `s some weird bug` to search StackOverflow for `some weird bug`
- Wallpaper support through URL with blur and fade effects
- Terminal window opacity and translucency effects
- Customisable Fetch UI for fetching browser and system data, including custom image support
- Autosuggest and Autocomplete support just like `zsh` and `fish`
- Cycle through filtered links back and forth
- Built-in configuration editor to easily edit and save your configuration

Please refer to the [Exalith configuration](https://github.com/excalith/excalith-start-page/wiki/Configuration) page for more information.

### Built-In Commands

- Show usage with `help` command (shows basic usage and your configured search shortcuts)
- Show info with `fetch` command (time, date, system and browser data)
- Update your configuration with `config` command
  - `config help` - Displays config command usage
  - `config import <url>` - Imports a configuration from URL
  - `config theme` - Lists all [available themes](./data/themes/)
  - `config theme <theme-name>` - Switches between themes and sets your local configuration
  - `config edit` - Edit local configuration within editor
  - `config reset` - Reset your configuration to default

### Key Bindings

- Use <kbd>→</kbd> to auto-complete the suggestion
- Search without auto-complete with <kbd>CTRL</kbd> + <kbd>ENTER</kbd>
- Cycle through filtered links using <kbd>TAB</kbd> and <kbd>SHIFT</kbd> + <kbd>TAB</kbd>
- Clear the prompt quickly with <kbd>CTRL</kbd> + <kbd>C</kbd>
- Close windows with <kbd>ESC</kbd>

## Customisation

This project, at its heart, supports customisation to better suit your desktop environment. There are three methods to personalise the project according to your preferences:

You can either
- **Method 1:** Configure your **fork** by editing [settings.json](./data/settings.json) file
- **Method 2:** Use `config edit` command to edit on the fly, by built-in json editor
- **Method 3:** Use `config import <url>` command to import your remote config file from your dotfiles repository