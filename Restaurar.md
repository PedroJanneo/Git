# Restaurar por Git

## 1. `git status`
Exibe o estado atual do repositório. Mostra os arquivos modificados, adicionados, e se há arquivos não rastreados. É útil para entender o que precisa ser feito antes de um commit.

## 2. `git reset`
Desfaz alterações em commits ou arquivos. O comportamento pode variar:
- `git reset --soft HEAD~1`: Remove o último commit, mantendo as alterações na área de stage.
- `git reset HEAD~1`: Remove o último commit e as alterações vão para a área de trabalho.
- `git reset --hard HEAD~1`: Remove o último commit e descarta todas as alterações.

## 3. `git clean -df`
Remove arquivos não rastreados do diretório de trabalho. 
- `-d`: Remove diretórios não rastreados.
- `-f`: Força a remoção (necessário para que o comando funcione).

**Atenção**: Use este comando com cuidado, pois ele apaga permanentemente arquivos.

## 4. `git checkout -- .`
Desfaz todas as alterações não comitadas em arquivos rastreados no diretório de trabalho. O ponto (`.`) indica que a operação deve ser realizada em todos os arquivos do diretório atual.

---

Esses comandos são bastante poderosos, então sempre tenha cuidado ao utilizá-los, especialmente `git reset` e `git clean`.
