# Versionamento de Código com Git e GitHub

## Instalando o Git no Windows

- Acesse <https://git-scm.com/download/win>;
- Baixar o instalador e executar:
- Aceitar a licença e clicar em 'Next';
- Clica em 'Install' e 'Finish'.

Obs.: Em "Select Components“, deixe as opções “Git Bash Here” e “Git GUI Here” marcadas.

## Configurando o Git

Com o gitbash aberto tem-se na tela do terminal

`nome-usuario@nome-pc nome-compilador endereco-diretorio-aberto $ digite os comandos aqui `

- O comando `git config` retorna informações sobre a ferramenta
- Permite visualizar e configurar variáveis de visualização do git
- O comando CTRL+L limpa o terminal

## Definindo nome e email no git (globalmente)

```
$ git config --global user.name "Nome Sobrenome"
$ git config --global user.email seuemail@gmail.com
```

> Na tela nao retorna nada, mas podemos verificar o valor que foi configurado.

Entendendo...

- Retorna nome e email configurados pelo usuário:

```
$ git config user.name
$ git config user.email
```

- Configura o nome da branch padrão:

`$ git config --global init.defaultBranch main`

- Renomeia a branch padrão:

`$ git config --global --list`

- Retorna todas as configurações globais:

`$ git config --global --list`