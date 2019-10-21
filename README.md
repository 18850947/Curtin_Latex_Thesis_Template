# Curtin Latex Thesis Template
###### A repository to keep up to date with changes made to the latex template that is flying around for curtin undergrads.

This repo contains only the "thesis_main.tex" file, as this file contains all the formatting neccesary. The chapters can be edited to suit your requirements and will reflect in the ToC. 

 ## Tips for Use
 ### basic use
 #### First time
 1. create an folder called Thesis_Latex (or whatever you want to name it)
 within this folder make a folder called figures, and another called chapters, ie
 > Thesis_latex
 >  - figures
 >  - chapters
 
 2. create a blank .tex file and save it in the folder.
 
 3. copy/paste the code from the desired version on the repo into the empty .tex file.
 
 4. now you should have the option to automatically create the relevant chapter .tex files, which will appear in the thesis_latex/chapters directory
 
 5. save your figures to the figures folder as you go. 
 
#### Updating versions
If you already have the file implemented you can update it to the desired version by simply changing the preamble to that of the desired version.

**Updates that require other code changes will be made clear in the readMe** so make sure to check before updating.

## references
It is recomended to use bibTex to handle references. The template is setup to use IEEE referencing style, however this is not the style that The university requests. make sure to get 
permission from your supervisor to use IEEE if you want to use it. Changing Referencing styles is untested.

To use bibTex do the following:
1. Create a .bib file and fill this with bibTex formatted references.
2. Change line 120 to \bibliography{name_of_the_bib_file}
3. press F8 to compile the bibliography file
4. press F5 to compile the main document

If you were previously using Endnote, it can be exported to a bibTex .bib file by following [this link](https://www.rhizobia.co.nz/latex/convert)
which can be used directly in the in above steps in place of (1.)

To then reference in text, use the 
```
\cite{bibTexID}
```
command, where bibTexID is the first entry in the bibTex Entry

if you transfered from endnote these are formatted as 
>RN#

Where # is a number. You can uncompile word document Endnote references from the endnote tab of word, and then the # is the number that appears after the Author and date in the { } brackets.

This holds true over multiple word documents that use the same endnote library.

### figures
A shortcut command for inputing figures has also been implemented. this doesn't overwrite the inbuilt figures environment/

to use: 

```
\fig{filename}{label}{title}
```

as opposed to starting an environment, captioning, ect. The only thing with this method is the label doesn't appear when you use \ref, as it is not put in until compile time.


## Issues
Feel free to message someone or open a ticket if you encounter any issues or notice any changes that need to be made

## Updates
If you fix any issues feel free to push to a branch under your student id/name

## TODO:
  - [ ] ToC Formatting
  - [ ] Fix line hyphenation (properly)
  - [ ] Regulate line spacing to just text
        - ie: remove the massive line spacing in LoF and ToC
  - [ ] format bibliography
  - [ ] input letter template
  
## Use
- Available for free use by anyone without any acknowledgement required
- It is the responsibility of the user to ensure this template suits any and all requirements set out by their institue
- This Template is designed only as a guide that is formatted to the Curtin university standards to the best of the authors' ability.
  
