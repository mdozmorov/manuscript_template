# Template of a manuscript in Rmd

Track/commit only text files (R, md, Rmd, txt, csv)! Do not commit large binary files (docx, xlsx, pptx, etc.) into GitHub repository. Every time such a file change, it changes completely and gets committed as such. This will grow your GitHub repository very fast. If needed, clean the repository using https://rtyley.github.io/bfg-repo-cleaner/

- Keep the central idea in mind, and make a list of points to illustrate it. 
- Be critical and creative, ask any questions you may think of, develop strategies to answer them. 
- Make a structured strategy to answer your questions. Think bulletpoints.
- Name your bulletpoints like newspaper headers - they should tell the story without the need to read the writeup.
- Don't run your analyses on full datasets. Make sure your pipeline _works from start to finish_ on a small subset of the data, then scale up.
- Read more, get inspiration from how others present results, what they discuss, which figures they show.

## Files

- `manuscript.Rmd` - Rmd skeleton of a manuscript

- `references.bib` - BibTex references example

## Folders

- `figures` - folder to store figures. Work-in-progress figures should be stored in PNG format. Publication-quality figures should be stored in TIFF format, 300dpi. Name figures as `Figure_X_<brief description>.png`. Add figures to the manuscript. Add legends.

- `tables` - folder to store tables. Work-in-progress tables should be stored in CSV format. Publication-quality tables may be stored as XLSX or PDF files. Name tables as `Table_X_<brief description.csv`. Add table legends to the manuscript.

- `supplementary` - folder for supplementary files. Name them as `Supplementary_<Table or Figure or File>_<brief description>`. Add legends for supplementary files to the manuscript.

- `submission` - folder only for files formatted for submission. 

- `styles.ref` - style files defining how (for which journal) references should be rendered. More at https://www.zotero.org/styles

- `styles.doc` - DOCX template defining margins and font styles in the knitted Word document. How-to at http://rmarkdown.rstudio.com/articles_docx.html

	- `Arial_11_double_space_normal_margins.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, double-spaced, regular margins
    - `Arial_11_single_space_normal_margins.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, single-spaced, regular margins
    - `NIH_grant_style.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, narrow margins
    - `nar_word_template.doc` - generic template provided by NAR

