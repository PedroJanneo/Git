# Git básico

Para começar um envio via git, começamos pelo comando :
 -  ```git init```
 
Feito isso vamos para o segundo passo (git add) :

O ``git add`` por sua vez, tem duas formas de serem executadas, vamos lá:
 
   -  `git add index.html`

      - Nesse caso, estou usando um arquivo html para exemplo, mas pode ser qualquer outro tipo de arquivo, seguindo o modelo:
       - index -> nome do meu arquivo .
      - .html -> extensao do arquivo.
      - Esse metódo de ``add`` adiciona arquivo por arquivo.

   - `git add .`
      - Nesse outro caso, ele adiciona todos os arquivos que foram modificados.

Para adicionar uma mensagem ao seu commit, use:
   - ```git commit -m "msg explicando o commit"```
     - Não esquecer das [boas práticas ao escrever a mensagem de commit](commits.md).

Para renomear a branch atual para `main`, utilize:
   - ```git branch -M main```
     - A branch `main`, é a principal, caso queira colocar esse projeto atual na branch `principal` use `main`, caso contrário:

     - Caso faça uma outra `branch` [ use boas praticas ao fazer branch](branchs.md). Para criar [uma nova](comandos_avancados.md#gerenciamento-branches)

Para adicionar um remote ao seu repositório, execute:

- ```git remote add origin https://github.com/usuario/repositorio.git```
   - O ``remote`` é a ligação que você vai fazer do seu comptador (local) com o github (servidor).
    - o nome 'origin' é dado pela boa prática.
    - não esqueça de substituir o link do repositorio pelo seu link.

Para enviar suas alterações para o repositório remoto, use:
   - ```git push -u nomeDoRemote nomeDaBranch```
     - o **NomedaBranch** normalmente é `main`.
     - O **nomeDoRemote** é o mesmmo do passo anterior, por convenção e praticidade, sugiro colocar `origin`.
      - Ficando: `git push -u origin main`.