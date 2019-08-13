# Arquitetura Dinâmica para o Gerenciamento de Memória em Aplicações com Reuso de Dados no Apache Spark

## Dissertação de Mestrado - Programa de Pós-Graduação em Ciência da Computação

**Universidade Federal de Santa Maria -- Santa Maria/RS -- 2019**

**Aluno**: Maurício Matter Donato

**Orientador**: Dra. Patrícia Pitthan de Araujo Barcelos


## Instruções para compilação

O seguinte documento foi projetado usando [TeXLive](https://www.tug.org/texlive/) e [Visual Studio Code](https://code.visualstudio.com).

Para uma build correta em um ambiente debian-based linux, você pode precisar dos seguintes pacotes:

* [abntex](https://packages.debian.org/buster/abntex)
* [texlive-latex-extra](https://packages.debian.org/buster/texlive-latex-extra)
* [texlive-luatex](https://packages.debian.org/buster/texlive-luatex)
* [texlive-publishers](https://packages.debian.org/buster/texlive-publishers)

Para um build correta no MacOS:

* [MacTex](https://www.tug.org/mactex/)
      
      pdflatex --file-line-error --synctex=1 --shell-escape main.tex

### Observações

* O template é uma versão customizada da versão 1.08 do MDT UFSM. As seguintes modificações foram aplicadas ao arquivo [`ufsm_2015.cls`](blob/master/ufsm_2015.cls):
  * Adição da importação de um documento pdf para substituir a folha de aprovação (linhas [1194](blob/master/ufsm_2015.cls#L1194) ~ [1301](blob/master/ufsm_2015.cls#L1301)). Comente/descomente para alternar entre a importação do pdf e a geração da folha vazia. O documento deve possuir o nome `banca.pdf`;
  * Adição do número sequencial do trabalho à folha de rosto (linha [1137](blob/master/ufsm_2015.cls#L1137)). Descomente para ativar e remova as chaves duplas `{{` do começo da linha [1138](blob/master/ufsm_2015.cls#L1138);
  * Adição de suporte à citação longa no padrão do MDT (linhas [858](blob/master/ufsm_2015.cls#L858) ~ [870](blob/master/ufsm_2015.cls#L870). 4 cm à esquerda da margem, fonte 10, espaçamento simples). Para fazer uma citação longa, use o environment `citacao`.
* Template atualizado por [Rafael Trindade](https://github.com/648trindade)