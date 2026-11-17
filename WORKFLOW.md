# Como trabalho nesta linha

O método é o mesmo da linha Hefesto ([`spec-hefesto/WORKFLOW.md`](https://github.com/Green-Cinnamon-Labs/spec-hefesto/blob/main/WORKFLOW.md)). Aqui fica só o que muda.

## Papéis

- **Eu escrevo todo o código**, digitando. O Claude não edita nem commita nos repositórios de código.
- **O Claude guia.** Em cada versão ele responde assim: "arquivo:linha hoje está assim → mude para → por quê (1 a 3 linhas)", e diz como conferir. A teoria não fica na sessão: vai para o livro, que eu dito.
- O Claude pode escrever e commitar documentação neste hub.

## Onde ficam as issues

Todas as issues da linha ficam **neste hub**, não nos repositórios de código (o `tep-plant` nem tem issues ligadas). O título diz o repositório: `[monjolo]`, `[tep-plant]`, `[tep-optimizer]` ou `[tep-plant/monjolo]`. No [board](https://github.com/orgs/Green-Cinnamon-Labs/projects/12), Linha = Monjolo.

Como a issue mora em outro repositório, os commits e PRs a citam com o nome completo: `Refs Green-Cinnamon-Labs/spec-monjolo#14`.

## Versões progressivas

As issues novas (#14 em diante) já vêm em versões: uma **v0 ingênua**, e cada versão seguinte corrige **uma** coisa que eu observei. As antigas (#1 a #13) têm só uma lista de escopo; cada uma ganha versões quando eu começar a trabalhar nela.

## GitHub Flow

1. Uma branch por issue no repositório de código: `<tipo>/<n>-<resumo>`, por exemplo `build/14-git-dependency`.
2. Um commit por versão.
3. Um comentário na issue por versão, com o que quebrou, por quê e o que mudou.
4. PR em inglês, merge sem squash.

## Commits

[Conventional Commits](https://www.conventionalcommits.org/), em inglês, com `Refs Green-Cinnamon-Labs/spec-monjolo#N`.

## Repositórios

Ficam todos lado a lado em `C:\Projetos\gclabs\`, e o workspace é o [`monjolo.code-workspace`](monjolo.code-workspace):

| Pasta | O que é |
| --- | --- |
| `spec-monjolo` | este hub: o livro, as issues e este fluxo |
| `monjolo` | o runtime de simulação, em Rust |
| `tep-plant` | a planta TEP sobre o `monjolo` |
| `tep-optimizer` | o otimizador, em Python, que chama a planta como função |

## A planta é desta linha

O `tep-plant` se desenvolve aqui. As outras linhas (Hefesto, Gajeiro) só rodam a planta, sem abrir o código: ver "Subir a planta" no `WORKFLOW.md` do Hefesto. Enquanto o `tep-plant` depender de `path = "../monjolo"` (#14), os dois precisam estar clonados lado a lado.
