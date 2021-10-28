# Como Documentar? 

O processo de documentação consiste em, organizar um conjunto de documentos com
 o propósito de esclarecer ou provar alguma coisa.

!!! tldr "Vamos documentar"

    Como vamos fazer isso? 

## Primeiros passos

Primeiro devemos saber o que deve ser documentado, diante disso, iremos 
elaborar
um padrão a ser seguido pela documentação, para quando outra pessoa consultar,
seja algo claro e simples de ser entendido.

## Instalação do Python

!!! tldr "Para instalar"

    Entre no link <a href="https://www.python.org/downloads/release/python-390/" 
    target = "_blank">clicando aqui</a>.

    Em seguida, baixe o Instalador, como segue no anexo abaixo:

![ex1](\img\py-01.PNG)

## Instalação do VSCodium

!!! tldr "Como instalar"
    Entre no site do VSCodium <a href="https://vscodium.com/" target = "_blank">
    clicando aqui</a>.
    
    E aperte em `Download latest release` para baixar.

![VSCodium1](\img\vsc-01.PNG)

## Instalação do Mkdocs

!!! tldr "Instalando o Mkdocs"

    Feita instalação do `Python`, feito isso abra sua IDE de desenvolvimento
    (Vscode, Eclipse, Sublime) e execute o comando `install mkdocs` para 
    windows,
    caso use linux, no seu gerenciador de pacotes, utilize `sudo apt 
    install mkdocs`  

## Criando Ambiente Virtual

!!! tldr "Criação do ambiente virtual para o desenvolvimento"

    Com o terminal aberto em sua máquina, execute o comando `python -m venv 
    .venv`

    se seu Sistema Operacional for Windows, Caso seja Linux, utilize `python3 
    -m venv .venv`

!!! tldr "Ativando o ambiente virtual"

    Para ativar o ambiente virtual, execute o comando
     `.venv\Scripts\activate.bat`
    no windows, 
    
    E no linux `source .venv/bin/activate`, feito isso seu ambiente 
    está ativado.

![ex2](\img\venv-01.PNG) 

## Rodando o Servidor

git push -u origin main

    Para o servidor rodar execute o comando no terminal `mkdocs serve`, assim 
    um ip vai ser dado para você. 

![ex3](\img\sv-01.PNG)

Feito isso, seu servidor já está rodando e está pronto para documentar. 

## Padrões de nomenclatura 

!!! info "Padrão de nomenclatura"

    - Escrita: Nome de todos os arquivos em inglês.
    - Arquivos: Todas as letras minúsculas separados por underline(_) e com 
    a extensão .md. Exemplo: ip_permission.md
    - Pastas: Todas as letras minúsculas e separados por underline. Exemplo:
    ip_permission
    - Fotos: Todas as letras minúsculas e separados por traço(-). 
    O nome da imagem tem que ter o prefixo do nome do arquivo que você 
    está documentando,
    seguido por um numeral começado do um. Exemplo: ip-permission-1.png

## Github
 
!!! tldr "Enviando sua documentação para o GitHub"

    Sempre que alterar algo em sua documentação, utilize o comando no seu 
    terminal
    `git add .` para adicionar o que foi mudado no seu repositorio, feito isso
    faça seu commit informando o que foi alterado na documentação utilizando o 
    comando `git commit`  

!!! tldr "Dando o `push` para o seu repositorio"

    Após adicionar as alterações e comitar, você tem que enviar para o github, 
    faremos isso através do comando `git push (nome-da-branch)` 

!!! tldr "Criando uma branch" 
    
    Para criar uma branch, faremos isso através do comando `git checkout -b 
    nome_da_branch`,
    feito isso sua branch está criada, evitando conflitos se você estiver 
    trabalhando
    em equipe, pois assim, você faz a alteração na sua branch, evitando de 
    modificar
    a branch `main` do projeto na qual está trabalhando, em seguida você envia
    envia uma `Pull request` para avisar que alterações forem feitas no projeto
    logo em seguida, essa `Pull request` será analizada, e consequentemente 
    aceita
    se não houver erros.