# Tabletop MRI wiki migration report

The `hugo-content` branch adds a native Hugo content tree while preserving the
original MediaWiki extraction in `md_pages/` and downloads in `wiki_files/`.

- Eight archived pages are available under `/tabletop-mri/`.
- Download assets are mounted under `/tabletop-mri/files/` without duplication.
- Links to archived downloads were redirected to their local files where a
  matching file exists.
- The exported `Lecture1.pdf` link was removed because the file was absent from
  the archive.
- Some extracted MediaWiki image markup remains as text and can be cleaned up
  incrementally without blocking the site integration.
