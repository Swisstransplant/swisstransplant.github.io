# Swisstransplant Data Science Website

Landing page for Swisstransplant Data Science.

## Rendering the website with Quarto

> [!TIP]
> Before rendering, it may be a good idea to temporarily pause OneDrive synchronization. The reason is that during rendering, a lot of temporary files are being created and deleted, which can cause problems. 

### 1. Rendering

First, we need to render all profiles. It is important to first render the German version.

```
quarto render --profile de
quarto render --profile fr
```
    
The preview option can also be used to render and display the page. Don't preview the website in case you have drafts because preview will render them.

```
quarto preview --profile de
```

### 2. Multilanguage support

We run the post-processing script, which translates the document titles.

```
Multilanguage.qmd
```
    
### 3. Upload the project to GitHub

Let's review all changes.

```
git status
``` 

If all is fine, commit all changes and push a new version of the website.

```
git add --all
git commit -m "update Q1 2024"
git push
```
