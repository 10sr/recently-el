[![MELPA](https://melpa.org/packages/recently-badge.svg)](https://melpa.org/#/recently)
[![MELPA Stable](https://stable.melpa.org/packages/recently-badge.svg)](https://stable.melpa.org/#/recently)


recently.el
===========


Track recently opened files to visit them again


Usage
-----

**`M-x recently-mode`** Start saving file paths on visiting them

**`M-x recently-show`** Display buffer that shows list of recently visited files


Why not recentf?
----------------

Of course built-in `recentf` is a great package, but it lacks some
features that I would appreciate if it had:

- Record directories visited with dired
  - `recentf-ext` also provides this, but this sometimes adds too many
    entries
  - `recently` records only the "deepest" paths when going into
    subdirectories
- Share the file list among multiple Emacs instances
  - `sync-recentf` also provides this, but the sync can only be
    triggered with timer
  - `recently` saves and restores the list every time, if necessary,
    when adding files and reading the list
- Do not remove entries that are not found in filesystems
  - Today it is common that a file is not found temporarily,
    for example when using some VCSes like Git
- Use `tabulated-list-mode` to show the list, instead of a special
  mode for this


License
-------

This software is licensed under GPL Version 3 (or any later version).
See `LICENSE` for details.
