# Termos e Conceitos do Git

## Branch
- **`main`**: 
  - A branch principal do projeto.
  - **Exemplo**: Geralmente, o código estável é mantido na branch `main`.

## Remote
- **`origin`**: 
  - Nome padrão do repositório remoto.
  - **Exemplo**: Ao clonar um repositório, ele é automaticamente associado ao remote chamado `origin`.

## Extensões de Arquivo
- **Extensões**: 
  - Usadas para identificar o tipo de arquivo.
  - **Exemplo**:
    - `.html`: Arquivos de hipertexto.
    - `.css`: Arquivos de estilo em cascata.
    - `.js`: Arquivos de JavaScript.


## Stage
- **`stage`**: 
  - Fase onde as alterações são preparadas antes de serem comitadas.
  - **Exemplo**: Após usar `git add`, os arquivos vão para o stage, prontos para o commit.

## Voltar Commits
- **`~N`**: 
  - Indica quantos commits você deseja voltar na linha do tempo.
  - **Exemplo**:
    - `head~1`: Volta um commit.
    - `head~2`: Volta dois commits.
  - **Observação**: A `main` é a branch principal e os comandos de voltar são executados a partir dela.
