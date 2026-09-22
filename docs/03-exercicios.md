# Exercícios práticos

## Exercício 1 — Primeiro commit
1. Crie uma pasta e rode `git init`
2. Crie um arquivo `teste.md` com qualquer conteúdo
3. Adicione e commite: `git add teste.md` e `git commit -m "primeiro commit"`
4. Confira com `git log`

## Exercício 2 — Trabalhando com branches
1. Crie uma branch: `git checkout -b feature/exercicio`
2. Edite o `teste.md`, adicione uma linha
3. Commite a mudança
4. Volte pra `main` com `git checkout main` e repare que a mudança não está lá
5. Faça o merge: `git merge feature/exercicio`

## Exercício 3 — Provocando e resolvendo um conflito
1. Na `main`, edite a linha 1 do `teste.md` e commite
2. Crie uma branch a partir de um commit anterior e edite a mesma linha 1 de forma diferente, commitando também
3. Tente mergear — o Git vai acusar conflito
4. Abra o arquivo, escolha a versão final, remova as marcações `<<<<<<<`, `=======`, `>>>>>>>`
5. Adicione e commite a resolução

## Exercício 4 — Pull request no GitHub
1. Dê push de uma branch: `git push origin feature/exercicio`
2. Abra um pull request pela interface do GitHub
3. Mergeie o PR

## Exercício 5 — Desfazendo mudanças
1. Edite um arquivo sem commitar
2. Descarte a mudança: `git checkout -- arquivo.md`
3. Faça um commit, depois desfaça o último commit mantendo as alterações: `git reset --soft HEAD~1`