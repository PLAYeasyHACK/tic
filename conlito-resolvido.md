# Registro do conflito resolvido

## O que causou o conflito
Duas branches editaram a mesma linha do README.md: uma manteve o texto original, a outra substituiu o conteúdo por "nada".

## Como apareceu
<<<<<<< HEAD
Ensinar os fundamentos de controle de versão com Git e colaboração no GitHub, cobrindo desde a configuração inicial até a resolução de conflitos e pull requests.

nada

feature/ajuste-readme


## Como foi resolvido
Mantive o texto original, já que a versão "nada" não tinha conteúdo real — foi usada só pra provocar o conflito de propósito, como pedido no exercício.

## Comandos usados

git checkout main
git merge feature/ajuste-readme

conflito apareceu aqui
edição manual do README.md

git add README.md
git commit -m "fix: resolve conflito de merge no README"