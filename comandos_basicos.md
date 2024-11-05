# Git básico

## Inicializando um repositorio git
Para começar um envio via git, começamos pelo comando :
 -  ```git init```
 
Feito isso vamos para o segundo passo (git add).

## Adicionando um arquivo no repositorio

O ``git add`` por sua vez, tem ``duas`` formas de serem executadas, vamos lá:
 
   -  `git add index.html`

      - Nesse caso, estou usando um arquivo html para exemplo, mas pode ser qualquer outro tipo de arquivo, seguindo o modelo:
       - index -> nome do meu arquivo .
      - .html -> extensao do arquivo.
      - Esse metódo de ``add`` adiciona arquivo por arquivo.

   - `git add .`
      - Nesse outro caso, ele adiciona todos os arquivos que foram modificados.

## Adicionando commmits
Para adicionar uma mensagem ao seu commit, use.
   - ```git commit -m "msg explicando o commit"```
     - Trocar o que esta entre aspas pelas [boas práticas ao escrever a mensagem de commit](commits.md).

## Mudando de branch:
Para renomear a branch atual para `main` ou `master`, utilize:
   - ```git branch -M main``` ou ```git branch -M master```
   - Porém atualmente, é mais usado a ``main``.
     - A branch `main`, é a principal, caso queira colocar esse projeto atual na branch `principal` use `main`, caso contrário:
     - Caso faça uma outra `branch` [ use boas praticas ao fazer branch](branchs.md). Para criar [uma nova](comandos_avancados.md#gerenciamento-branches)

## Criando o remote
Para adicionar um remote ao seu repositório, execute:

- ``git remote add nomeDoRemote https://github.com/usuario/esseÉUmLinkDoRepositorio.git``
   - O ``git remote add`` é a ligação que você vai fazer do seu comptador (local) com o github (servidor).
    - O **nomeDoRemote** você pode substituir por um nome de **sua escolha**, mas por convenção usamos ``origin``.
    - Não esqueça de **substituir** o link do repositorio pelo **seu link**.

## Enviando os arquivo
Para enviar suas alterações para o repositório remoto, use:
   - ```git push -u nomeDoRemote nomeDaBranch```
     - o **NomedaBranch** normalmente é `main`.
     - O **nomeDoRemote** é o nome que você colocou no passo anterior.
      - Ficando: `git push -u origin main`.
   - Caso você tenha seguido todos os passos e mesmo assim o ``git push`` não funcionou, existe outro metódo, mas ele **NÃO é recomendado** : [forçar git push](comandos_avancados.md#forçando-push)