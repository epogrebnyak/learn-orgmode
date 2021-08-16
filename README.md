## My Emacs workflow

### Minimal pipeline

  - Install emacs on WSL with `sudo apt-get install emacs`
  - Launch emacs with `emacs` command
  - Open a file with F10 menu
  - Edit file using org mode (various operations)
  - Save file **C-x C-s**
  - Exit Emacs **C-x C-c**

<div class="INSTALL drawer">

  - Running in cmder bash (ubuntu)
  - Windows Emacs MSI (bad russian font spacing)
  - VSCode extension (no agenda view)

</div>

### Improvements \[4/4\]

  - F10 may need Fnlock to work on Lenovo - use Fn-Esc.
  - Configure terminal to resolve [key binding
    conflicts](https://emacs.stackexchange.com/questions/68105/how-to-use-ctrl-c-on-wsl-key-binding-conflict)
    like Ctrl-C. See also `org-disputed-keys` in [Orgmode
    conflicts](https://orgmode.org/manual/Conflicts.html).
  - Launch emacs with filename `emacs -nw README.org`
  - Use Shift for selection and CUA mode with more familiar key
    bindings.
  - `pandoc README.org -f org -t gfm -o README.md` (see pandoc [formats
    list](https://pandoc.org/MANUAL.html#general-options))

## Next steps

### Nice to have \[0/2\]

  - \[ \] Move line across headers, beyond own section (Alt - arrow has
    limits within a header)
  - \[ \] What does bottom line with `-UUU(DOS)**--F1` mean? How to
    remove it?

### Not critical \[0/5\]

  - \[ \] Recalulcate list stats
  - \[ \] Add timestamp with current time, not just date
  - \[ \] Change selection color to lightblue (I did, but it did not
    save)
  - \[ \] View calendar
  - \[ \] [Reload on file
    change](https://emacs.stackexchange.com/questions/169/how-do-i-reload-a-file-in-a-buffer?newreg=a3feb7dd0515464f962f420449b8f1a5)
    (will allow editing in VS Code)

### CANCELLED Not todo

  - Use spacemacs on Windows
  - Fix wrong spacing of Russian fonts in Windows Emacs GUI

### DONE Finshed tasks \[7/7\]

  - \[X\] Sort this list based on completion is C-c ^
  - \[X\] Add more cycling todo tags `#+SEQ_TODO:`
  - \[X\] What is the difference between scheduled and deadline?
  - \[X\] Archive tasks with menu
  - \[X\] Create a link
  - \[X\] Make a selection, copy and paste selection
  - \[X\] \* Use sterisk to add difficulty level / priority for plain
    text

## Editing in orgmode

### \<TAB\> is all you need

  - TAB shows/hides headers (quite powerful\!)
  - Shift-TAB opens all headers

### Editing a hyperlink

Use `[[url][]]` syntax or C-c C-l TODO: hyperlinks inside documents.

### Getting around headers

  - Alt + left rightor changes header level
  - Alt + up or down moves lines around
  - Shift - arrow:
      - changes list numbering style
      - cycles TODO-DONE in header
      - selects in CUA mode

### Use timestamps

SCHEDULED: \<2021-08-15 Sun\>

As
[guide](https://orgmode.org/guide/Creating-Timestamps.html#Creating-Timestamps)
suggests:

  - C-c . for timestamp
  - S-arrow for change

### Checkboxes

  - You must type \[0/0\] or \[0%\] for checkbox
  - Only X counts for completion, not \`x\` or \`+\`
  - C-c C-c toggles and recalculates
  - Q: what can recalcultae on its own?
  - Check Rainer König video [OrgMode E01S05:
    Checklists](https://www.youtube.com/watch?v=gvgfmED8RD4&list=PLVtKhBrRV_ZkPnBtt_TD1Cs9PJlU0IIdE&index=5&t=444s)

Sample checkbox list \[2/3\], \[66%\]:

  - \[X\] Item 1
  - \[X\] Item 2
  - \[ \] Item 3

### Agenda

  - Use F10 and menu
  - C-a key binding must be configured

<!-- end list -->

1.  Question
    <span class="tag" data-tag-name="QUESTION"><span class="smallcaps">QUESTION</span></span>
    
      - How to close agenda buffer

## Emacs configuration

### Where is the config?

  - \~/.emacs is a file
  - \~/.emacs.d is a directory
  - Q: what is th difference?

### Setting org-support-shift-select and CUA options

  - Selecting with Shift is already built-in part of Emacs, but not
    org-mode
  - Start with 'M-x customize' to find options
  - Setting CUA is part of F10 menu

## Reference

### Concepts

  - "buffer" - a screen that represents a file or Emacs own
  - "frame" - ?
  - "window" - ?

### Notation

\- \* is always a header

  - properties box has :NAME: and :END:

## Videos

Essential:

  - [Carsten Dominik keynote
    (2008)](https://www.youtube.com/watch?v=oJTwQvgfgMM)
  - [Rainer König lesson
    series](https://www.youtube.com/playlist?list=PLVtKhBrRV_ZkPnBtt_TD1Cs9PJlU0IIdE)

Extension:

  - [Evil Mode: Or, How I Learned to Stop Worrying and Love
    Emacs](https://www.youtube.com/watch?v=JWD1Fpdd4Pc)

## Blogs and success stories

  - <https://sachachua.com/blog/2014/01/tips-learning-org-mode-emacs/>
  - <https://blog.aaronbieber.com/2016/09/24/an-agenda-for-life-with-org-mode.html>

## Quotes

> Everything should be made as simple as possible, but not any simpler
> —Albert Einstein
