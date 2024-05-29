# swtdata

Landing page for Swisstransplant Data Science.

## Rendering the website with quarto

First, we need to render all profiles, it is important to first render the German version.

    quarto render --profile deutsch
    quarto render --profile francais
    quarto render --profile english
    
Then we apply the post-processing script `Multilanguage.qmd` which translates the document titles.