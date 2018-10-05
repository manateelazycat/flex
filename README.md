<img src="./screenshot.png">

### What's this?
It's a mode for flex files that provide better syntax highlight than flex-mode.el

## Installation
Then put flex.el to your load-path.

The load-path is usually ~/elisp/.

It's set in your ~/.emacs like this:

```Elisp
(add-to-list 'load-path "<path-to-flex") ; add flex to your load-path
(require 'flex)

(dolist (elt-cons '(
                    ("\\.l$" . flex-mode)
                    ))
  (add-to-alist 'auto-mode-alist elt-cons))

(autoload 'flex-mode "flex")
```
