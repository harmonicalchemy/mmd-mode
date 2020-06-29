---
file: ~/.emacs.d/lisp/my-modules/mmd-mode/README.md
author: Alisha Awen Sheppard
created: 2019-002-05
updated: 2020-006-28
tags: Emacs, apps-tools, SysAdmin, HA-ModEmacs, MWM-how-to, how-to, README 
---

mmd-mode
========

## About this Clone:

This **`mmd-mode`** package is based on a customized implementation of: [markdown](http://daringfireball.net/projects/markdown/syntax) that uses the extended [multimarkdown](http://fletcherpenney.net/multimarkdown/) features for syntax highlighting.

**`mmd-mode`** is an Emacs major-mode derived from and extending: [markdown-mode](http://jblevins.org/projects/markdown-mode/) created by Jason Blevins which is available on MELPA... 

The original **`jmquigley/mmd-mode`** is no longer available on MELPA and its Github repository has not been updated in 3 years... 

I cloned the original repository here and am now maintaining it to be used with **Harmonic Alchemy Modular Emacs**, and also to keep it up to date with new changes/updates within upstream **`markdown-mode`** which just became necessary this year... (not sure if JmQuigley will be updating his)...

## Current Status:

- **2020-06-27:** Changed name of variable: `markdown-footnote-face` to: `markdown-footnote-text-face`. to maintain upward compatability with `markdown-mode`.

## Usage:

> **Note:** _(If you are using this with **Harmonic Alchemy Modular Emacs** everything instructed below has already been done for you. You do not have to do this manually here.  Instructions are only here below as an FYI for other users who do not use **HA Modular Emacs** and only wish to use this updated version of **`mmd-mode`** within their own custom Emacs configurations.)_

- In order to use this derived mode you must first install **`markdown-mode`** from MELPA, or clone: [Jason Blevin's Github markdown-mode repository](https://jblevins.org/projects/markdown-mode/) and install it manually... _(follow instructions from above link)_

- To use this mode, first add it to your load path in .emacs:

```lisp
    (add-to-list 'load-path "{code location}")
```

- Once this is in your load path add a require statement to source it

```lisp
    (require 'mmd-mode)
```

- To automatically start the mode when visiting an mmd file add the 
following to your .emacs file:

```lisp
    (add-to-list 'auto-mode-alist '("\\.md\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mdwn\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mdt\\'" . mmd-mode))
    (add-to-list 'auto-mode-alist '("\\.mmd\\'" . mmd-mode))
```

