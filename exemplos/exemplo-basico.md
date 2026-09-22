# Exemplo básico — fluxo completo

Sequência de comandos de um fluxo real, do zero ao merge:

git init
git add .
git commit -m "commit inicial"

git checkout -b feature/nova-secao
git add .
git commit -m "docs: adiciona nova seção"

git push origin feature/nova-secao

abrir PR no GitHub, revisar, mergear

git checkout main
git pull origin main


Esse é o mesmo fluxo usado pra construir este próprio guia.