# COVID Vaccine Timelines

This is a repository for writing a paper to accomany [this analysis of COVID vaccine timelines](https://github.com/davidoj/covid-vaccine-timeline).

This repository uses the [bookdown](https://bookdown.org/yihui/rmarkdown/books.html) package for cross-referencing and [rticles](https://bookdown.org/yihui/rmarkdown/journals.html) for the arxiv template. To install:

	devtools::install_github('rstudio/bookdown')
	devtools::install_github("rstudio/rticles")

References are generated using Zotero with the [Better BibTex](https://retorque.re/zotero-better-bibtex/) extension.

To build the report, navigate to the `report` folder and run

	bookdown::render_book("index.Rmd", "bookdown::pdf_book")

The directories are:

`bookdown-example`: contains a minimal bookdown book example which might be a helpful reference for some purposes. It is for reference purposes only

`report`: contains the Rmd files comprising the report
 - `index.Rmd`: header file for the report, including the abstract
 - `01_introduction`: introduction
 - `02_methods.Rmd`: methods section (simulation and counterfactual generation)
 - `03_results.Rmd`: results section
 - `04_discussion_conclusion`: discussion and conclusion
 - `05_appendix.Rmd`: appendix section (sensitivity analysis, comparison to Watson et. al.)
 - `_bookdown.yml`: [optional build settings](https://bookdown.org/yihui/rmarkdown/bookdown-project.html#bookdown.yml)
 - `_output.yml`: [specify book output formats and format-specific settings](https://bookdown.org/yihui/rmarkdown/bookdown-project.html#bookdown.yml)
 - `report.bib`: BibTex references

