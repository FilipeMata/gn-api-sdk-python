### Canceling the carnet

Only `active` carnets can be canceled:

```python
# encoding: utf-8

from gerencianet import Gerencianet

credentials = {
    'client_id': 'client_id',
    'client_secret': 'client_secret',
    'sandbox': True
}

gn = Gerencianet(credentials)

params = {
    'id': 1
}

response =  gn.cancel_carnet(params=params)
print(response)

```

If everything goes well, the return will be:

```python
{
  "code": 200
}
```
