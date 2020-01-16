## Realizar solicitudes HTTP con Python
Para poder experimentar con la web necesitamos un método programático para solicitar URLs y obtener HTML

Requests: Nos permite generar solicitudes a la web dentro de Python y utilizar los diferentes verbos HTTP, normalmente utilizaremos el método GET porque vamos a traer datos.

```python
requests.get('url')  // para hacer una solicitud a la web y nos devolverá un objeto response
```
Todas las solicitudes HTTP tienen metadatos para que los diferentes sistemas y computadoras puedan entender de qué va la solicitud.

Ejemplo 

```python
import requests

response = requests.get('https://www.platzi.com')

response??

print(dir(response))

print(response.status_code)
print(response.headers)
print(response.headers['date'])
print(response.text)
```