# Template of a manuscript in Rmd

Track/commit only text files (R, md, Rmd, txt, csv)! Do not commit large binary files (docx, xlsx, pptx, etc.) into GitHub repository. Every time such a file change, it changes completely and gets committed as such. This will grow your GitHub repository very fast. If needed, clean the repository using https://rtyley.github.io/bfg-repo-cleaner/

## Files

- `manuscript.Rmd` - Rmd skeleton of a manuscript

## Folders

- `figures` - folder to store figures. Work-in-progress figures should be stored in PNG format. Publication-quality figures should be stored in TIFF format, 300dpi. Name figures as `Figure_X_<brief description>.png`. Add figures to the manuscript. Add legends to `figure_legends.md`.

- `tables` - folder to store tables. Work-in-progress tables should be stored in CSV format. Publication-quality tables may be stored as XLSX or PDF files. Name tables as `Table_X_<brief description.csv`. Add table legends to `table_legend.md`.

- `supplementary` - folder for supplementary files. Name them as `Supplementary_<Table or Figure or File>_<brief description>`. Add legends for supplementary files to `supplementary_legend.md`.

- `references` - BibTex `references_MD.bib` file with references. For Mac, use [BibDesk](https://bibdesk.sourceforge.io/) together with [bibdesk-pandoc-export-templates](https://github.com/dsanson/bibdesk-pandoc-export-templates) to work with references in BibTex format.

- `submission` - folder only for files formatted for submission. 

- `styles.ref` - style files defining how (for which journal) references should be rendered. More at https://www.zotero.org/styles

- `styles.doc` - DOCX template defining margins and font styles in the knitted Word document. How-to at http://rmarkdown.rstudio.com/articles_docx.html

    - `Arial_11_double_space_normal_margins.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, double-spaced, regular margins
    - `Arial_11_single_space_normal_margins.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, single-spaced, regular margins
    - `Helvetica_11_single_space_normal_margins.docx` - Helvetica font, 11 pt
    - `NIH_grant_style.docx` - Arial font, 11 pt, all headers are also Arial, all fonts are black, narrow margins
    - `nar_word_template.doc` - generic template provided by NAR
    - `Times_12_single_space_normal_margins.docx` - standard formatting

## Writing tips

- Keep the central idea in mind, and make a list of points to illustrate it. 
- Be critical and creative, ask any questions you may think of, develop strategies to answer them. 
- Make a structured strategy to answer your questions. Think bulletpoints.
- Name your bulletpoints like newspaper headers - they should tell the story without the need to read the writeup.
- Address the following questions under each header:
    - What is the question?
    - What data/methods are used?
    - Any relevant details/results?
    - What is the answer (take home message)?
- Don't run your analyses on full datasets. Make sure your pipeline _works from start to finish_ on a small subset of the data, then scale up.
- Read more, get inspiration from how others present results, what they discuss, which figures they show.
- As you add files, describe them in the `README.md`. Add brief description of each file.

- Savage, Van, and Pamela Yeh. “Tips from a Pulitzer Prizewinner,” - Tips for writing scientific papers: minimalism = clarity, make 2-3-points home message, one paragraph = one message, use short sentences, use fast-paced narrative, avoid over-elaboration, use commas and dashes appropriately, more.

- [The Modern Language Association (MLA) citation and format style](https://owl.purdue.edu/owl/research_and_citation/mla_style/mla_style_introduction.html) and other [General Writing Resources](https://owl.purdue.edu/owl/general_writing/index.html) from Purdue University

## Figure tips

- Rules for better figures: 1) Know your audience; 2) Identify your message; 3) Adapt the figure to the support medium; 4) Captions are not optional; 5) Do not trust the defaults; 6) Use color effectively; 7) Do not mislead the reader; 8) Avoid chartjunk; 9) Message trumps beauty; 10) Get the right tool (Matplotlib, Inkskape, GIMP, others). Examples of good and bad figures.
    - Rougier, Nicolas P., Michael Droettboom, and Philip E. Bourne. “Ten Simple Rules for Better Figures.” PLoS Computational Biology 10, no. 9 (September 11, 2014): e1003833. https://doi.org/10.1371/journal.pcbi.1003833.

## Reviewing tips

- Guidelines and ideas for providing objective reviews, addressing quality and impact (Box 1). Recommendations on review behavior to avoid (Box 2). https://immunox.ucsf.edu/future-immunology
    - Krummel, Matthew. “Universal Principled Review: A Community-Driven Method to Improve Peer Review,” 2019

