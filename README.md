recently.el
===========


Track recently opened files to visit them again later


Usage
-----

`M-x recently-mode` to start recording file paths on visiting them,
and `M-x recently-show` to display buffer to visit them again.


Why not recentf?
----------------

Besides built-in `recentf` is a great package, I want several features
that this package does not provide:

- Record directories visited by dired
  - `recentf-ext` also provides this, but this adds too many entries
  - `recently` adds only the "deepest" paths when go into
    subdirectories
- Share recent list amongh multiple Emacs instances
  - `sync-recentf` also provides this
- Do not remove entries that are not found in filesystems
- Use `tabulated-list-mode` to show the list, instead of package
  specific mode


License
-------

This software is unlicensed. See `LICENSE` for details.
