After installing the Quarto CLI, check the installation:

```bash
quarto check
```

Preview locally:

```bash
quarto preview
```

Switch to the Quarto environment you installed with Jupyter:

```bash
conda activate quarto
```

Create a folder for your post under the `posts` directory:

```bash
mkdir -p posts/hello-quarto
```

Create Quarto files:

```bash
touch posts/hello-quarto/index.qmd
touch posts/_index.qmd
```

Manually delete the generated `_site/` folder to clear the cache, then render and preview again:

```bash
rm -rf _site
quarto render
quarto preview
```

Create a new notebook under the `posts/` directory:

```bash
jupyter notebook posts/2025-09-09-hello-quarto.ipynb
```

Render the notebook into a post:

```bash
quarto render posts/2025-09-09-hello-quarto.ipynb
```
This will output the corresponding HTML file to `_site/` and automatically update the site.

