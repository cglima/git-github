# Versionamento de Código com Git e GitHub

## Comandos Úteis no Dia a Dia

`$git fetch origin main`

`$git diff main origin/main`

- Trazer as alterações do repositório remoto para o repositório local:

`$git merge origin/main`

- Clonar um repositorio que tenha varias branches e quer clonar apenas uma branch:

copiar a url do repositorio remoto

`$git clone url-repositorio-remoto --branch branch-que-quer-clonar --single-branch`

- Para arquivar uma alteração que foi feita e nao quer passá-la para outra branch:

`$git stash`

- Para trazer as modificações que foram excluídas na branch:

`$git stash pop`
