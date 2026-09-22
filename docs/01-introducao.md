# Introdução ao controle de versão

## O que é controle de versão
Controle de versão é um sistema que registra o histórico de mudanças em arquivos ao longo do tempo. Permite voltar a versões anteriores, comparar alterações e saber quem mudou o quê e quando.

## Por que usar Git
- Guarda todo o histórico do projeto localmente
- Permite trabalhar em paralelo sem sobrescrever o trabalho dos outros (branches)
- Facilita reverter erros
- É o padrão da indústria — praticamente todo projeto de software usa Git

## Git vs GitHub
- **Git**: ferramenta de controle de versão que roda na sua máquina
- **GitHub**: plataforma online que hospeda repositórios Git e adiciona colaboração (pull requests, issues, revisão de código)

Git funciona sem GitHub. GitHub é só um dos serviços que hospedam repositórios Git (existem outros, como GitLab e Bitbucket).

## Instalação
- **Windows**: baixar em git-scm.com
- **Mac**: `brew install git` ou já vem instalado
- **Linux**: `sudo apt install git` (Debian/Ubuntu) ou equivalente

## Configuração inicial

git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

Essas informações aparecem em cada commit que você fizer.