## ¿Cómo trabajar con un documento HTML?

En el caso de Python la librería estándar para manipular los documentos HTML se llama BeautifulSoup.

BeautifulSoup nos ayuda a organizar gramaticalmente(parsear) el documento HTML para que tengamos una estructura con la cual podamos manejar y extraer información. BeautifulSoup convierte el string de HTML en un árbol de nodos para poder manipularlo.

Para manipularlo podemos usar los selectores CSS con soup.select()

### Ejemplo

```python
import requests
import bs4

response2 = requests.get ('https://platzi.com/categorias/desarrollo/')
soup2 = bs4.BeautifulSoup(response2.text, 'html.parser')

courses_links = soup2.select('.LearningPathItem')

courses = [course['href'] for course in courses_links]
 
for course in courses:
    print(course)
```