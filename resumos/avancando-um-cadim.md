# Versionamento de Código com Git e GitHub

## Enviando o baixando alterações com o Repositório Remoto

- Conectar os dois repositórios:

`$git remote add origin url-do-repositorio-remoto`

em seguida

`$git push -u origin main`

- Trazer as alterações do repositório remoto para o repositório local:

`$git pull`

## Trabalhando com branches

- Criando:

`$git checkout -b nome-da-branch-teste`

- Mesclando:

`$git merge nome-da-branch-teste`

- Deletando:

`$git branch -d nome-da-branch-que-quer-excluir`

- Tratando Conflitos:

[Resolvendo conflitos em Git](https://jtemporal.com/resolvendo-conflitos/)