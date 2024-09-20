# Git básico

Para configurar o Git pela primeira vez, siga estes passos:

1. Para definir o nome de usuário global para o Git, use:
   - ```git config --global user.name "seuNome"```
     - Substitua `"seuNome"` pelo seu nome completo.

2. Para definir o e-mail global para o Git, utilize:
   - ```git config --global user.email "seuEmail@example.com"```
     - Substitua `"seuEmail@example.com"` pelo seu e-mail.
     
Para começar um envio via git, começamos pelo comando :
 -  ```git init```
 
Feito isso vamos para o segundo passo :
 -  `git add index.html`

    - Nesse caso, estou usando um arquivo html para exemplo, mas pode ser qalquer outro tipo de arquivo, seguindo o modelo:
    - index -> nome do meu arquivo 
    - .html -> extensao do arquivo
 - `git add .`
    - Nesse outro caso, ele adiona todos os arquivos que foram modificados.

Para adicionar uma mensagem ao seu commit, use:
   - ```git commit -m "msg explicando o commit"```
     - Não esquecer das [boas práticas ao escrever a mensagem de commit](readme.md#boas-praticas-commit).

Para renomear a branch atual para `main`, utilize:
   - ```git branch -M main```
     - Por convenção, usamos a branch `main`, mas existem exceções.

Para adicionar um remote ao seu repositório, execute:

- ```git remote add origin https://github.com/usuario/repositorio.git```
    - o nome 'origin' é dado pela boa prática.
    - não esqueça de substituir o link do repositorio pelo seu link.

Para enviar suas alterações para o repositório remoto, use:
   - ```git push -u nomeDoRemote nomeDaBranch```
     - o **NomedaBranch** normalmente é `main`.
     - O **nomeDoRemote** é o mesmmo do passo anterior, por convenção e praticidade, sugiro colocar `origin`.
      - Ficando: `git push -u origin main`.