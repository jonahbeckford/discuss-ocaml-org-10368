# https://discuss.ocaml.org/t/is-dune-just-for-building-targets-or-can-i-also-make-it-organize-build-output/10368

## Setup

```console
$ opam install diskuvbox js_of_ocaml-compiler
```

## Input

```console
$ tree -a -I .direnv -I .git -I .vscode .
.
├── bg.ml
├── common.ml
├── dune
├── dune-project
├── icons
│   ├── pin-32.png
│   ├── pin-64.png
│   ├── pin-dark.svg
│   └── pin-light.svg
├── long_click.ml
├── manifest.json
├── preferences.html
├── prefs.ml
```

## Output

```console
$ tree -a _build/default/output/
_build/default/output/
├── icons
│   ├── pin-32.png
│   ├── pin-64.png
│   ├── pin-dark.svg
│   └── pin-light.svg
├── js
│   ├── bg.bc.js
│   ├── long_click.bc.js
│   └── prefs.bc.js
├── manifest.json
└── preferences.html
```
