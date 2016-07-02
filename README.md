[![MELPA](http://melpa.org/packages/charmap-badge.svg)](http://melpa.org/#/charmap)

## What is CharMap?

CharMap is unicode table viewer for Emacs.
With CharMap you can see the unicode table based on The Unicode Standard 6.2.

Newest CharMap is available on MELPA.

## How to use?

CharMap is really simple to use.
Just execute a command 'M-x charmap' to display a unicode block that you want to see.

To see all unicode blocks, try to M-x charmap-all but the entire blocks are so huge to display
and it takes a little time.

![alt text](https://raw.github.com/lateau/charmap/gh-pages/images/charmap.png "")

### Keybindings

* C-f: forward
* C-b: backward
* C-n: next line
* C-p: previous line
* RET: copy a character that current cursor's on
* z: zoom(tooltip)
* s: search(NYI)

## Customization

Here are customizable variables.

```cl
(defcustom charmap-text-scale-adjust 4
  "Text scale."
  :type 'integer
  :group 'charmap)

(defface charmap-face '((t (:family "dejavu sans" :weight normal :slant normal :underline nil)))
  "Font lock face used to *charmap* buffer."
  :group 'charmap)
```
