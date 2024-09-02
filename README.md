# Latex sample

Simple example of components LaTeX with Russian language.

![preview](data/preview.png)

### Build for Ubuntu 24.04

Install Visual Studio Code:

[https://code.visualstudio.com](https://code.visualstudio.com)

Extensions:

- [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop).
- [LTeX – LanguageTool grammar/spell checking](https://marketplace.visualstudio.com/items?itemName=valentjn.vscode-ltex).
- [Highlight Trailing White Spaces](https://marketplace.visualstudio.com/items?itemName=ybaumes.highlight-trailing-white-spaces).

```shell
code --install-extension valentjn.vscode-ltex
code --install-extension james-yu.latex-workshop
code --install-extension ybaumes.highlight-trailing-white-spaces
```

Visual Studio Code settings:

`~/.config/Code/User/settings.json`

```json
"latex-workshop.latex.build.forceRecipeUsage": false,
"latex-workshop.latex.outDir": "%DIR%/build",
"latex-workshop.latex.magic.args": [
    "-synctex=1",
    "-interaction=nonstopmode",
    "-file-line-error",
    "--output-directory=%OUTDIR%",
    "%DOC%"
],
```

Packages:

```shell
sudo apt-get install \
    latexmk \
    texlive-xetex \
    texlive-extra-utils \
    texlive-latex-extra \
    texlive-lang-cyrillic \
    texlive-fonts-extra \
    font-manager
```

### License

```
Copyright 2024 Vitaliy Zarubin

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
