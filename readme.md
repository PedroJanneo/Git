# Repositorio 
- Criado apenas para testar os comandos (pratica)

# Boas praicas commit:
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
- git remote add origin (linkDoRepositorioDoGitHub);
- git push -u origin main;

# Outros comandos:
- git status; (ver as alterações).
- git branch nomeNovaBranch;
- git checkout nomeDaBranch; (mudar de branch)
- git merge nomeDaBranch; (mesclar a branch atual com a escolhida)
- git pull origin nomeDaBranch; (atualizar o repositorio local (da maquina) com o do servidor (github))


# Alguns conceitos:
--> main (branch); <br>
--> origin (nome do remote); <br>
--> extensao: .html. css, etc;<br>
--> o . é tudo modificado; <br>

# Comandos do terminal (auxilia no uso git):
- mkdir nomeDaPasta; -> criar pasta.
- touch nomeDoArquivo.extensao; -> criar arquivo.
- cd nomeDaPasta; ->entar na pasta.
- cd .. ;-> voltar um repositorio(posição).
- ls; -> mostra todos os arquivos dentro da pasta.
- code . ; -> abrir o vs code dentro da pasta.
- git log ou git log --oneline; --> mostrar historicos de commits, o 1º forma geral, o 2º forma resumida. ATENÇÃO: n1 1º opção,presssiona a tecla 'q' em seguida.

# Atalhos
- tecla q; -> interrope as açoes do git.

# Observações

- Depois que você fez o *git push - u origin main* pela primeira vez, nas demais vezes, só digitar *git push*