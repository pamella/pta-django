# :pizza: [CITi | PTA | 2018.2] Treinamento - Django

## Instalação de ferramentas
Vamos precisar de duas coisas basiquinhas (e essenciais) para este treinamento: **Python** e **Django**.

### Instalando Python na sua máquina
#### Windows
Por motivos de agilidade, usem o site para fazer o download de Python. Este site [aqui](https://www.python.org/downloads/).
#### Linux
Vocês podem seguir o procedimento do Windows, ou (mais simples), usar o terminal. Basta usar o comando:

```sudo apt install python3.7```

Confiram se o Python foi instalado digitando ```python```no terminal! 
Done!


### Instalando Django na sua máquina

Quando Python é instalado na sua máquina, ele vem com o **pip**. Pip é um instalador (e gerenciador) de pacotes de Python. E é com ele que vamos instalar Django! (Que crossover, bicho)

Para instalar o Django, basta fazer:

```pip install django```

E ele será instalado na sua última versão. Caso vocês queiram instalar uma versão específica do Django, vocês podem usar:

```pip install django==2.1```


## Criando um ambiente virtual

Criamos um step-by-step para facilitar:

#### 1. Criar a pasta do projeto
Pelo terminal, vocês vão entrar na pasta onde seu projeto vai ficar (recomendamos que vocês criem uma pasta só para os projetos):

```mkdir projeto```

Entrem na pasta:

```cd projeto```

### 2. Criando ambiente virtual
Ainda no terminal, dentro da pasta do projeto, rodem o comando:

```python3 -m venv env```

Caso dê um erro parecido com esse:

```The virtual environment was not created successfully because ensurepip is not available.  On Debian/Ubuntu systems, you need to install the python3-venv package using the following command.
   apt install python3-venv
You may need to use sudo with that command.  After installing the python3-venv package, recreate your virtual environment.```
