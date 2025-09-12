# 📄 Currículo em LaTeX

Este repositório contém um modelo de currículo desenvolvido em **LaTeX**, utilizando a classe [`altacv`](https://github.com/liantze/AltaCV).  
O design foi customizado com uma paleta em tons de **roxo escuro, lilás e verde-água**, mantendo foco em clareza e legibilidade.

---

## 🚀 Como compilar

### Pré-requisitos
- Distribuição LaTeX instalada (TeX Live, MiKTeX ou MacTeX).  
- Compilador **XeLaTeX** ou **LuaLaTeX** (recomendado para suporte às fontes e ícones).  

### Passos
1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/altaCV.git
   cd altaCV
   ```
2. Compile o arquivo principal:
   ```bash
   xelatex main.tex
   ```
   ou
   ```bash
   lualatex main.tex
   ```

O PDF final será gerado como `main.pdf`.

---

## 🎨 Personalização

### Paleta de cores
As cores principais ficam definidas no preâmbulo (`main.tex`):

```latex
\definecolor{PrimaryColor}{HTML}{160C3F}   % Roxo escuro
\definecolor{SecondaryColor}{HTML}{9C7CC2} % Lilás suave
\definecolor{ThirdColor}{HTML}{14B8A6}     % Verde-água / Teal
\definecolor{BodyColor}{HTML}{666666}      % Texto explicativo
\definecolor{EmphasisColor}{HTML}{2E2E2E}  % Títulos em destaque
\definecolor{BackgroundColor}{HTML}{FAFAFA}% Fundo claro
```

### Estrutura
- **Seções**: `\cvsection{Nome da seção}`  
- **Subseções**: `\cvsubsection{Nome da subseção}`  
- **Experiências**: `\cvevent{Cargo}{Empresa}{Período}{Local}` + descrição em `quote`.  
- **Sobre mim** ou descrições: blocos em `quote`, já configurados para usar a cor `BodyColor`.  

### Foto de perfil
Troque o arquivo `linkedin-me.png` pela sua foto e ajuste o tamanho no comando:
```latex
\photoL{4cm}{linkedin-me}
```

---

## 📂 Estrutura do projeto

```
.
├── main.tex        # Arquivo principal do currículo
├── linkedin-me.png # Foto usada no cabeçalho
├── altacv.cls      # classe de documentação
├── README.md       # Este arquivo
```

---

## 📸 Exemplo (Preview)

<img src="/sample.png" width="100%">

---

## ℹ️ Sobre o template

Este projeto é baseado na classe **AltaCV**, criada e mantida pela comunidade:

%%%%%%%%%%%%%%%%%
% This is an sample CV template created using altacv.cls
% (v1.3, 10 May 2020) written by LianTze Lim (liantze@gmail.com). 
% Now compiles with pdfLaTeX, XeLaTeX and LuaLaTeX.
% (v1.7.1b, 11 Jan 2024) forked by Nicolás Omar González Passerino (nicolas.passerino@gmail.com)
%
%% It may be distributed and/or modified under the
%% conditions of the LaTeX Project Public License, either version 1.3
%% of this license or (at your option) any later version.
%% The latest version of this license is in
%%    http://www.latex-project.org/lppl.txt
%% and version 1.3 or later is part of all distributions of LaTeX
%% version 2003/12/01 or later.
%%%%%%%%%%%%%%%%
%% AltaCV uses the fontawesome5 and academicons fonts
%% and packages.
%% See http://texdoc.net/pkg/fontawesome5 and http://texdoc.net/pkg/academicons 
%% for full list of symbols. You MUST compile with XeLaTeX or LuaLaTeX 
%% if you want to use academicons.

---

## 📜 Licença
Este projeto segue a [LaTeX Project Public License (LPPL)](http://www.latex-project.org/lppl.txt).  
Sinta-se à vontade para usar como base e customizar o modelo conforme sua necessidade.
