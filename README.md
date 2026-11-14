<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for <a href="https://gitlab.com">GitLab</a>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
	<a href="https://github.com/jerr3n/gitlab/stargazers"><img src="https://img.shields.io/github/stars/jerr3n/gitlab?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
	<a href="https://github.com/jerr3n/gitlab/issues"><img src="https://img.shields.io/github/issues/jerr3n/gitlab?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
	<a href="https://github.com/jerr3n/gitlab/contributors"><img src="https://img.shields.io/github/contributors/jerr3n/gitlab?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
	<a href="https://github.com/jerr3n/gitlab/raw/main/catppuccin.user.css"><img src="https://img.shields.io/badge/stylus-install-cba6f7?colorA=363a4f&style=for-the-badge"></a>
</p>

<!-- TODO: add a catwalk preview (assets/preview.webp) and per-flavor screenshots. -->

## Usage

1. Install [Stylus](https://github.com/openstyles/stylus) for
   [Firefox](https://addons.mozilla.org/en-GB/firefox/addon/styl-us/) or
   [Chrome](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne).
2. Open [`catppuccin.user.css`](https://github.com/jerr3n/gitlab/raw/main/catppuccin.user.css)
   and click **Install style**.
3. Pick your light flavor, dark flavor and accent in the style's settings.

The light/dark flavor follows GitLab's own **Color theme** preference
(_Preferences_ → _Appearance_), including _Auto_.

## 🙋 FAQ

- Q: **_"Does it work on self-hosted GitLab?"_**\
  A: Out of the box it applies to any instance whose hostname starts with
  `gitlab.` (`gitlab.com`, `gitlab.gnome.org`, `gitlab.freedesktop.org`, ...).
  For other hostnames, edit the `@-moz-document` line in Stylus' editor (an
  update of the style will overwrite this edit).

- Q: **_"Which syntax highlighting theme should I use?"_**\
  A: GitLab's default (**Light** / **Dark**). Code and diffs are recolored
  either way, but the other built-in themes may keep some of their own colors.

## Development

`catppuccin.user.css` is generated from [`gitlab.tera`](./gitlab.tera) with
[whiskers](https://github.com/catppuccin/whiskers). Do not edit it by hand:

```sh
whiskers gitlab.tera
```

The style remaps GitLab's design tokens (the `--gl-color-*` scales and a few
semantic tokens) instead of styling individual elements, so most of the UI,
including new components, picks up the palette automatically.

## 💝 Thanks to

- [jerren](https://github.com/jerr3n)

&nbsp;

<p align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" />
</p>

<p align="center">
	Copyright &copy; 2021-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
</p>

<p align="center">
	<a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a>
</p>
