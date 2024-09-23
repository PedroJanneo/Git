# Arquivos do Git


## .gitkeep
- **Descrição**: 
  - Um arquivo vazio criado para permitir que uma pasta vazia seja rastreada pelo Git.
- **Uso**:
  - O Git não rastreia pastas vazias. Portanto, se você quiser manter uma estrutura de diretórios, mas não tiver arquivos para colocar na pasta, você pode criar um arquivo chamado `.gitkeep` dentro dessa pasta.
  - **Exemplo**:
    - Se você tem uma pasta chamada `logs/` que está vazia e deseja que ela seja incluída no repositório, crie um arquivo `.gitkeep`:
      ```bash
      touch logs/.gitkeep
      ```

## .gitignore
- **Descrição**: 
  - Um arquivo de configuração que informa ao Git quais arquivos ou pastas devem ser ignorados e não rastreados.
- **Uso**:
  - É útil para excluir arquivos que não precisam ser incluídos no repositório, como arquivos temporários, arquivos de configuração locais ou dependências de desenvolvimento.
  - **Exemplo**:
    - Para ignorar arquivos de log e a pasta de dependências de um projeto, o conteúdo do arquivo `.gitignore` poderia ser:


  
  **DICA**: criar esses arquivos pelo [terminal](terminal.md)