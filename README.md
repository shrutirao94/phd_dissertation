# PhD dissertation template

Use this folder as the single source folder.

## Which file to compile

- `main-final.tex` is the final dissertation build. Use this for the real dissertation/book rhythm, including recto-opening front matter and truly blank blank pages.
- `main.tex` is only the compact preview build. Use this for faster visual checking while editing.

Both builds use the same typography, chapter styling, fixed non-mirrored Tufte text column, and right-margin sidenotes.

## Compile

```bash
latexmk -lualatex main-final.tex
```

For preview mode:

```bash
latexmk -lualatex main.tex
```

## Edit first

1. Edit `metadata.tex` for title, author, date, faculty, and university details.
2. Replace/add chapter files in `chapters/`.
3. Add references to `references.bib`.
4. If needed, place the official signed/institutional approval page at `frontmatter/approval-page.pdf`. If absent, that page is left blank.

## Notes

This package intentionally contains one template folder only. Older duplicate/staging folders such as `turon_v10_clean` should be ignored if they appear elsewhere.
