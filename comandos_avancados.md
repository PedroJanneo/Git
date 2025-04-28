## Clonando Repositórios
- **`git clone https://github.com/usuario/repositorio.git`**: 
  Cria uma cópia do repositório (junto com o histórico e commits).

## Verificando Alterações
- **`git status`**: 
  - Mostra as alterações no repositório.

## Gerenciamento Branches
- Caso for criar uma **branch**, faça um desses comandos logo em seguida do **git init**:
- Ao criar uma nova `branch` [ use boas praticas ao fazer branch](branchs.md)

- **`git branch <nomeNovaBranch>`**: 
  - Cria uma nova branch.

- **`git checkout <nomeDaBranch>`**: 
  - Muda para a branch especificada.

- **`git checkout <nomeDaBranch> | <codigoDaModificacao> | head~N`**: 
  - Muda para a branch e aplica a modificação do commit especificado.

- **`git merge <nomeDaBranch>`**: 
  - Mescla a branch atual (mudar para ```main```) com a branch especificada (nomeDaBranch).

- **``git switch -b <nomeDaBranch>``**
  - Esse comando cria e muda a branch.

**APÓS FAZER O MERGE:**

- **``git branch -d <nomeDaBranch>``**
    -Para apagar a branch (caso vpcê não tenha feito o merge ainda, o git te impede)

- **``git push origin --delete <nomeDaBranch>``**
    - Caso já tenha subido a branch para o github, é so dar esse comando para appagar por lá.

## Atualizando o Repositório Local
- **`git pull origin <nomeDaBranch>`**: 
  - Atualiza o repositório local com as mudanças do repositório remoto (ex.: GitHub).

## Manipulando o Stage e as Modificações
- **`git reset`**: 
 - Remove as alterações do stage (antes de fazer o commit).
  
- **`git clean -df`**: 
 -  Remove arquivos não rastreados e diretórios.

- **`git checkout -- .`**: 
  - Reverte as modificações não comitadas.

## Histórico de Commits
- **`git log`**: 
  - Mostra o histórico de commits (forma geral).
  
- **`git log --oneline`**: 
 -  Mostra o histórico de commits de forma resumida.

  **Atenção**: Na primeira opção, pressione a tecla `q` para sair.

## Mostrando Diferenças
- **`git diff <nomeDoArquivo.extensao>`**: 
  - Mostra as alterações feitas em um arquivo específico.

## Revertendo Commits
- **`git reset --soft head~N`**: 
  - Volta o commit especificado, mantendo as modificações.

- **`git reset --hard <codigoDoCommit>` ou `head~N`**: 
  - Deleta o commit e as modificações.

## Descartar as alterações locais e puxar o do servidor (github)
- **`git reset --hard nomeRemote/Branch`**
  - Substitua o `Branch` por seu caso. (normalmente é ``main`` ou `master`).
  - O ``nomeRemote`` é o mesmo nome de quando você criou um [repositorio](comandos_basicos.md#criando-o-remote)


## Forçando Push
- **`git push -f <nomeDoRemote> <nomeDaBranch>`**: 
  - Força o push do repositório local para o remoto, sobrescrevendo o histórico.
  -Não é recomendado.

## Alterando o Remote
- **`git remote set-url origin https://github.com/usuario/Novorepositorio.git`**: 
  - Altera o repositório remoto, desvinculando o antigo e vinculando o novo.