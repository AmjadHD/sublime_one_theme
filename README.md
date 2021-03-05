# One Theme

A port of Atom's One Dark and One Light UI and Syntax Themes.

![screencast](./screencast.gif)

The package includes two color schemes `One Dark` and `One Light` in addition to an adaptive Theme.
Make sure to disable or remove any other color scheme with the same name, namely https://packagecontrol.io/packages/One%20Dark%20Color%20Scheme.

## Installation

[Package Control](https://packagecontrol.io/docs/usage)

## Preferences

Preferences for the closest look to atom, add to your user settings (if you wish).

```json
{
	"always_show_minimap_viewport": true,
	"animation_enabled": false,
	"caret_extra_bottom": 2,
	"caret_extra_top": 1,
	"caret_style": "blink",
	"enable_tab_scrolling": false,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"indent_guide_options": [
		"draw_normal",
		"solid"
	],
	"line_padding_bottom": 2,
	"line_padding_top": 1,
	"margin": 0
}
```

## Customization

See https://www.sublimetext.com/docs/themes.html#customization
Navigate to `Preferences > Package Settings > Theme One > Customize`

Here's a sample override:
```json
{
	"variables": {},

	"rules": [
		// Hide sidebar's vcs status icons
		{
			"class": "vcs_status_badge",
			"layer0.opacity": 0.0,
		},
		// Show panel's close button
		{
			"class": "panel_close_button",
			"content_margin": 8,
			"layer0.opacity": 1.0
		},
		// Highlight the top border of the focused tab instead of the left one
		{
			"class": "tab_control",
			"layer2.inner_margin": [0, 2, 0, 0],
		},
	]
}
```

## Credits

https://github.com/andresmichel/one-dark-theme was helpful for me to create this theme.