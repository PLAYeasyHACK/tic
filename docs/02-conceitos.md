# Conceitos e comandos essenciais

## Repositório
Pasta onde o Git rastreia as mudanças dos arquivos. Criado com:

git init

Ou copiado de um já existente:

git clone <url>


## Área de stage e commit

git add arquivo.md # adiciona ao stage
git add . # adiciona tudo
git commit -m "mensagem" # registra a mudança no histórico


## Verificar estado

git status # o que mudou
git log # histórico de commits
git diff # diferenças não commitadas


## Branches
Uma branch é uma linha de desenvolvimento paralela.

git branch # lista branches
git checkout -b feature/nome # cria e muda pra nova branch
git checkout main # volta pra main


## Merge
Junta o conteúdo de uma branch em outra.

git checkout main
git merge feature/nome


## Conflitos
Acontecem quando duas branches alteram a mesma linha do mesmo arquivo. O Git marca o trecho conflitante no arquivo:
<<<<<<< HEAD
versão da branch atual

versão da branch que está sendo mergeada

feature/nome

Você edita manualmente, escolhe o que fica, remove as marcações, e faz um novo commit.

## Remoto e GitHub

git remote add origin <url>
git push origin main # envia commits pro GitHub
git pull origin main # traz commits do GitHub


## Pull request
Depois do push de uma branch, abre-se um PR no GitHub pedindo pra mergear ela na `main`. Serve pra revisar as mudanças antes de integrar.