# UGRacing Electrical Documentation

Welcome to UGR Electrical's documentation repo. The goal here is that anyone can contribute if they feel the documentation needs changed, and provides a central location to access everything. LaTeX will be used throughout your degree if you haven't started already and is a good skill to have, and so is what is used to write the majority of the documentation in this repo.

## Table of contents

---

### Software

Altium: 

- [Getting Started](https://github.com/UGRacing-Electronics/UGR_Electrical_Documentation/blob/main/Software/Altium/Getting%20Started/getting_started.pdf?raw=true)

## Making Changes

---

If you have editing abilities for this repository/this organisation, you have been trusted to not mess with or break anything. **Please do not abuse this trust.** If you are unsure if your addition is useful or functional, check with your team head before pushing a commit.

The university offers all students free access to [overleaf.com](http://overleaf.com/). I advise using this to make changes to LaTeX files as its quite a process installing it locally.

Use Overleaf's import from github function to add it to your overleaf account. Please periodically pull on Overleaf to make sure it remains up to date. When you load into overleaf there are some configuration changes you'll need to make.

Use the settings icon in the bottom left and modify these two settings found under ‘compiler’:

- Main document
- Compiler

The “Main Document” should be set to whichever .tex file you are editing, and the Compiler should be (for compatibility reasons) set to **LuaLaTeX**. It’s possible that some packages you use may only allow you to use specific compilers. So **change this as necessary**.

Once you’ve made your changes and you’ve checked with your team head, you are free to commit to the repo. 

Please note: **Overleaf has no branching functions, you will be pushing directly to main.**

If you create any additional guides/PDFs, please add them to the table of contents at the start of this readme. Please do this by appending “?raw=true” to the end of the github link for the PDF. e.g.

```
https://github.com/UGRacing-Electronics/UGR_Electrical_Documentation/blob/main/Software/Altium/Getting Started/getting_started.pdf

becomes

https://github.com/UGRacing-Electronics/UGR_Electrical_Documentation/blob/main/Software/Altium/Getting Started/getting_started.pdf?raw=true
```
