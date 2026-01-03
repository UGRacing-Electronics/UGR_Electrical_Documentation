# UGR Electrical Documentation Templates

This folder contains the templates you'll need to create useful documentation.

## Main Essentials

In order to make the UGR template what it is, the following files and folders are essential to the template and must be present in the same folder structure. To make it easier, if you copy the folder "TemplateProject", you should be off to the races. But what each file does is outlined below:

- `fonts/`: Contains the fonts we use in UGR as per the design guide in the teams
- `template/`: Contains the images required to make the UGR template work.
- `preamble.tex`: The .tex file responsible for loading all packages in. This could have been put at the top of the main.tex but is 100 lines so was made separate for readability.
- `main.tex`: This is your main tex file that you will use to write your documentation.

## Additional Tex Files

There are some helper tex files that have been made (if you make a helper .tex, please add it here for others to use) to make things easier/show information in a nice way.

Any additional .tex files you use must be placed in your project directory alongside your "main.tex" and "preamble.tex" and used as below:

```\input{FILENAME}``` where FILENAME is the name of the helper .tex file without the ".tex" suffix. Place this at the top of your main.tex under `\input{preamble}`.

e.g. for the emphasis boxes detailed below, use `\input{emphasis_boxes}`. 

### emphasis_boxes.tex

This is a helper tex that gives nice formatting to "Notes", "Important" boxes that you might want to use as part of your documentation. 

```latex
\begin{important}
    IMPORTANT INFO % Standard LaTeX can be used here
\end{important}

\begin{note}
    NOTEWORTHY INFO % Standard LaTeX can be used here
\end{note}
```
![result](image.png)