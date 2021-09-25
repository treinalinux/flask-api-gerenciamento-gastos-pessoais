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
