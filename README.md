# Swisstransplant Data Website

Landing page for Swisstransplant Data.

## 1. Render the Website in both Languages

> [!TIP]
> Before rendering, it may be a good idea to temporarily pause OneDrive synchronization. The reason is that during rendering, a lot of temporary files are being created and deleted, which can cause problems. 

> [!WARNING]
> It is important to first render the German version.

```
quarto render --profile de
quarto render --profile fr
```

> [!TIP]
> The preview option can also be used to render and display the page.

```
quarto preview --profile de
```

## 2. Multilanguage support

We run the post-processing script, which translates the document titles for French.

```
Multilanguage.qmd
```
    
### 3. Publish the website

First, let's review all changes.

```
git status
```

> [!CAUTION]
> Always check git status to ensure no unintended or sensitive files are being committed.

If all is fine, commit all changes and push a new version of the website.

```
git add --all
git commit -m "update Q1 2024"
git push
```
