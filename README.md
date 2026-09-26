# Primary GBM spatial atlas data

This repository serves data to the [single gGBO Spatial Atlas viewer](https://ysun-8.github.io/ggbo-spatial-atlas/). It does not contain a separate viewer.

The four FFPE Visium HD samples are 26455A4, 41602A8, 26941A3, and 26547A15, with 343,558 retained cells in total. Public files contain histology, cell annotations and coordinates, UMAP coordinates, QC metrics, and the complete exported SCT/data gene expression. Histology uses lossless WebP. Metadata and sparse gene chunks use gzip.

Source objects remain unchanged. Each retained center was checked against its source segmentation bounds; 26455A4 requires the source coordinate axes to be swapped. Viewer source, export scripts, and validation reports are maintained in ysun-8/ggbo-spatial-atlas.

GitHub Pages serves only the public directory. Its root redirects visitors to the main atlas. Keep relative filenames stable and deploy replacement metadata and expression chunks together. Both data and viewer deployments have separate 1 GB size checks.

## License

MIT. See [LICENSE](LICENSE).
