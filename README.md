# AGENDA

Esta é uma agenda totalmente funcional criada com framework Django. App criado durante o Curso Desenvolvimento para Internet e Banco de Dados com Python e Django da <a href='https://web.digitalinnovation.one/home'>digitalinnovation</a>

# Passos para usados para a criação
- Foi criado uma maquina virtual venv
- O django instalado com os comandos: >pip install django
- Criado um projeto com o comando: >django-admin startproject agenda
- Dentro da pasta agenda foi criado o core da aplicação: >django-admin startapp core
- Foi criado as migrações para o Banco de Dado: >python manage.py migrate
- Foi criado um superusuario de nome admin: >python manage.py createsuperuser --user admin
- O Aplicativo pode ser rodado com o comando: >python manage.py runserver

# Acessando a agenda
- Acessa-se o link <a href='http://127.0.0.1:8000/admin'>http://127.0.0.1:8000/admin</a> para cadastrar novos usuários:

# Criação das tabelas
- criação da class Eventos em models
- criação dos campos para ser preenchidos: titulos, descrição, datas, etc
- Inserção do App core em INSTALLED_APPS
- Criação da class meta com o nome da tabela no banco de dados
- Comandos:
- > python manage.py makemigrations core
- > python manage.py sqlmigrate core 0001
- > python manage.py migrate core 0001
- É feito o registro da class no arquivo admin

# Criação de um template
- Criação de uma pasta templates
- arquivo agenda.html
- criação da rota para a view
- Exibição de eventos 
- Código e comandos python dentro do html {% for x in y %}{{ comandos }} {% endfor %}
- Criação de modelos de extensão

# Autenticação, login e decoradores
- Criação de gerenciamente de login e visualização onde cada usuário somente vê a sua agenda
- Somente staffs e admin consegue administrar a agenda

