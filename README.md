# Curso Takeishi — Python desde Cero

Curso práctico de Python 3 pensado para quienes vienen de C (o algún lenguaje) y quieren aprender Python con fundamentos sólidos. Cada clase alterna teoría con ejemplos ejecutables en Jupyter Notebooks.

> **Estado:** 20 clases + 1 clase especial disponibles, organizadas según el plan [`plan_curso_python.md`](plan_curso_python.md). El curso cubre la Parte I (Fundamentos Esenciales) de la guía de MoureDev, agregando temas que rara vez se enseñan: POO, decoradores, Zen/PEPs, type hints y patrones de diseño.

## Clases

| Clase | Tema | Notebook |
|-------|------|----------|
| 1 | Introducción a Python y Entorno de Desarrollo | [`clases/clase_1.ipynb`](clases/clase_1.ipynb) |
| 2 | Sintaxis, `print()` y Modelo de Objetos | [`clases/clase_2.ipynb`](clases/clase_2.ipynb) |
| 3 | Palabras Reservadas y Punto de Entrada | [`clases/clase_3.ipynb`](clases/clase_3.ipynb) |
| 4 | Control de Flujo (`if`, `for`, `while`) | [`clases/clase_4.ipynb`](clases/clase_4.ipynb) |
| 5 | Funciones y Recursividad | [`clases/clase_5.ipynb`](clases/clase_5.ipynb) |
| 6 | Listas y Tuplas | [`clases/clase_6.ipynb`](clases/clase_6.ipynb) |
| 7 | Diccionarios y Sets | [`clases/clase_7.ipynb`](clases/clase_7.ipynb) |
| 8 | Strings en Profundidad | [`clases/clase_8.ipynb`](clases/clase_8.ipynb) |
| 9 | Pilas, Colas, Árboles y Grafos | [`clases/clase_9.ipynb`](clases/clase_9.ipynb) |
| 10 | Algoritmos y Complejidad (Big O) | [`clases/clase_10.ipynb`](clases/clase_10.ipynb) |
| 11 | Módulos y Paquetes | [`clases/clase_11.ipynb`](clases/clase_11.ipynb) |
| 12 | Archivos y Excepciones | [`clases/clase_12.ipynb`](clases/clase_12.ipynb) |
| 13 | POO Fundamental: Clases, Encapsulamiento, Composición | [`clases/clase_13.ipynb`](clases/clase_13.ipynb) |
| 14 | POO Avanzada: Herencia, Polimorfismo, Métodos Mágicos | [`clases/clase_14.ipynb`](clases/clase_14.ipynb) |
| 15 | El Zen de Python y PEPs | [`clases/clase_15.ipynb`](clases/clase_15.ipynb) |
| 16 | Type Hints y módulo `typing` | [`clases/clase_16.ipynb`](clases/clase_16.ipynb) |
| 17 | Programación Funcional | [`clases/clase_17.ipynb`](clases/clase_17.ipynb) |
| 18 | Decoradores, Generadores y Context Managers | [`clases/clase_18.ipynb`](clases/clase_18.ipynb) |
| 19 | Patrones de Diseño | [`clases/clase_19.ipynb`](clases/clase_19.ipynb) |
| 20 | Cierre: Regex, Async, Clean Code, IA | [`clases/clase_20.ipynb`](clases/clase_20.ipynb) |
| Especial | Funciones Integradas (Built-in) | [`clases/clase_builtins.ipynb`](clases/clase_builtins.ipynb) |

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

## Estructura del repositorio

```
curso_takeishi/
├── clases/                  # Notebooks de cada clase (1-20 + especial)
├── plan_curso_python.md     # Plan detallado de las 18 clases
├── pyproject.toml           # Configuración del proyecto (uv)
└── README.md                # Este archivo
```

## Material de referencia

Este curso se apoya en los siguientes recursos:

- **Corcuera, J. L.** — *Introducción a Python* (apuntes de cátedra, Universidad de Cantabria)
- **MoureDev** — *Guía Junior 2026* (guía de conceptos fundamentales, parte I: Fundamentos Esenciales)
- **Bonaretti, S.** — *Learn Python with Jupyter* (libro práctico con notebooks); traducción al español por **Rodrigo Ernesto Álvarez Aguilera** ([incognia/Notebooks](https://github.com/incognia/Notebooks))
- **Parmar, M.** (milaan9) — [01_Python_Introduction](https://github.com/milaan9/01_Python_Introduction) (introducción completa a Python desde cero)
- **Basnet, R.** (rambasnet) — [Python-Fundamentals](https://github.com/rambasnet/Python-Fundamentals) (fundamentos y estructuras de datos, basado en *How to Think Like a Computer Scientist*)
