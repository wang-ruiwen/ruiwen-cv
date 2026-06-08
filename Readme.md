# Resume Files

## Bilingual set — one page & two pages (EN / 中文)

The requested four-CV set. Same content, two languages, two lengths. SCOPE is
intentionally excluded from the publication lists.

- `cv_en_1page.tex`: English, one page (compact, uses `myresume_industry.sty`).
- `cv_en_2page.tex`: English, two pages (modern layout, uses `myresume_modern.sty`).
- `cv_zh_1page.tex`: 中文，一页 (uses `myresume_cjk.sty`).
- `cv_zh_2page.tex`: 中文，两页 (uses `myresume_cjk.sty`).
- `myresume_cjk.sty`: Chinese (CJK) style package; Latin text reuses the bundled Sabon font.

Compile any of them with XeLaTeX, e.g.:

```powershell
xelatex -interaction=nonstopmode -halt-on-error cv_en_1page.tex
xelatex -interaction=nonstopmode -halt-on-error cv_en_2page.tex
xelatex -interaction=nonstopmode -halt-on-error cv_zh_1page.tex
xelatex -interaction=nonstopmode -halt-on-error cv_zh_2page.tex
```

The Chinese files default to the `fandol` font set (bundled with TeX, compiles on
any platform). On Windows you can switch to system fonts (SimSun / SimHei) by
changing `fontset=fandol` to `fontset=windows` near the top of each `cv_zh_*.tex`.

## Other templates

- `main.tex`: original resume source.
- `main_modern.tex`: redesigned research-oriented resume with stronger visual hierarchy.
- `main_industry.tex`: redesigned 1-page industry-oriented resume for AI systems / ML systems / distributed training roles.
- `main_refined.tex`: refined version that stays close to the original content and section structure while fixing formatting and build issues.
- `main_research.tex`: research-oriented version that stays close to the original content and keeps publications/patents more prominent.
- `myresume.sty`: original style package.
- `myresume_modern.sty`: new modern style package used by `main_modern.tex`.
- `myresume_industry.sty`: compact industry style package used by `main_industry.tex`.
- `myresume_refined.sty`: refined original-style package used by `main_refined.tex`.

# Compile

Use XeLaTeX because the project depends on the local custom fonts in `Fonts/`.

```powershell
xelatex -interaction=nonstopmode -halt-on-error main_modern.tex
```

Industry version:

```powershell
xelatex -interaction=nonstopmode -halt-on-error main_industry.tex
```

Refined original-style version:

```powershell
xelatex -interaction=nonstopmode -halt-on-error main_refined.tex
```

Research version:

```powershell
xelatex -interaction=nonstopmode -halt-on-error main_research.tex
```

If you want the original version instead:

```powershell
xelatex -interaction=nonstopmode -halt-on-error main.tex
```
