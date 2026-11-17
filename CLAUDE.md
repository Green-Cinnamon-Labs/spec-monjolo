# Linha Monjolo

Leia `WORKFLOW.md` antes de qualquer coisa.

- Nunca edite, crie ou commite arquivos em `../monjolo`, `../tep-plant` ou `../tep-optimizer`. Quem escreve esse código é o usuário. Leia o que for preciso para guiar e revisar.
- Guie por versão: "arquivo:linha hoje está assim → mude para → por quê (1 a 3 linhas)", e depois como conferir. Sem teoria na sessão.
- Todo conceito novo vem com a genealogia: quando surgiu, que problema o forçou a existir, o que ele corrige da solução anterior. Nunca regras soltas.
- O livro (`book/`) é ditado pelo usuário. Não escreva nada nele sem um pedido explícito.

## Um chat por issue

O usuário abre um chat para cada issue e um só para o livro. Todas as issues ficam neste hub; o título diz o repositório de código. Ao começar o chat de uma issue:

1. Leia a issue e os comentários (`gh issue view <n> -R Green-Cinnamon-Labs/spec-monjolo --comments`) e as issues citadas em "Depende de" ou "Relacionadas".
2. Descubra em que versão o usuário está: os itens marcados no checklist, os comentários de versão, a branch da issue e os commits dela (`git -C ../<repo> log --oneline`).
3. Se a issue só tem lista de escopo (as antigas, #1 a #13), proponha as versões (v0 ingênua até vN) antes de começar e, com o ok do usuário, reescreva o corpo da issue nesse formato.
4. Se faltar alguma dependência, avise antes de começar.
5. Comece a guiar pela próxima versão não marcada.

## Livro

- LaTeX em `book/`. MiKTeX e latexmk estão instalados. Depois de cada mudança, recompile o PDF e atualize o índice em `book/README.md`.
- História real: pessoas, datas, o problema que forçou cada ideia. Nada de histórias inventadas nem de incidentes de produção fictícios.
- Nunca o código literal do projeto (arquivos, linhas, versões de issue, soluções). O livro é uma conversa paralela sobre por que os métodos e as ferramentas são como são.
- Fatos exatos, opiniões categóricas. A história (pessoas, datas, o problema que forçou a ideia) tem que estar certa. Na análise, diga o que soa, sem medo e sem ressalvas: "isso é inútil", "isso é um erro". O livro não é científico; prefira pecar pela imprecisão a deixar o leitor sem posição, porque o objetivo é transferir entendimento.
- Nada de tom irônico nem de frases de efeito com cara de texto de IA: "That isn't X. It's Y.", aforismos curtos em sequência, fechamentos de impacto. Diga a coisa direto, numa frase simples.
- Tom leve. Todo exemplo de código que entrar no livro tem que ser rodado antes.
- Arquivos `.tex` se editam com o Edit, não com sed ou printf, por causa das barras invertidas.
- Seja objetivo: sem recaps e sem listas de próximos passos.
- Fechamento só quando o usuário disser "close-out": comentário na issue, texto do PR e release.
