# Tabletop MRI wiki migration report

The `hugo-content` branch adds a native Hugo content tree. The original
MediaWiki extraction in `md_pages/` and downloads in `wiki_files/` remain as
source archives but are not published by the main site.

- Eight archived pages are available under `/tabletop-mri/`.
- Referenced images are stored in their Hugo page bundles.
- Archived ZIP, PDF, CAD, and similar downloads are not published. Pages mark
  those downloads as pending until the responsible PI or project owner adds an
  authoritative external link.
- The exported `Lecture1.pdf` link was removed because the file was absent from
  the archive.
- Extracted MediaWiki image markup and raw HTML links were converted to
  portable Markdown.
