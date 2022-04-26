### Create a virtual enviroment
```bash
virtualenv venv
```

### Active the virtual enviroment created using source command
```bash
source venv/Scripts/activate
```

### Install the Django framework using [pip](https://pip.pypa.io/en/stable/)
```bash
pip install django djangorestframework django-cors-headers
```

**django-admin startproject project-name**: django-admin é um utilitário de linha de comando usado para realizar tarefas com o Django. O comando startproject cria um novo projeto Django.

**python manage.py startapp myapp**: manage.py é um script utilitário, adicionado automaticamente a cada projeto Django, que executa uma série de tarefas administrativas: criar novos aplicativos, migrar o banco de dados e atender ao projeto Django localmente. Seu comando startapp cria um aplicativo Django dentro do projeto Django. No Django, o termo aplicativo descreve um pacote Python que fornece alguns recursos em um projeto.

### Crie o projeto Django
```bash
django-admin startproject <nome_projeto>
```

### Folders
```bash
├── djangoreactproject
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── manage.py
```

### A pasta **~/djangoreactproject** é a raiz do projeto. Dentro dessa pasta, há vários arquivos que serão importantes para seu trabalho:

**manage.py**: o script utilitário que faz uma série de tarefas administrativas.

**settings.py**: o arquivo de configuração principal para o projeto Django onde você pode modificar as configurações do projeto. Essas configurações incluem variáveis como INSTALLED_APPS, uma lista de strings que designam os aplicativos habilitados para seu projeto. A documentação do Django tem mais informações sobre as [configurações disponíveis.](https://docs.djangoproject.com/en/2.0/ref/settings/)

**urls.py**: este arquivo contém uma lista de padrões de URL e visualizações relacionadas. Cada padrão mapeia uma conexão entre um URL e a função que deve ser chamada para aquele URL. Para obter mais informações sobre URLs e visualizações, consulte nosso tutorial em [Como Criar Visualizações no Django.](https://www.digitalocean.com/community/tutorials/how-to-create-views-for-django-web-development)


### CORS
Você pode encontrar mais opções de configuração nos [django-cors-headers](https://github.com/adamchainz/django-cors-headers#configuration) docs. 


### Migrations and Models
[Migrações](https://docs.djangoproject.com/en/2.0/topics/migrations/) consistem no modo que o Django tem de propagar as alterações que você faz nos modelos do esquema do seu banco de dados. Essas alterações podem incluir coisas como adicionar um campo ou excluir um modelo, por exemplo. Para saber mais sobre modelos e migrações, consulte o tópico Como [Criar Modelos do Django.](https://www.digitalocean.com/community/tutorials/how-to-create-django-models)