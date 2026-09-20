# ADT

Coursework notebooks kept for reference. This repository is classwork, not a portfolio project: nothing here is a finished analysis with a business question, tests or a reproducible pipeline. The analyst projects are in the [profile README](https://github.com/VijayChamakuri).

## What is here

| Notebook | What it does |
|---|---|
| [`Vichama_Homework2 MongoDB.ipynb`](Vichama_Homework2%20MongoDB.ipynb) | Data-cleaning homework: loads a `Sales.csv` extract with pandas, strips thousands separators from `Unit Price` and `Unit Cost`, casts both to float, and writes `cleaned_sales_data.csv`. |
| [`docs/m11-highdim/lab11.ipynb`](docs/m11-highdim/lab11.ipynb) | Lab on visualizing high-dimensional data: scatterplot matrix, parallel coordinates, and PCA, including PCA on face images, with pandas, seaborn, Altair and scikit-learn. |
| [`docs/m12-maps/lab12.ipynb`](docs/m12-maps/lab12.ipynb) | Lab on maps: an Altair dotmap of US zip codes, a choropleth, a datashader raster and an ipyleaflet interactive map. |

The two lab notebooks under `docs/` follow the open [dviz-course](https://github.com/yy/dviz-course) materials; the surrounding text and exercises are the course's, and the worked solutions are mine.

## Data

The homework notebook reads a local `Sales.csv` from an absolute path on the machine where it was run, and that file is not committed, so the notebook will not rerun as written without supplying your own extract and editing the path. The lab notebooks pull their datasets from `vega_datasets` and the course's own sources at run time.

## Run it

```bash
pip install jupyter pandas numpy matplotlib seaborn altair scikit-learn vega_datasets datashader holoviews colorcet ipyleaflet
jupyter lab
```

## Limitations

Stored outputs are from the original runs and are not regenerated or tested by any CI. The homework notebook is a small cleaning exercise, not a data-quality framework. The name `ADT` is the course shorthand used when the repository was created and is left as is so existing links keep working.
