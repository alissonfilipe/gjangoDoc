# 3 parte Django

- https://docs-djangoproject-com.translate.goog/en/5.0/intro/tutorial03/?_x_tr_sl=auto&_x_tr_tl=pt&_x_tr_hl=pt-BR

# comandos para a iniciação

python -m django --version -> verifica se o python está instalado
python -m venv venv -> instalação do ambiente virtual
pip freeze -> verificação da instalação do django

# comandos no desenvolvimento

python manage.py migrate -> serve para fazer as tabelas dos instaled apps no banco de dados configurado(normal sqlite3)
python manage.py makemigrations polls -> dizendo ao django que fez algumas alterações em seus modelos
python manage.py sqlmigrate polls 0001 -> comando pega nomes de migração e retorna seu sql
python manage.py check -> verifica se há problemas em seu projeto sem fazer migrações
python manage.py migrate -> pega todas as migrações que foram aplicadas e executam no seu banco de dados
python manage.py -> sincroniza a alteração que você fez nos modelos com o seu esquema de arquivo base de dados
python manage.py shell -> API gratuíta que Django oferece

# passos da camada models

- Mude seus modelos (em models.py).
- Execute para criar migrações para essas alteraçõespython manage.py makemigrations
- Execute para aplicar essas alterações ao banco de dados.python manage.py migrate

# criação do admin 
- python manage.py createsuperuser -> só seguir com nome email etc

# desenvolvimento

- parei na primeira parte onde crio com HttpResposnse views e urls com parâmetros
