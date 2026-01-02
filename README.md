# UGRacing Electrical Documentation

Welcome to UGR Electrical's documentation repo. The goal here is that anyone can contribute if they feel the documentation needs changed, and provides a central location to access everything. LaTeX will be used throughout your degree if you haven't started already and is a good skill to have, and so is what is used to write the majority of the documentation in this repo.

## Table of contents
---
### Software

Altium: 

 - [Getting Started (PDF)](https://raw.githubusercontent.com/UGRacing-Electronics/UGR_Electrical_Documentation/main/Software/Altium/Getting%20Started/Getting%20Started.pdf)


## How this repo works

This repo is set up to use GitHub Actions to compile the LaTeX PDF. When running the compile process the action will check for changes made to files called "main.tex". Therefore, whatever file structure you use, please call your main .Tex file `main.tex`. Otherwise the action will not recognise that there is a tex file to compile. Please also make sure that the folder containing your "main.tex" is titled appropriately, as it will use this folder name to determine what to call your PDF.

**TL;DR: Name your tex file main.tex, and after a commit a PDF will be generated in that folder under the name of the parent folder.**

e.g.     /Software/Altium/Getting Started/**main.tex** => /Software/Altium/Getting Started/**Getting Started.pdf**

**Do not edit the action workflow unless you know what you're doing**

## Creating a new document

If creating a LaTeX document from scratch, there will be no prior folder set up for use. It is therefore important that you follow the existing file structure and name your folders appropriately. For details on how to name your files and final folder, please read the "How this repo works" section above. It is very important come compile time. Otherwise, just be reasonable with your folder names, and please please please capitalise correctly.

## Making Changes

---

If you have editing abilities for this repository/this organisation, you have been trusted to not mess with or break anything. **Please do not abuse this trust.** If you are unsure if your addition is useful or functional, check with your team head before pushing a commit.

The university offers all students free access to [overleaf.com](http://overleaf.com/). I advise using this to make changes to LaTeX files as its quite a process installing it locally.

Use Overleaf's import from github function to add it to your overleaf account. Please periodically pull on Overleaf to make sure it remains up to date. When you load into overleaf there are some configuration changes you'll need to make.

Use the settings icon in the bottom left and modify these two settings found under ‘compiler’:

- Main document
- Compiler

The “Main Document” should be set to whichever .tex file you are editing, and the Compiler should be (for compatibility reasons) set to **LuaLaTeX**. It’s possible that some packages you use may only allow you to use specific compilers. So **change this as necessary**.

Once you’ve made your changes and you’ve checked with your team head, you are free to commit to the repo. The way this repo is set up to work, upon pushing a change to a main.tex file, the github servers will automatically recompile the PDF. 

Please note: **Overleaf has no branching functions, you will be pushing directly to main.**

If you create any additional guides/PDFs, please add them to the table of contents at the start of this readme. Please do this by appending “?raw=true” to the end of the github link for the PDF. e.g.

```
https://github.com/UGRacing-Electronics/UGR_Electrical_Documentation/blob/main/Software/Altium/Getting Started/Getting%20Started.pdf

becomes

https://github.com/UGRacing-Electronics/UGR_Electrical_Documentation/blob/main/Software/Altium/Getting Started/Getting%20Started.pdf?raw=true
```

## Force recompile all main.tex files

Though unlikely, there may be a situation where you need to force recompile every main.tex in the repo. To do this, go to the repo's actions page, select "Compile LaTeX Files" on the left hand side, and click "Run Workflow" in the main table. Now refresh and you should see a new workflow run with the text "Manually triggered by _______". 
