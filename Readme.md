# Resume Files

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
