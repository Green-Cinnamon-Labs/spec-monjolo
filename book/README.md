# Livro

O livro desta linha: o meu estudo, escrito conforme eu avanço. Tem uma parte para cada campo que o projeto atravessa: equações diferenciais e sistemas dinâmicos, métodos numéricos e algoritmos, engenharia de software, otimização e teoria de controle. Dentro de cada parte, os capítulos entram na ordem em que aparecem.

Escrito em inglês. Compilar: `latexmk -pdf main.tex` nesta pasta (gera `main.pdf`).

## Padrão visual

Definido em [monjolo.sty](monjolo.sty), a mesma família de caixas dos livros do Hefesto e do Pítia.

- Caixa âmbar, `\begin{history}{ano · lugar}`: uma história, com quem, quando e o que forçou a ideia.
- Caixa azul, `\begin{concept}{nome}`: um conceito-chave, com o que é, o que corrige e o que custa.
- Caixa verde-azulada, `\begin{question}{pergunta}`: a pergunta boba que ninguém faz em voz alta, e a resposta.
- Caixa roxa, `\begin{reflection}{pergunta}`: uma pausa numa constatação que soa absurda ou que o texto disse de passagem, com o que ela quer dizer e por que é verdade.
- Caixa cinza, `\begin{etymology}`: de onde vêm as palavras.
- Uma caixa só quebra de página se pelo menos 40% dela couber na primeira.
- Código em `\begin{code}` (Rust por padrão; Python com `\begin{code}[language=Python]`) e a saída de um comando em `\begin{terminal}`. Todo exemplo foi rodado antes de entrar, e a saída é a que ele imprimiu.
- Diagramas em TikZ, com os estilos `hf/*` do `.sty`, uma cor por papel e a mesma em todas as figuras.
- Referências entre capítulos e partes por `\ref` (`ch:*`, `part:*`), nunca por número fixo.

## Índice

0. [How to Read This Book](chapters/00-how-to-read.tex): a epígrafe "Lasciate ogne fretta, voi ch'intrate" (Dante, quase: deixai toda pressa), o aviso de que o livro é denso e foi escrito para gente curiosa (o mesmo texto em todos os livros, aqui com código e exemplos para rodar), o projeto que atravessa o livro (o simulador da planta Tennessee Eastman, de Downs e Vogel, 1993), as cinco partes e a pergunta de cada uma, a genealogia com um exemplo por parte (Poincaré, Curtiss e Hirschfelder, a conferência da OTAN de 1968, Dantzig, Minorsky), as cinco caixas, código, a legenda das cores dos diagramas e o mote "fatos exatos, opiniões categóricas".

### Parte I: Differential Equations and Dynamical Systems

Ainda sem capítulos.

### Parte II: Numerical Methods and Algorithms

Ainda sem capítulos.

### Parte III: Software Engineering

Ainda sem capítulos.

### Parte IV: Optimization

Ainda sem capítulos.

### Parte V: Control Theory

Ainda sem capítulos.
