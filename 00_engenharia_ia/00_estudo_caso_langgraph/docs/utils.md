# Comandos Úteis

## 0. Ambientes Virtuais

#### 0.1. Criar um ambiente virtual
python -m venv <nome_do_ambiente> # estudo_

#### 0.2. Ativar um ambiente virtual
.\.venv\Scripts\activate.bat

#### 0.3. Deletar um ambiente virtual
deactivate
rm .venv

## 1. GitHub

#### 1.1. Instalar o GitHub Cli
winget install --id GitHub.cli

#### 1.2. Autenticação GitHub Cli
gh auth login

#### 1.3. Vincular a um repositório em branco no github
git remote add origin https://github.com/breno-ferrari-silva/SEU-NOVO-REPOSITORIO.git
git branch -M main
git push -u origin main

#### 1.4. emover um arquivo do versionamento local
git rm --cached secrets/.env

#### 1.5. Remove o histórico de comandos do git (muito util)
Remove-Item -Recurse -Force .git

#### 1.6. Git push destrinchado
git push -u origin main

origin
É o nome de atalho (alias) que aponta para o endereço do seu repositório remoto no GitHub.Por convenção, o Git chama o servidor remoto principal de origin.

main
É o nome da ramificação (branch) para a qual você está enviando os seus arquivos.

-u (ou --set-upstream)
Esta é a parte mais importante do flag. O -u cria um vínculo (tracking link) entre a sua branch local (main) e a branch remota (origin/main).