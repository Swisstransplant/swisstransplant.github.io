# swtdata

Landing page for Swisstransplant Data Science.

## Rendering the website with quarto

### 1. Rendering

First, we need to render all profiles, it is important to first render the German version.

    quarto render --profile de
    quarto render --profile fr
    quarto render --profile en
    
The preview option can also be used to render and also display the page

    quarto preview --profile de

### 2. Multilanguage support

# Then we run the post-processing script which translates the document titles.
    
    Multilanguage.qmd
    
### 3. Upload the project to GitHub

Review, commit and push changes to GitHub

    git status
    git 