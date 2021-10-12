# TUTORIAL GIT
## Parabéns aos envolvidos

> Aqui vão os comandos necessários para tornar os projetos comitados pelo git mais flúidos. O Git é sistema de controle de versionamento, isto é, um suporte a mudança de código e suas versões para uma equipe de desenvolvimento.

## 💻 Proposta para organização de branches/Áreas do repositório
- MASTER: linha base, mantém versões em produção.
- DEVELOP: branch para atividades de desenvolvimento/manutenção.
- FEATURE: exclusiva para novas funcionalidades.
- RELEASE: branch para tarefas de bug-fix.
<img src="https://user-images.githubusercontent.com/72531807/136963894-5c8b509e-269e-4fd1-aa76-e440a2504832.png" width="600px;" alt="branchesOrg"/>

- WORKING DIRECTORY: alterações são feitas mas não rastreadas.
- STAGING AREA: fotografia dos arquivos é armazenada.
- LOCAL REPOSITORY: armazenamento das mudanças dos arquivos na máquina.
- REMOTE REPOSITORY: armazenamento das mudanças dos arquivos no GitHub.
<img src="https://user-images.githubusercontent.com/72531807/136963239-a0a65dbf-d0a9-456d-a753-45dd8b17627f.png" width="600px;" alt="commandsOrg"/>

## 🚀 Comandos

### Iniciando um repositório
A partir de um diretório com dados:
```
mkdir seuDiretorio 
cd seuDiretorio
git init 
git add
touch criaFile
```
A partir de um projeto existente em repositório remoto:
```
git clone git://host.org/projrto.git
git clone ssh://username@host.org/projeto.git
```

### Configurando o repositório 
Definir nome e e-mail do autor das mudanças:
```
git config --global user.email endereço_de_email
git config --global user.name nome_sobrenome
```

### Verificações no repositório 
Verificar arquivos versionados e não versionados:
```
git status
```
Verificar alteraçãoes no diretório:
```
git log
git log --graph ---decorate     <!-- apresenta a árvore -->
```
Verificar alteraçãoes não incorporadas no diretório:
```
git diff
git diff arquivo     <!-- mostra alteraçcões em arquivo -->
```

### Atualizando o repositório real
Buscar alterações mais recentes da branch atual armazenadas no repositório remoto:
```
git fetch
git fetch --all     <!-- busca alterações de todas as branchs -->
```
Buscar alterações e incorporá-las no repositório local:
```
git pull
```

### Adicionando/Removendo mudanças no diretório local
Adicionar todas as mudanças:
```
git add
```
Adicionar mudanças de arquivos específicos:
```
git add arquivo1 arquivo2
```
Desfazer alterações de um arquivo:
```
git reset file
```
Desfazer conjunto de alterações de um commit:
```
git revert commit
```

### Confirmando mudanças no repositório local (commit)
Empacotar mudanças em commit e adicionar ao log:
```
git commit
git commit -m "mensagem do commit"
```

### Gerenciamento de branches
Listar branches do repositório:
```
git branch
```
Alterar branch específica:
```
git checkout branch
```
Criar branch e migrar para ela:
```
git checkout -b branch
```
Fundir branch com a atual:
```
git merge branch
```

### Editar arquivo diretamente
Listar branches do repositório:
```
vin arquivo.txt
w -> write
q -> quit
cat arquivo.txt
```

[⬆ Voltar ao topo](#nome-do-projeto)<br>

