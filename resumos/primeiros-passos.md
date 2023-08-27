# Versionamento de Código com Git e GitHub

## Criando e Clonando Repositórios

Existem duas maneiras de obter um repositório Git:

1. Transformando um diretório local que não está sob controle de versão, em um repositório Git
2. Clonando um repositório Git existente

### 1. Criando um Repositório Local

Acesse a pasta que deseja transformar em um repositório Git pelo terminal ou clique no atalho em “Git Bash Here”:

- Abra o gitbash na pasta desejada para criar um repositório:

`$ mkdir nome-do-diretorio`

- Para acessar o diretorio criado:

`$ cd nome-do-diretorio`

- Inicialize um repositório Git no diretório escolhido:

`$ git init`

### 2. Clonando o Repositório

- Pega o link gerado no github na aba do HTTPS:

`$git clone url-copiada-do-github`

- Renomeando a pasta que foi clonada:

`$git clone url-copiada-do-github novo-nome-da-pasta-clonada`

### 3. Salvando alterações no repositório local

- Verificando o status do repositório:

`$git status`

- Criando um arquivo README.md:

`$ touch README.md`

- Colocando o arquivo README.md no estágio de preparação:

`$ git add README.md`

- Verifica novamente o status do repositório:

`$git status`

- Colocando o arquivo dentro de um commit:

`$git commit -m"commit inicial"`

- Exibindo o commit que foi feito:

`$git log`

- Criando o .gitignore:

(a pasta resumos não está sendo reconhecida pelo .gitignore)

`$echo resumos/ > .gitignore`

- Inserindo todos os arquivos do diretório para a preparação:

 `$git  add .`

### 4. Desfazendo alterações no Repositório Local

- Se usou o comando no diretório errado

`$ git init`

basta excluir o trecho /.git/ utilizando o comando:

`$ rm -rf .git`

- Para retornar ao ultimo estágio, caso tenha apagado informações do arquivos indesejada:

`$ git restore nome-do-arquivo-para-restaurar`

- Alterando a última mensagem do commit:

`$git commit --amend -m"nova msg"`

- Desfazer o commit e retornar ao commit anterior:

`$git reset --soft cola-o-hash-do-commit`

**OU** podemos utilizar este comando padrão do reset:

`$git reset --mixed hash-do-commit-`

**Ou AINDA** este comando ignora todos os arquivos que não estavam no commit que queremos retornar (anterior):

`$ git reset --hard hash-do-commit`

- Retirando arquivos que estão na área de preparação:

`$git reset nome-do-arquivo-que-quer-excluir`

`$git restore --staged nome-do-arquivo-que-quer-excluir`