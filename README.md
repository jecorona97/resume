# Resume

LaTeX resume built with the [Awesome CV](https://github.com/posquit0/Awesome-CV) template.

## Compiling

This repo uses [Tectonic](https://tectonic-typesetting.github.io/) — a self-contained LaTeX engine that automatically downloads only the packages it needs. No full TeX distribution required.

### Install Tectonic

**macOS (Homebrew):**
```bash
brew install tectonic
```

**Other platforms:** See the [Tectonic installation docs](https://tectonic-typesetting.github.io/en-US/install.html).

### Build the PDF

```bash
tectonic resume.tex
```

On the first run, Tectonic will download any required LaTeX packages automatically. Run it a second time if the output looks incomplete (normal on first compile due to aux file generation).

The compiled PDF will be written to `resume.pdf`.

### Notes

- The template uses XeLaTeX-style font commands. Tectonic handles this natively.
- A patched version of `awesome-cv.cls` is included in this repo with a `\FA` command conflict resolved for compatibility with Tectonic.
