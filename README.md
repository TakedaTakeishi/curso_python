# Curso Takeishi — Python desde Cero

Curso práctico de Python 3 pensado para quienes vienen de C (o algún lenguaje) y quieren aprender Python con fundamentos sólidos. Cada clase alterna teoría con ejemplos ejecutables en Jupyter Notebooks.

> **Estado:** El curso está en desarrollo. Por ahora solo está disponible la Clase 2, e iremos agregando más clases si es que se posee tiempo, no se promete nada.

## Clases

| Clase | Tema | Notebook |
|-------|------|----------|
| 2 | Tipos de Datos, Operadores y Modelo de Objetos | [`clases/clase_2.ipynb`](clases/clase_2.ipynb) |

## Requisitos

- Python 3.14 o superior
- [uv](https://docs.astral.sh/uv/) (gestor de proyectos y paquetes)

## Instalación

### 1. Instalar uv

Si aún no tienes `uv` instalado, sigue las instrucciones oficiales según tu sistema operativo:

- **Windows (PowerShell):**
  ```powershell
  powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
  ```
- **Linux/macOS:**
  ```bash
  curl -LsSf https://astral.sh/uv/install.sh | sh
  ```

También puedes instalarlo con pip: `pip install uv`, o con tu gestor de paquetes favorito (brew, winget, etc.). Más información en la [documentación oficial](https://docs.astral.sh/uv/#installation).

### 2. Clonar y preparar el entorno

```bash
# Clonar el repositorio
git clone <url-del-repo>
cd curso_takeishi

# Sincronizar dependencias (crea el .venv e instala Jupyter, ipykernel, etc.)
uv sync

# Iniciar Jupyter Notebook
uv run jupyter notebook
```

O desde VS Code: abre la carpeta, selecciona el kernel `.venv` en la pestaña de selección dentro del Jupyter Notebook y ejecuta las celdas.

> **Nota:** `uv sync` instala todo lo necesario según `pyproject.toml`. No es necesario activar el entorno manualmente — `uv run` lo maneja automáticamente.

## Material de referencia

Este curso se apoya en los siguientes recursos:

- **Corcuera, J. L.** — *Introducción a Python* (apuntes de cátedra)
- **MoureDev** — *Guía Junior 2026* (guía de conceptos fundamentales)
- **Bonaretti, S.** — *Learn Python with Jupyter* (libro práctico con notebooks); traducción al español por **Rodrigo Ernesto Álvarez Aguilera** ([incognia/Notebooks](https://github.com/incognia/Notebooks))
- **Parmar, M.** (milaan9) — [01_Python_Introduction](https://github.com/milaan9/01_Python_Introduction) (introducción completa a Python desde cero)
- **Basnet, R.** (rambasnet) — [Python-Fundamentals](https://github.com/rambasnet/Python-Fundamentals) (fundamentos y estructuras de datos, basado en *How to Think Like a Computer Scientist*)

