recently.el
===========


Track recently opened files to visit them again


Usage
-----

`M-x recently-mode` to start recording file paths on visiting them,
and `M-x recently-show` to display buffer to visit them again.


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
  - `recently` saves and restores the list every time when adding
    files and reading the list, if necessary
- Do not remove entries that are not found in filesystems
  - Today it is common that a file is not found temporarily,
    for example when using some VCSes like Git
- Use `tabulated-list-mode` to show the list, instead of package
  specific mode


License
-------

This software is unlicensed. See `LICENSE` for details.
