# Comandos Git
## Criar repositório
- Para iniciar uma repositorio no projeto

    ```bash
    git init
    ```

- Para configurar a branch padrão para todos os projeto da maquina

    ```bash
    git config --global init.defaultBranch main
    ```
    > **Nota**: o padrão da branch principal é main 

- Para saber o status do seu repositório

    ```bash
    git status
    ```
- Para ***Deletar*** o Repositório git
    
    ```bash
    rm -fr .git
    ```
    > **Aviso**: Evite deletar a pasta .git
## Adicionar Mudanças
- Para adicionar arquivos ou pastas para o git começar a monitorar suas mudanças
    
    **Arquivos**
    ```bash
    git add arquivo.txt
    ```
    **Pastas**
    ```bash
    git add ./pastas
    ```
    **Tudo**
    ```bash
    git add .
    git add -A
    git add --all
    ```
## Remover Arquivos Adicionados
- Para remover arquivos ou pastas adicionados ao git por engano
    **Tudo**
    ```bash
    git rm --cached -r .
    ```
    **Arquivos**
    ```bash
    git rm arquivo.txt
    ```
    **Pastas**
    ```bash
    git rm ./pastas
    ```
## Salvar Mudanças
- Para salvar as mudanças de arquivos ou/e pastas adicionados ao git
    ```bash
    git commit -m "mensagem"
    ```
    > **Nota**: o commit só irá registrar os arquivos que já estão registrados no repositório por isso use o `git add` para registrar novos arquivos e `git status` para ver quais arquivos não estão no repositório
## 4 Estados do arquivo
![Alt text](image.png)

## Visualizar alterações
- Para exibir todas as diferenças entre seus commits, branch e cópias locais e o índice sincronizado

    ```bash
    git diff
    ```