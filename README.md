CharMap
=======

## What is CharMap?

CharMap is unicode table viewer for Emacs.
With CharMap you can see the unicode table based on The Unicode Standard 6.2.

You can install CharMap via http://marmalade-repo.org/

## How to use?

CharMap is really simple to use.
Just execute a command 'M-x charmap' to display a unicode block that you want to see.

To see all unicode blocks, try to M-x charmap-all but the entire blocks are so huge to display
and it takes a little time.

![alt text](https://raw.github.com/lateau/charmap/gh-pages/images/charmap.png "")

## Customization

Here are customizable variables.

```cl
(defcustom charmap-rollback-cursor nil
  "Move cursor to other window after charmap-describe-char."
  :type 'symbol
  :group 'charmap)

(defcustom charmap-text-scale-adjust 4
  "Text scale."
  :type 'integer
  :group 'charmap)

(defcustom charmap-enable-simple nil
  "Display a result in minibuffer"
  :type 'symbol
  :group 'charmap)

(defface charmap-face '((t (:family "dejavu sans" :weight normal :slant normal :underline nil)))
  "Font lock face used to *charmap* buffer."
  :group 'charmap)
```

## TODO

* simple mode using minibuffer instead using describe-char
* search mode (by code)
* ecb integration
* major mode
* doesn't work well with (set-fontset-font nil 'japanese-jisx0208 ...)
* font selector
