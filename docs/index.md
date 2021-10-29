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

!!! tip "Versão do vscodium"
    Busque o executável, nomeado de `VSCodiumSetup-x64-1.61.2.exe`

![ex2](\img\vsc-02.png)

## Instalação do Mkdocs

Feita instalação do `Python`, feito isso abra sua IDE de desenvolvimento
(Vscode, Eclipse, Sublime) para o windows, execute o comando 
```
install mkdocs
``` 
caso use linux, no seu gerenciador de pacotes, utilize 
```
sudo apt install mkdocs
```  

## Criando Ambiente Virtual

Criação do ambiente virtual para o desenvolvimento"

Com o terminal aberto em sua máquina, se seu Sistema Operacional for Windows,
execute o comando 
```
python -m venv .venv
```

Caso seja Linux, utilize 
``` 
python3 -m venv .venv
```

## Ativando o ambiente virtual

Para ativar o ambiente virtual, no windows execute o comando 
```
.venv\Scripts\activate.bat
```
    
E no linux 
```
source .venv/bin/activate
```
!!! done "Feito isso seu ambiente está ativado."

![ex2](\img\venv-01.PNG) 

## Rodando o Servidor

Para o servidor rodar execute o comando no terminal 
```
mkdocs serve
```
assim um ip vai ser dado para você. 

![ex3](\img\sv-01.PNG)

Feito isso, seu servidor já está rodando e está pronto para documentar. 

## Padrões de nomenclatura 

- Escrita: Nome de todos os arquivos em inglês.

- Arquivos: Todas as letras minúsculas separados por underline(_) e com 
a extensão .md. Exemplo: ip_permission.md

- Pastas: Todas as letras minúsculas e separadas por underline. Exemplo:
ip_permission

- Fotos: Todas as letras minúsculas e separados por traço(-). 
O nome da imagem tem que ter o prefixo do nome do arquivo que você 
está documentando,
seguido por um numeral começando do um. Exemplo: ip-permission-1.png

# Github
 
## Enviando sua documentação para o GitHub

Sempre que alterar algo em sua documentação, utilize o comando no seu 
terminal
```
git add .
``` 
para adicionar o que foi mudado no seu repositório, feito isso
faça seu commit informando o que foi alterado na documentação utilizando o 
comando 
```
git commit
```  

## Criando uma branch 
    
Para criar uma branch, faremos isso através do comando 
```
git checkout -b nome_da_branch
```
feito isso sua branch está criada, evitando conflitos se você estiver 
trabalhando
em equipe, pois assim, você faz a alteração na sua branch, evitando de 
modificar
a branch `main` do projeto na qual está trabalhando.

## Dando o `push` para o seu repositório

Após adicionar as alterações e comitar, você tem que enviar para o github, 
faremos isso através do comando 
```
git push origin (nome_da_branch)
``` 

## Pull Request 

logo em seguida, você envia um `Pull request` no github para adicionar os 
novos arquivos da sua branch para a main, o `Pull request` será analisado,
e aceito se não houver erros.

## Criando um Pull Request

Com a nova branch criada, alterações adicionadas e o commit feito, iremos 
da um 
```
git push origin (nome_da_branch)
```
assim a pull request foi criada.

![ex](\img\create-pr-02.png) 

## Acessando o GitHub

Abrindo a página do repositório irá aparecer a seguinte mensagem.

![ex](\img\create-pr-03.png)

!!! info "Comparação"
    A pull request será comparada para ver o que foi alterado.

![ex](\img\create-pr-04.png)

Em seguida clique no botão `Create Pull Request` 

!!! done "Feito isso sua Pull Request foi criada!"

![ex](\img\create-pr-05.png)

