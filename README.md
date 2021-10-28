# Instalação

Criando o ambiente virtual python para rodar a documentação

GNU/Linux

```
python3 -m venv .venv
```

Windows

```
python -m venv .venv
```

Ativando o ambiente:

GNU/Linux

```
source .venv/bin/activate
```

Windows

```
.venv\Scripts\activate.bat
```

Instalando as dependências:

```
pip install -r requirements.txt
```

Rodando o Mkdocs:

```
mkdocs serve
```