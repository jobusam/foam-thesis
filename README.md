# foam-thesis
This Latex project contains my master thesis. 

The main goal is to build up a forensic analysis platform based on Apache Hadoop ecosystem. 
See compiled document [thesis.pdf](main.pdf).

## Build the document

### Install software

Installation on Fedora 27. Following packages must be installed:
```
sudo dnf install texmaker texlive-collection-langgerman texlive-csvsimple texlive-titlesec texlive-biblatex biber texlive-glossaries texlive-glossaries-german texlive-makeindex
```

### Run with Texmaker
You can buil the document from latex source code with Texmaker. Open Texmaker and create a cusom command (see User-> User Commands -> Edit User Commands). Following user command "Build with Biblatex" must be created:

```
pdflatex %.tex | makeglossaries % | biber % | pdflatex %.tex | evince %.pdf
```
Execute this command on [main.tex](main.tex).
Afterwards a Quick Build with Texmake is also sufficient unless you change the list of references.
