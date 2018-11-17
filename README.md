# [CITi | PTA | 2018.2] Treinamento - Django :pizza:

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

Agora que vocês têm Python na máquina, precisaremos também do Pip. Pip é um instalador (e gerenciador) de pacotes de Python. E é com ele que vamos instalar Django!

Vocês podem conferir a versão do pip fazendo:

```pip --version```

Para instalar o Django, basta fazer:

```pip install django```

E ele será instalado na sua última versão. Caso vocês queiram instalar uma versão específica do Django, vocês podem usar:

```pip install django==2.1```


## Criando um ambiente virtual

Criamos um step-by-step para facilitar:

#### 1. Criar a pasta do projeto
Pelo terminal, vocês vão entrar na pasta onde seu projeto vai ficar (recomendamos que vocês criem uma pasta só para os projetos):

```mkdir django-pta```

Entrem na pasta:

```cd django-pta```

### 2. Criando ambiente virtual
Ainda no terminal, dentro da pasta do projeto, rodem o comando:

```python3 -m venv env```

Caso dê um erro parecido com esse:

```
The virtual environment was not created successfully because ensurepip is not available.  On Debian/Ubuntu systems, you need to install the python3-venv package using the following command.
   apt install python3-venv
You may need to use sudo with that command.  After installing the python3-venv package, recreate your virtual environment.
```
Basta seguir o que o erro pede, rodando na linha de comando do terminal:

```apt install python3-venv```

### 3. Ativando o ambiente virtual
Precisamos agora ativar o nosso ambiente virtual, para que as dependências relacionadas a ele possam funcionar enquanto rodamos nosso projeto. Isso tem que ser feito sempre que vocês quiserem acessar o projeto!

#### Windows

```env\Scripts\activate```

#### Linux

```source env/bin/activate```

Agora vocês podem sair da pasta do ambiente virtual (\env) e vamos criar nosso projeto em Django!

## Criando um projeto em Django :sparkles::sparkles:
Na pasta do projeto (fora da pasta do ambiente virtual!!!), rode o comando:

```django-admin startproject blog```

Isso criará uma pasta chamada blog, e se você entrar nela, vai ver a estrutura de pastas e arquivos de Django (que facilitam nossa vida, amém).

`cd blog`

Vamos agora criar um app (vocês vão entender melhor durante o treinamento). No terminal, rodem:

```python manage.py startapp core```

Viram que surgiu uma pasta core no projeto?

Ok, estamos quase finalizando este tutorial!
Na pasta do projeto, vocês vão notar que existe uma pasta com o mesmo nome da pasta do projeto (blog/blog). Abram o arquivo `settings.py`. Nele, tem uma lista `INSTALLED_APPS`. Basta agora você acrescentar mais um tópico à lista: `'core'` (que é o nome do seu app!).

## Rodando seu projeto!:rocket:

Agora, para terminar, na pasta do projeto mesmo, onde tem o arquivo `manage.py`, vocês vão rodar no terminal:

```python manage.py runserver```

E vão ver algo parecido com isso:

![Projeto rodando](https://glaucocustodio.github.io/assets/rodando-primeiro-projeto-django.jpg)

(Imagem do Google, não tem Glauco aqui).

Quando essa mensagem aparecer, vocês vão acessar no browser o link dado no terminal (nesse caso, `http://127.0.0.1:8000/`).

Se deu tudo certo, vocês vão ver essa página aqui:

![Django Successfull Install](https://wsvincent.com/assets/images/django-auth-mega/welcome.png)

Yayyy, you did it!!! :sparkles::dancer:
