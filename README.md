# swtdata

Landing page for Swisstransplant Data Science.

## Rendering the website with quarto

### 1. Rendering

First, we need to render all profiles, it is important to first render the German version.

    quarto render --profile de
    quarto render --profile fr
    quarto render --profile en
    
The preview option can also be used to render and also display the page. Don't preview the website in case you have drafts because preview will render them.

    quarto preview --profile de

### 2. Multilanguage support

We run the post-processing script which translates the document titles.
    
    Multilanguage.qmd
    
### 3. Upload the project to GitHub

Let's review all changes.

    git status
    
If all if fine, commit all changes and push a new version of the website.

    git add --all
    git commit -m "update Q1 2024"
    git push
    
    