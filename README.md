## Features

* Multi-language support, multi-platform

* Handy splited window control (C-x o a\~z; M-1\~9)

* Friendly to new emacsers, customizable, productive

* Integrated with many useful developing tools (magit, slime, etc.)

* Magical appearence

## Supported Language

* Ruby / Clojure / Python / Haskell 

* Erlang / Lisp / Mozart Oz / Coq

* Js / Coffeescript / PHP / Html

* CSS / LESS / SASS / SCSS

* HAML / Markdown / Textile / ERB

## Emacs Cheat Sheet

On Construction.

<table>
  <tr>
    <td valign=top>
	 <table border>
	   <tr>
	     <th rowspan=2><font size=+1>Cursor<br>Motion</font></th>
	     <th colspan=4>Operation</th>
	   </tr>
	   <tr>
	     <th colspan=2>Move</th>
	     <th colspan=2>Delete</th>
	   </tr>
	   <tr>
	     <th>Amount</th>
	     <th>forward</th>
	     <th>backward</th>
	     <th>forward</th>
	     <th>backward</th>
	   </tr>
	   <tr>
	     <td>Characters</td>
	     <td><tt>C-f</tt></td>
	     <td><tt>C-b</tt></td>
	     <td><tt>C-d</tt></td>
	     <td><tt>DEL</tt></td>
	   </tr>
	   <tr>
	     <td>Words</td>
	     <td><tt>M-f</tt></td>
	     <td><tt>M-b</tt></td>
	     <td><tt>M-d</tt></td>
	     <td><tt>M-DEL</tt></td>
	   </tr>
	   <tr>
	     <td>Lines</td>
	     <td><tt>C-n</tt></td>
	     <td><tt>C-p</tt></td>
	     <td><tt>C-k</tt> <i>(to EOL)</i></td>
	     <td><tt>C-SPC C-a C-w</tt></td>
	   </tr>
	   <tr>
	     <td>Sentences</td>
	     <td><tt>M-e</tt></td>
	     <td><tt>M-a</tt></td>
	     <td><tt>M-k</tt></td>
	     <td><tt>C-x&nbsp;DEL</tt></td>
	   </tr>
	   <tr>
	     <td>Expressions</td>
	     <td><tt>C-M-f</tt></td>
	     <td><tt>C-M-b</tt></td>
	     <td><tt>C-M-k</tt></td>
	     <td><tt>C-M-DEL</tt></td>
	   </tr>
	   <tr>
	     <td>Paragraphs</td>
	     <td><tt>M-}</tt></td>
	     <td><tt>M-{</tt></td>
	     <td colspan=2><i>(no standard bindings for delete
		  cmds)</i></td>
	   </tr>
	   <tr>
	     <td>End/start of line</td>
	     <td><tt>C-e</tt></td>
	     <td><tt>C-a</tt></td>
	     <td colspan=2><i>(repeat count goes to following
		  lines)</i></td>
	   </tr>
	   <tr>
	     <td>End/start of buffer</td>
	     <td><tt>M-&gt;</tt></td>
	     <td><tt>M-&lt;</tt></td>
	     <td colspan=2><i>(no repeat count)</i></td>
	   </tr>
	 </table>
    </td>

    <table>
  <tr>
    <th colspan="3">Scroll Motion</th>
    <th colspan="2" rowspan="2">Other Scroll Method</th>
  </tr>
  <tr>
    <td>Amount</td>
    <td>Up</td>
    <td>Down</td>
  </tr>
  <tr>
    <td>Paragraph</td>
    <td>M-{</td>
    <td>M-}</td>
    <td>Go to line</td>
    <td>M-g g</td>
  </tr>
  <tr>
    <td>Screen</td>
    <td>M-v</td>
    <td>C-v</td>
    <td>Scroll other window down</td>
    <td>C-M-v</td>
  </tr>
  <tr>
    <td>Buffer</td>
    <td>M-&lt;</td>
    <td>M-&gt;</td>
    <td></td>
    <td></td>
  </tr>
</table>
    <table id="">
    </table>
    <table id="">

</table>

## Prerequisites

1. When programming with Haskell, you need to install Haskell syntax checking tool Stack (and GHC 8.0.2 +). Run:

```shell

# Install Stack

wget -qO- https://get.haskellstack.org/ | sh

# Install Haskell

stack setup --install-ghc

```
This GHC will not replace former versions.

Warning : Lacking of Stack will cause Emacs fail to respond for seconds when editing .hs files.

2. Proof-general for Coq (or others).


Proof-general is already exists in "~/.emacs.d/site-lisp/". You should indicate the Coq path on Windows.

3. Mozart-Oz. You can find Mozart-Oz on its <a href="https://mozart.github.io/mozart-v1/doc-1.4.0/install/index.html">Official Website</a>.

If you are installing an rpm package (only i386 version is avaliable), you need to convert it to amd64 version.

After installation, you can weak up Mozart Oz by:

```elisp
M-x run-oz
```

Or change current mode to oz-mode by:

```elisp
M-x oz-mode
```

## Plug-in List

## Attention

global-git-commit-mode may slows the reative of some operations in some low performance hard disks. You can block up this package in init-git.el.

In init-windows.el, windmove-defualt-keybindings is set to 'control and it is conflicted with paredit. Now you can edit parenthesis with C-<right>, C-<left>, etc.
    



  
