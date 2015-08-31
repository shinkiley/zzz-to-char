# Zzz to Char

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)

This package provides two new commands: `zzz-to-char` and `zzz-up-to-char`
which work like built-ins `zap-to-char` and `zap-up-to-char`, but allow you
quickly select exact character you want to “zzz” to.

The commands are minimalistic and often work like built-in ones when there
is only one occurrence of target character (except they automatically work
in backward direction too). You can also specify how many characters to scan
from each side of point, see `zzz-to-char-reach`.

This package uses avy as backend.

## Installation

Download this package and place it somewhere, so Emacs can see it. Then put
`(require 'zzz-to-char)` into your configuration file. Done!

## Usage

Just bind `zzz-to-char` or `zzz-up-to-char` (depends on your taste, the
latter doesn't include target char into killed text):

```emacs-lisp
(global-set-key (kbd "M-z") #'zzz-to-char)
```

## License

Copyright © 2015 Mark Karpov

Distributed under GNU GPL, version 3.