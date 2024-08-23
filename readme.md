# Repositorio 
- Criado apenas para testar os comandos (pratica)
- Criando para facilitar o acesso aos comandos (teoria)

# Comandos para configurar 1° vez:
- git config --global user.name "seuNome"
- git config --global user.email "seuEmail@example.com"

# Comandos para desconfigurar:
- git config --global --unset user.name
- git config --global --unset user.email

# Boas praticas commit:
- feat: nova funcionalidade;
- fix: correçao de bugs;
- docs: mudança de documenação;
- style: mudança na formatação (css);
- refactor: melhora a legibilidade do código, sem adicionar funcionalidades nem corrigir bugs (deixar o cod mais limpo);
- test: adição ou correção de testes;
- chore: adiciona novas pastas para organização de build e ferramentas.

# Comandos basicos:
- git init;
- git add nomeDoArquivo.extensao ou git add . 
- git commit -m "msg explicando o commit" --> nao esquecer das boas praticas.
- git branch -M main;
- git remote add nomeDoRemote (linkDoRepositorioDoGitHub);
- git push -u nomeDoRemote nomeDaBranch; --> branch principal é main

# Outros comandos:
- git clone linkRepositorio; -> cria uma copia do reposiorio (junto com o historico e commit)
- git status; (ver as alterações).
- git branch nomeNovaBranch;
- git checkout nomeDaBranch OU **_codigoDaModificacao_** OU head~N; (mudar de branch)
- git merge nomeDaBranch; (mesclar a branch atual com a escolhida)
- git pull origin nomeDaBranch; (atualizar o repositorio local (da maquina) com o do servidor (github))
- git reset; -> tira do stage. (antes de fazer o commit )
- git clean -df; -> tirar as modificações.
- git checkout -- .; --> reverter as modficações, usar junto com o de cima.
- git log ou git log --oneline; -> mostrar historicos de commits, o 1º forma geral, o 2º forma resumida. **ATENÇÃO:** na 1º opção,presssiona a tecla 'q' em seguida.
- git diff nomeDoArquivo.extensao; -> mostra as alterações feitas
- git reset --soft head~N --> voltar o commit sem apagar as modificações.
- git reset --hard codigoDoCommit ou head~N ; -> deletar commit e as modificacao
- git push -f nomeDoRemote nomeDoBranch ; -> forçando o local ser salvo no servidor (destroi o historico)
- git remote set-url origin linkDoRepositorioNovo ; -> vincular com outro repositorio, desvinculando o outro.

# Comandos do terminal (auxilia no uso git):
- mkdir nomeDaPasta; -> criar pasta.
- touch nomeDoArquivo.extensao; -> criar arquivo.
- cd nomeDaPasta; ->entar na pasta.
- cd .. ;-> voltar um repositorio(posição).
- ls; -> mostra todos os arquivos dentro da pasta.
- code . ; -> abrir o vs code dentro da pasta.

# Comandos para restaurar arquivos
    - Esses comandos servem para restaurar aruivos excluidos ( ele puxa do ultimo commit)
- git status; 
- git reset;
- git clean -df;
- git checkout -- . ;

# Alguns conceitos:
--> main (branch); <br>
--> origin (nome do remote); <br>
--> extensao: .html. css, etc;<br>
--> o . é tudo modificado; <br>
--> stage -> git add; <br>
--> ~N -> quantas versões você quer voltar? **LEMBRANDO:** a main é a principal, voce volta apartir dela. ( ~N -> quanidade, tipo, 1,2,3..)

# Observações
- Depois que você fez o **git push - u origin main** pela primeira vez, nas demais vezes, só digitar **git push**.
- **_codigoDaModificacao_** é dado no **git log** ou na **pagina do historicos de commits**.
- Enquanto tiver no **git checkout head~N** não pode alterar o arquivo.
- O **git reset --hard**  ele apaga o historico do commit (do local/maquina), caso voce queira recuperar, **git pull nomeDoRemote mainomeDaBranchn** (ele puxa o ultimo salvo do github).
- Caso voce tenha um repositorio desatualizado em comparação do servidor, e tenha novos arquivos/modificações, use o **git pull nomeDoRemote mainomeDaBranchn** e da o nome do commit de marge.

# Arquivos do git
- .gitkeep -> arquivo inexistente, usado so pra poder subir uma pasta (vazia) pro github.
- .gitignore -> arquivo que não deve ser salvo pelo git. -> pesquisar quando usar o gitignore.

# Atalhos
- tecla q; -> interrope as açoes do git.
- tecla tab -> em algumas ocasiões ela incrementa/completa o nome.
