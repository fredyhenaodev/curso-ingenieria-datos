# curso-ingenieria-datos

## Configuración del ambiente

```python
conda create --name course-data beautifulsoup4 requests numpy pandas matplotlib yaml
```

* beautifulsoup: parsear y manipular html
* requests: permite solicitudes a la web
* numpy: analisis numerico de los datos
* pandas: analisis descriptivos de los datos, modificarlos, etc.
* matplotlib: visualización de los datos.
* yaml: archivo para configuraciones

## Comandos

* activar el ambiente
```python
source activate course-data
conda activate course-data
```
* salir del ambiente
```python
source deactivate
conda deactivate
```
* ambientes virtuales que tenemos

```python
conda env list
```

* eliminar el ambiente
```python
conda remove --name course-data --all
```