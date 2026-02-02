# DUCK-DB: Exploración y Uso de DuckDB

Este repositorio contiene ejemplos y scripts para explorar las capacidades de [DuckDB](https://duckdb.org/), una base de datos analítica en proceso (OLAP) incrustada y de alto rendimiento. Ideal para análisis de datos local, prototipado rápido y procesamiento eficiente de grandes volúmenes de datos directamente desde tu entorno Python u otros lenguajes.

## Contenido

*   `Untitled0.ipynb`: Un notebook de Jupyter que probablemente demuestra el uso interactivo de DuckDB para análisis de datos.
*   `untitled0.py`: Un script de Python que puede contener lógica para interactuar con DuckDB o realizar operaciones de datos.

## Características Potenciales

*   **Análisis Rápido:** Aprovecha la velocidad de DuckDB para consultas analíticas sobre archivos CSV, Parquet, o directamente en memoria.
*   **Integración Sencilla:** Facilita la integración con Python y el ecosistema de análisis de datos.
*   **Ligero y Potente:** Una solución ideal para escenarios donde se necesita un motor OLAP sin la complejidad de un servidor de base de datos tradicional.

## Instalación y Uso (Ejemplo en Python)

Para empezar con DuckDB en Python, puedes instalarlo con pip:

```bash
pip install duckdb pandas
```

Luego, puedes interactuar con DuckDB en tus scripts o notebooks:

```python
import duckdb
import pandas as pd

# Crear una conexión a una base de datos en memoria o a un archivo
con = duckdb.connect(database=':memory:', read_only=False)

# Cargar datos desde un archivo CSV (ejemplo)
# con.execute("CREATE TABLE my_data AS SELECT * FROM 'path/to/your/data.csv';")

# Ejecutar consultas SQL
# result = con.execute("SELECT COUNT(*) FROM my_data;").fetchval()
# print(f"Número de registros: {result}")

con.close()
```

## 🧑‍💻 Autor

Isaac Haro Ingeniero en Sistemas · Full Stack · Automatización · Data

## 📄 Licencia

MIT — contribuciones bienvenidas 🚀
