# 🛠️ Comandos Principais do Git

## Configuração e Inicialização
- **`git init`** – Inicializa um repositório Git na pasta atual.
- **`git clone <url>`** – Clona um repositório remoto para a máquina local.
- **`git config --global user.name "Seu Nome"`** – Define o nome do usuário globalmente.
- **`git config --global user.email "seu@email.com"`** – Define o e-mail do usuário globalmente.

## 📂 Trabalho com Branches
- **`git branch`** – Lista as branches no repositório.
- **`git branch <nome>`** – Cria uma nova branch.
- **`git switch <branch>`** – Alterna para outra branch (substitui `git checkout <branch>`).
- **`git merge <branch>`** – Mescla a branch especificada na branch atual.
- **`git rebase <branch>`** – Aplica os commits da branch atual sobre outra branch, reorganizando o histórico.
- **`git branch -d <branch>`** – Deleta uma branch local.
- **`git push origin --delete <branch>`** – Deleta uma branch remota.

## 📌 Adicionando e Confirmando Alterações
- **`git status`** – Mostra o status atual dos arquivos no repositório.
- **`git add <arquivo>`** – Adiciona um arquivo específico para ser commitado.
- **`git add .`** – Adiciona todos os arquivos modificados.
- **`git commit -m "mensagem"`** – Cria um commit com a mensagem especificada.
- **`git commit --amend`** – Edita o último commit (útil para corrigir mensagens ou adicionar arquivos esquecidos).

## 🔄 Sincronização com o Repositório Remoto
- **`git remote -v`** – Lista os repositórios remotos configurados.
- **`git push origin <branch>`** – Envia os commits da branch local para o repositório remoto.
- **`git pull origin <branch>`** – Baixa as mudanças do repositório remoto e mescla com a branch local.
- **`git fetch`** – Baixa as mudanças do repositório remoto sem mesclar automaticamente.

## 🔙 Revertendo Alterações
- **`git restore <arquivo>`** – Restaura um arquivo modificado para sua última versão commitada.
- **`git reset --soft HEAD~1`** – Remove o último commit, mantendo as mudanças no staging.
- **`git reset --hard HEAD~1`** – Remove o último commit e descarta todas as mudanças.
- **`git revert <commit>`** – Cria um novo commit desfazendo as alterações de um commit específico.

## 🏷️ Tags e Versões
- **`git tag <versão>`** – Cria uma nova tag de versão.
- **`git tag -d <versão>`** – Deleta uma tag local.
- **`git push origin --tags`** – Envia todas as tags para o repositório remoto.

## 🔍 Logs e Histórico
- **`git log`** – Exibe o histórico de commits.
- **`git log --oneline`** – Exibe o histórico de commits em uma única linha por commit.
- **`git blame <arquivo>`** – Mostra quem modificou cada linha de um arquivo e em qual commit.
- **`git diff`** – Mostra as diferenças entre arquivos modificados e a última versão commitada.
