---
file: ~/.emacs.d/lisp/my-modules/mmd-mode/README.md
author: Alisha Awen Sheppard
created: 2019-002-05
updated: 2020-006-27
tags: Emacs, apps-tools, SysAdmin, HA-ModEmacs, MWM-how-to, how-to, README 
---

mmd-mode
========

## About this Clone:

This package is based on a customized implementation of: [markdown](http://daringfireball.net/projects/markdown/syntax) that uses the extended [multimarkdown](http://fletcherpenney.net/multimarkdown/) features for syntax highlighting.

This **Major Mode** is derived from and extends: [markdown-mode](http://jblevins.org/projects/markdown-mode/) created by Jason Blevins.

## Current Status:

- **2020-06-27:** Changed name of variable: `markdown-footnote-face` to: `markdown-footnote-text-face`. to maintain upward compatability with `markdown-mode`.

## Usage:

> **Note:** _(Everything Instructed below has already been done for you if you installed Harmonic Alchemy Modular Emacs as instructed in the main README.md file. You do not have to do this manually here.  Instructions are only here below as an FYI for cherry picking users who need that specific info.)_

In order to use this derived mode you must first retrieve the original markdown mode from the site above.

To use this mode, first add it to your load path in .emacs:

    (add-to-list 'load-path "{code location}")

Once this is in your load path add a require statement to source it

    (require 'mmd-mode)

To automatically start the mode when visiting an mmd file add the following to your .emacs file:

    (add-to-list 'auto-mode-alist '("\\.md\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mdwn\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mdt\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mmd\\'" . mmd-mode))

