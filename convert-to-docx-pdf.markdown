To convert the collection of bylaws from markdown to docx or pdf, use [pandoc](https://pandoc.org). 

To insert line breaks after each page, use [pandoc filter](https://pypi.org/project/pandoc-docx-pagebreak/).

	pandoc -o bylaws.docx -f markdown -t docx --filter=pandoc-docx-pagebreakpy README.markdown "! PREAMBLE.markdown" ARTICLE-1.markdown ARTICLE-2.markdown  ARTICLE-3.markdown ARTICLE-4.markdown ARTICLE-5.markdown ARTICLE-6.markdown ARTICLE-7.markdown ARTICLE-8.markdown

**References:**

https://mrjoe.uk/convert-markdown-to-word-document/