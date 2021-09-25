# Flask Api para gerenciamento de gastos pessoais

## File config.py

```python
DEBUG = True

USERNAME = 'usuario'
PASSWORD = 'senha'
SERVER = '127.0.0.1'
DB = 'gerenciamento_flask'

SQLALCHEMY_DATABASE_URI = f'mysql://{USERNAME}:{PASSWORD}@{SERVER}/{DB}'
SQLALCHEMY_TRACK_MODIFICATIONS = True

SECRET_KEY = 'Senha-Secreta'
```

## CRUD

Using httpie on terminal for GET, POST, PUT and DELETE.

```bash
http POST :5000/contas nome='Nubank' descricao='Conta do Nubank' saldo=1900.00
http POST :5000/contas nome='C6Bank' descricao='Conta do C6Bank' saldo=1400.00
http GET :5000/contas
http POST :5000/contas nome='inter' descricao='Conta do Inter' saldo=1800.00
http :5000/contas/3
http :5000/contas/5
http DELETE :5000/contas/5
http DELETE :5000/contas/1
http DELETE :5000/contas/1
http :5000/contas
http PUT :5000/contas/2 nome='digio' descricao='Conta do Digio' saldo=9800.90
http :5000/contas
http PUT :5000/contas/3 nome='Inter' descricao='Conta do Inter' saldo=189800.90
http :5000/contas

```
