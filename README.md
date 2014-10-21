mmd-mode
========

A customized [markdown](http://daringfireball.net/projects/markdown/syntax) mode that uses [multimarkdown](http://fletcherpenney.net/multimarkdown/) syntax highlighting.

This is a major mode that is derived from the emacs [markdown-mode](http://jblevins.org/projects/markdown-mode/) created by Jason Blevins.

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
    
