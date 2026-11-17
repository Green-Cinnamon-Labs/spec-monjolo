# Livro

O livro desta linha: o meu estudo, escrito conforme eu avanço. Sem sumário fixo; os capítulos entram na ordem em que aparecem.

Escrito em inglês. Compilar: `latexmk -pdf main.tex` nesta pasta (gera `main.pdf`).

## Padrão visual

Definido em [monjolo.sty](monjolo.sty), o mesmo padrão do livro do Hefesto.

- Caixa âmbar, `\begin{history}{ano · lugar}`: uma história, com quem, quando e o que forçou a ideia.
- Caixa azul, `\begin{concept}{nome}`: um conceito-chave, com o que é, o que corrige e o que custa.
- Código em `\begin{code}` (Rust por padrão; Python com `\begin{code}[language=Python]`) e a saída de um comando em `\begin{terminal}`. Todo exemplo foi rodado antes de entrar, e a saída é a que ele imprimiu.
- Diagramas em TikZ, com os estilos `hf/*` do `.sty`, uma cor por papel e a mesma em todas as figuras.

## Índice

Ainda sem capítulos.
