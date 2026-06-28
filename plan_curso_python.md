# Plan del Curso de Python para Estudiantes de C

Este plan unifica la *Guía de programador Junior 2026* (MoureDev) y las presentaciones *Programación en Python* (Pedro Corcuera), adaptándose a universitarios que ya conocen C. Cada clase dura máximo 1 hora y 30 minutos y está diseñada para construir conocimiento de manera progresiva y práctica.

El curso tiene **20 clases** + **1 clase especial** que cubren la Parte I (Fundamentos Esenciales) de la guía de MoureDev, con énfasis en temas que rara vez se enseñan bien: POO, decoradores, generadores y patrones de diseño.

---

## Índice expandido de clases

Este índice funciona como un mapa expandido: cada clase tiene una descripción de una línea de su contenido real en el notebook, para que cualquiera pueda ver de un vistazo qué cubre cada sesión.

| # | Tema | Descripción de una línea | Notebook |
|---|---|---|---|
| 1 | Introducción y Entorno | Historia de Python, UV, Jupyter, primer Hola Mundo. | [`clase_1.ipynb`](clases/clase_1.ipynb) |
| 2 | Sintaxis y `print()` | Archivos `.py`, `if __name__`, `print()`, modelo de objetos, `id()`/`is`. | [`clase_2.ipynb`](clases/clase_2.ipynb) |
| 3 | Palabras Reservadas | Las 35 keywords, `import`/`from`/`as`, punto de entrada. | [`clase_3.ipynb`](clases/clase_3.ipynb) |
| 4 | Control de Flujo | `if`/`elif`/`else`, `for`, `while`, `break`/`continue`/`pass`, `and`/`or`/`not`. | [`clase_4.ipynb`](clases/clase_4.ipynb) |
| 5 | Funciones y Recursividad | `def`, `*args`/`**kwargs`, scope, lambdas, recursividad (factorial, Fibonacci). | [`clase_5.ipynb`](clases/clase_5.ipynb) |
| 6 | Listas y Tuplas | Creación, slicing, métodos, tuplas, desempaquetado, `zip()`. | [`clase_6.ipynb`](clases/clase_6.ipynb) |
| 7 | Diccionarios y Sets | Llave-valor, métodos, iteración, sets, `frozenset`, patrones de uso. | [`clase_7.ipynb`](clases/clase_7.ipynb) |
| 8 | Strings en Profundidad | Métodos, escape, inmutabilidad, formato (f-strings, `format`, `ord`/`chr`). | [`clase_8.ipynb`](clases/clase_8.ipynb) |
| 9 | Pilas, Colas, Árboles, Grafos | LIFO/FIFO, BST, BFS/DFS, implementación con listas/dicts. | [`clase_9.ipynb`](clases/clase_9.ipynb) |
| 10 | Algoritmos y Complejidad | Big O, búsqueda (lineal/binaria), ordenación (burbuja, quicksort), divide y vencerás. | [`clase_10.ipynb`](clases/clase_10.ipynb) |
| 11 | Módulos y Paquetes | `import`, paquetes, `pyproject.toml`, módulos estándar (`os`, `json`, `collections`). | [`clase_11.ipynb`](clases/clase_11.ipynb) |
| 12 | Archivos y Excepciones | `open()`, `with`, `try/except/finally`, `raise`, excepciones personalizadas. | [`clase_12.ipynb`](clases/clase_12.ipynb) |
| 13 | POO Fundamental | Clases, `__init__`, `self`, encapsulamiento, composición, dataclasses. | [`clase_13.ipynb`](clases/clase_13.ipynb) |
| 14 | POO Avanzada | Herencia, MRO, polimorfismo, ABC, métodos mágicos, `__slots__`. | [`clase_14.ipynb`](clases/clase_14.ipynb) |
| 15 | El Zen de Python y PEPs | Los 19 aforismos, PEP 8, PEP 20, PEP 257, cómo leer un PEP. | [`clase_15.ipynb`](clases/clase_15.ipynb) |
| 16 | Type Hints y módulo `typing` | Anotaciones de tipo, `Optional`, `Union`, `TypedDict`, `Protocol`, `mypy`. | [`clase_16.ipynb`](clases/clase_16.ipynb) |
| 17 | Programación Funcional | Funciones puras, `map`/`filter`/`reduce`, comprehensions, `functools`. | [`clase_17.ipynb`](clases/clase_17.ipynb) |
| 18 | Decoradores y Generadores | `@decorador`, `yield`, generadores, context managers, `contextlib`. | [`clase_18.ipynb`](clases/clase_18.ipynb) |
| 19 | Patrones de Diseño | Singleton, Factory, Observer, Strategy, Decorator (patrón). | [`clase_19.ipynb`](clases/clase_19.ipynb) |
| 20 | Cierre del Curso | Comprehensions, regex, async/await, Clean Code, IA. | [`clase_20.ipynb`](clases/clase_20.ipynb) |
| Especial | Funciones Integradas | Las 75 built-in functions de Python organizadas por categoría. | [`clase_builtins.ipynb`](clases/clase_builtins.ipynb) |

### Cómo está organizado cada plan de clase

Cada sección de clase sigue este formato:
- **Duración estimada:** tiempo aproximado (la mayoría son 90 min, la Clase 2 es más corta).
- **Recursos base:** fuentes bibliográficas utilizadas.
- **Notebook de apoyo:** ruta al notebook ejecutable.
- **Contenido:** lista de temas cubiertos.
- **Puente con C:** comparación explícita con C para universitarios.
- **Ejemplo de mini herramienta:** proyecto práctico de la clase.
- **Restricción del ejercicio:** qué no se permite usar (para forzar el aprendizaje).
- **Conexión:** (opcional) cómo se conecta con clases anteriores y siguientes.

---

### Clase 1 — Introducción a Python y Entorno de Desarrollo
**Duración estimada:** 90 minutos
**Recursos base:** sección "El desarrollador en 2026" y "Terminal/IDEs" del Recurso A + páginas 4-13 del Recurso B
**Notebook de apoyo:** `01_introduccion.ipynb`

**Contenido:**
- Historia de Python, creador del lenguaje (Guido van Rossum, 1991), influencia de ABC.
- Ventajas: sintaxis sencilla + librería estándar extensa.
- Desventajas: velocidad de ejecución + necesidad de gestores de paquetes externos.
- Alto nivel vs bajo nivel: dónde se ubica Python.
- Instalación de UV y gestión de paquetes moderna (Recurso A).
- Entornos de desarrollo, IDEs y uso básico de terminal.
- Características de alto nivel e interpretación del lenguaje.
- Herramientas de IA como asistente de aprendizaje.

**Puente con C:**
A diferencia de C, que es compilado directamente a código máquina y requiere gestión de memoria manual, Python es un lenguaje interpretado de muy alto nivel donde el entorno de ejecución se encarga de la recolección de basura.

**Ejemplo de mini herramienta:**
Script "Hola Mundo IA", una herramienta sencilla de línea de comandos que imprime un mensaje de bienvenida y la versión del sistema, ejercitando la ejecución básica de un script.

**Restricción del ejercicio:**
El alumno no puede usar variables, bucles, ni funciones definidas por el usuario aún, solo ejecución secuencial de `print()` e imports básicos de sistema.

---

### Clase 2 — Sintaxis, `print()` y Modelo de Objetos
**Duración estimada:** 60-70 minutos (clase más corta, intencionalmente introductoria)
**Recursos base:** páginas 4-13 y 14-30 del Recurso B
**Notebook de apoyo:** `clases/clase_2.ipynb`

**Nota sobre la duración:** Esta clase es intencionalmente más corta que las demás. Sirve como puente entre la Clase 1 (introducción) y la Clase 4 (control de flujo), cubriendo los 3 pilares fundacionales que todo lo demás necesita: cómo es un archivo `.py`, cómo mostrar información, y cómo funciona el modelo de objetos en memoria. Los temas más densos (tipos, operadores, keywords) se cubren en clases posteriores con más profundidad.

**Contenido:**
- Extensión de archivos `.py` y convención `if __name__ == '__main__':`.
- Función `print()` en profundidad: `sep`, `end`, formato, redirección.
- Tipado dinámico: las variables son referencias, no contenedores.
- **Identidad de objetos:** `id()` y el operador `is` (referencia a Corcuera, IntroPython).
- Regla de oro: `==` para valores, `is` para identidad (usar solo con `None`, `True`, `False`).

**Puente con C:**
En C el código se compila y el punto de entrada es siempre `main()`. En Python, la convención `if __name__ == '__main__':` cumple un rol similar. Además, en C las variables "contienen" valores; en Python, las variables son **referencias** (punteros) a objetos en memoria.

**Ejemplo de mini herramienta:**
Script modular con un `main()` y un punto de entrada, demostrando la diferencia entre ejecutar un archivo directamente e importarlo como módulo.

**Restricción del ejercicio:**
Sin restricción estricta, pero se enfoca en entender los conceptos antes de avanzar a tipos y operadores (que se cubren en clases posteriores).

**Conexión con clases anteriores y siguientes:**
- **Viene de Clase 1:** El Hola Mundo que escribiste en Clase 1 se profundiza aquí con todos los parámetros de `print()`.
- **Va hacia Clase 3:** Ahora que entiendes cómo se estructura un script, aprenderás las 35 palabras reservadas que le dan estructura al lenguaje.

---

### Clase 3 — Palabras Reservadas y Punto de Entrada
**Duración estimada:** 90 minutos
**Recursos base:** páginas 15-16 del Recurso B
**Notebook de apoyo:** `03_keywords.ipynb`

**Contenido:**
- Las 35 palabras reservadas de Python organizadas por categoría.
- El operador asignación (`=`) y sus variantes (múltiple, en cadena, `del`).
- `import`, `from ... import`, `as`: cómo se importan módulos.
- Punto de entrada: `if __name__ == '__main__':` y la variable `__name__`.
- Diferencia entre ejecutar un archivo directamente e importarlo.

**Puente con C:**
En C el punto de entrada es siempre `main()`. En Python, el código se ejecuta de arriba a abajo, pero la convención `if __name__ == '__main__':` permite controlar qué código se ejecuta solo cuando el archivo es el programa principal.

**Ejemplo de mini herramienta:**
Script modular con un archivo `utilidades.py` que se importa desde un script principal, demostrando cuándo se ejecuta el código de cada archivo.

**Restricción del ejercicio:**
Solo se pueden usar palabras reservadas con su propósito; no se permite redefinir keywords ni crear variables con nombres reservados.

---

### Clase 4 — Control de Flujo
**Duración estimada:** 90 minutos
**Recursos base:** sección "Estructuras de Control" del Recurso A + páginas 66-94 del Recurso B
**Notebook de apoyo:** `04_control_flujo.ipynb`

**Contenido:**
- Condicionales: `if`, `elif`, `else` y operadores de comparación encadenados.
- Bucles definidos: `for-in` y `range()`, `enumerate()`, `zip()`, `reversed()`.
- Bucles indefinidos: `while` con condición de parada.
- Control de bucles: `break`, `continue`, `pass`.
- Operadores `in` y `not in` para membresía en secuencias.
- Operadores lógicos: `and`, `or`, `not` para combinar condiciones.
- Cortocircuito en evaluación de expresiones lógicas.

**Puente con C:**
El bucle `for` en Python funciona como un `foreach` iterando sobre secuencias, en contraste con la estructura clásica `for(int i=0; i<N; i++)` de C; para simular esta última se utiliza la función generadora `range()`.

**Ejemplo de mini herramienta:**
Validador de contraseñas seguras, que solicita una cadena y mediante bucles y condicionales cuenta mayúsculas, números y longitud, e informa si cumple criterios de seguridad.

**Restricción del ejercicio:**
No se pueden usar expresiones regulares (`re`) ni métodos de validación avanzados de strings.

---

### Clase 5 — Funciones y Recursividad
**Duración estimada:** 90 minutos
**Recursos base:** sección "Funciones" del Recurso A + páginas 126-151 del Recurso B
**Notebook de apoyo:** `05_funciones.ipynb`

**Contenido:**
- Definición de funciones con `def`, parámetros posicionales vs nominales.
- Valores de retorno múltiples (empaquetados en tuplas).
- Número variable de argumentos: `*args` y `**kwargs`.
- Espacio de nombres (Scope) y variables locales vs globales.
- Funciones como ciudadanos de primera clase (asignar a variables, pasar como argumentos).
- Funciones anónimas: `lambda`.
- **Recursividad:** caso base y caso recursivo, factorial, Fibonacci, Torres de Hanoi.

**Puente con C:**
En Python no hay declaración de firmas de funciones en archivos "header" (`.h`); además, las funciones pueden anidarse y ser pasadas como argumentos (Callbacks) de manera mucho más natural que usando punteros a función en C.

**Ejemplo de mini herramienta:**
Librería de utilidades matemáticas con funciones para factorial, Fibonacci, y cálculo de distancia euclidiana, usando `*args` para argumentos variables.

**Restricción del ejercicio:**
No se permite el uso de `numpy` o similares; todas las operaciones deben implementarse con bucles nativos y el módulo `math`.

---

### Clase 6 — Listas y Tuplas
**Duración estimada:** 90 minutos
**Recursos base:** sección "Estructuras Lineales" del Recurso A + páginas 52-55 y 95-104 del Recurso B
**Notebook de apoyo:** `06_listas_tuplas.ipynb`

**Contenido:**
- Listas: creación, indexado, mutabilidad.
- Operaciones con listas: `append`, `insert`, `pop`, `remove`, `extend`, `clear`, `sort`, `reverse`.
- Slicing: extracción de sub-listas con `[inicio:fin:paso]`.
- Tuplas: sintaxis, inmutabilidad, desempaquetado, retorno múltiple.
- Listas de listas: matrices y arrays multidimensionales.
- Diferencias clave entre listas y tuplas (mutabilidad, rendimiento, uso como claves de dict).
- `zip()` para combinar listas paralelas.

**Puente con C:**
Las listas de Python son estructuras dinámicas (arrays redimensionables subyacentes), no necesitan declarar tamaño inicial ni usar `malloc()` o `realloc()` como los arrays estáticos o dinámicos de C.

**Ejemplo de mini herramienta:**
Organizador de tareas por prioridad (pila/cola). Usa una lista para ingresar tareas pendientes y despachar tareas usando `pop()` para simular colas de procesamiento.

**Restricción del ejercicio:**
No se pueden utilizar diccionarios para vincular tareas con atributos adicionales.

---

### Clase 7 — Diccionarios y Sets
**Duración estimada:** 90 minutos
**Recursos base:** sección "Estructuras Asociativas" del Recurso A + páginas 56-64 del Recurso B
**Notebook de apoyo:** `07_diccionarios_sets.ipynb`

**Contenido:**
- Diccionarios: concepto de llave-valor, mutabilidad, indexación por llaves.
- Funciones de diccionarios: `keys()`, `values()`, `items()`, `get()`, `update()`, `pop()`.
- Iteración sobre diccionarios: por claves, valores o pares.
- Conjuntos (`set`): elementos únicos, operaciones de unión (`|`), intersección (`&`), diferencia (`-`).
- `frozenset`: versión inmutable de set.
- Estructuras complejas: listas de diccionarios, diccionarios anidados.
- Patrones de uso: contadores con `.get()`, agrupación de datos.

**Puente con C:**
Los diccionarios en Python son tablas hash (Hash Tables) altamente optimizadas que vienen implementadas de forma nativa, reemplazando la necesidad de programar manualmente punteros, funciones de hash y resolución de colisiones en C.

**Ejemplo de mini herramienta:**
Directorio de contactos para proyectos grupales. La llave es la matrícula del alumno y el valor es un diccionario con su nombre, correo y rol, permitiendo buscar información en complejidad O(1).

**Restricción del ejercicio:**
Aún no se pueden crear clases (`class`); toda la estructura debe depender exclusivamente de diccionarios anidados.

---

### Clase 8 — Strings en Profundidad
**Duración estimada:** 90 minutos
**Recursos base:** páginas 56-67 del Recurso B
**Notebook de apoyo:** `08_strings.ipynb` (existe como `clase_5.ipynb`)

**Contenido:**
- Creación de strings: comillas simples, dobles, triples para multilínea.
- Secuencias de escape: `\n`, `\t`, `\\`, `\'`, `\"`.
- Inmutabilidad de strings y por qué es importante.
- Indexado y slicing de strings.
- Operadores: `+` (concatenación), `*` (repetición), `in` (membresía).
- Métodos de strings: `upper`, `lower`, `strip`, `split`, `join`, `replace`, `find`, `count`, `startswith`, `endswith`.
- Formato: f-strings, `str.format()`, operador `%`.
- `ord()` y `chr()` para conversión carácter-ordinal.
- `r` strings (raw strings) para evitar escapes.

**Puente con C:**
En C, las cadenas son `char[]` mutables terminados en `'\0'`. En Python, los strings son objetos inmutables de la clase `str` con soporte Unicode completo.

**Ejemplo de mini herramienta:**
Procesador de texto que limpia, normaliza y formatea datos de entrada (correos, nombres, números de teléfono) usando métodos de strings.

**Restricción del ejercicio:**
No se pueden usar expresiones regulares (`re`); solo métodos estándar de strings.

---

### Clase 9 — Pilas, Colas, Árboles y Grafos
**Duración estimada:** 90 minutos
**Recursos base:** sección "Estructuras de Datos" del Recurso A
**Notebook de apoyo:** `09_estructuras_datos.ipynb`

**Contenido:**
- **Pilas (Stacks):** LIFO, operaciones push/pop/peek, implementación con listas.
- **Colas (Queues):** FIFO, operaciones enqueue/dequeue, `collections.deque`.
- **Colas de prioridad:** `heapq` para montículos binarios.
- **Árboles:** nodos, raíz, hijos, recorrido preorden/inorden/postorden.
- **Árboles binarios de búsqueda:** inserción, búsqueda en O(log n) promedio.
- **Grafos:** nodos y aristas, dirigidos vs no dirigidos, representación con diccionarios.
- **Recorridos de grafos:** BFS (amplitud) y DFS (profundidad).

**Puente con C:**
En C, todas estas estructuras se implementan manualmente con punteros y `malloc()`. En Python, las listas y diccionarios son tan versátiles que se pueden usar como base para casi cualquier estructura, y el módulo `collections` proporciona implementaciones optimizadas.

**Ejemplo de mini herramienta:**
Sistema de navegación de un mapa (grafo de ciudades) usando BFS para encontrar la ruta más corta entre dos puntos.

**Restricción del ejercicio:**
Implementar las estructuras desde cero usando listas y diccionarios; no usar librerías externas.

---

### Clase 10 — Algoritmos y Complejidad
**Duración estimada:** 90 minutos
**Recursos base:** sección "Algoritmos y Complejidad" del Recurso A
**Notebook de apoyo:** `10_algoritmos.ipynb`

**Contenido:**
- **Notación Big O:** O(1), O(log n), O(n), O(n log n), O(n²), O(2ⁿ).
- **Algoritmos de búsqueda:** lineal O(n), binaria O(log n) (requiere datos ordenados), hash O(1).
- **Algoritmos de ordenación:** burbuja O(n²), inserción O(n²), selección O(n²), quicksort O(n log n), mergesort O(n log n).
- **Técnicas algorítmicas:** divide y vencerás, algoritmos voraces (greedy), backtracking, dos punteros.
- **Análisis empírico:** medir tiempo de ejecución con `time`.

**Puente con C:**
En C, implementar estos algoritmos requiere gestión manual de memoria. En Python, el enfoque se centra en la lógica del algoritmo y el análisis de complejidad, dejando la optimización de bajo nivel a las bibliotecas estándar.

**Ejemplo de mini herramienta:**
Comparador de algoritmos de ordenación que mide el tiempo de ejecución de cada uno con diferentes tamaños de entrada y muestra los resultados en una tabla.

**Restricción del ejercicio:**
No usar `sorted()` ni `list.sort()` de Python; implementar los algoritmos manualmente para entender la lógica.

---

### Clase 11 — Módulos y Paquetes
**Duración estimada:** 90 minutos
**Recursos base:** sección "Modularidad y Gestión de Dependencias" del Recurso A
**Notebook de apoyo:** `11_modulos.ipynb`

**Contenido:**
- Módulos: qué son, cómo se crean (archivos `.py`).
- Importación: `import`, `from ... import`, `as`.
- Namespace y encapsulamiento: `__all__`, `_privado`, `__dunder__`.
- Paquetes: directorios con `__init__.py`.
- Gestión de dependencias con UV: `pyproject.toml`, `uv.lock`.
- Búsqueda de módulos: `sys.path`, `PYTHONPATH`.
- Módulos de la biblioteca estándar: `os`, `sys`, `math`, `random`, `datetime`, `json`, `collections`.

**Puente con C:**
En C, la modularidad se logra con archivos de cabecera (`.h`) y compilación separada con `gcc`. En Python, los módulos son archivos `.py` que se importan en tiempo de ejecución, sin necesidad de compilación previa.

**Ejemplo de mini herramienta:**
Crear un paquete `mi_libreria` con múltiples módulos (`estadisticas.py`, `geometria.py`, `cadenas.py`) y un script cliente que los use.

**Restricción del ejercicio:**
No usar paquetes externos (numpy, pandas); solo módulos de la biblioteca estándar.

---

### Clase 12 — Archivos y Excepciones
**Duración estimada:** 90 minutos
**Recursos base:** sección "Manejo de Errores" del Recurso A + páginas 105-116 y 179-191 del Recurso B
**Notebook de apoyo:** `12_archivos_excepciones.ipynb`

**Contenido:**
- Interacción con sistema operativo: `os.path`, `os.listdir`, `sys.argv` (argumentos CLI).
- Apertura de archivos: `open()` con modos `r`, `w`, `a`, `rb`, `wb`.
- Lectura: `read()`, `readline()`, `readlines()`, iteración directa.
- Escritura: `write()`, `writelines()`.
- Administradores de contexto: `with open(...) as f:` para cierre automático.
- Excepciones: jerarquía de errores, bloques `try-except-else-finally`.
- Lanzamiento de errores: `raise`, `raise ... from ...`.
- Filosofía "Fail Fast" y patrón Guard Clauses.
- Creación de excepciones personalizadas heredando de `Exception`.

**Puente con C:**
El uso de `with open(archivo) as f:` en Python garantiza el cierre automático del descriptor de archivo, eliminando la necesidad de recordar invocar `fclose(f)` o verificar los punteros nulos de `fopen()`. En C, los errores se manejan con valores de retorno; en Python, con excepciones.

**Ejemplo de mini herramienta:**
Procesador de logs (archivos `.txt`). Un script que recibe por línea de comandos el nombre de un archivo de log, intenta abrirlo, extrae mensajes de error manejando excepciones, y guarda un reporte filtrado en un archivo nuevo.

**Restricción del ejercicio:**
Todo el parseo de texto debe hacerse con métodos estándar de strings (`split`, `strip`), sin expresiones regulares ni POO.

---

### Clase 13 — POO Fundamental: Clases, Encapsulamiento, Composición
**Duración estimada:** 90 minutos
**Recursos base:** sección "Programación Orientada a Objetos" del Recurso A + páginas 209-217 del Recurso B
**Notebook de apoyo:** `13_poo_fundamentos.ipynb`

**Contenido:**
- Paradigma POO: clases vs. instancias (objetos).
- Sintaxis de clases: `class`, método constructor `__init__`, parámetro `self`.
- Atributos de instancia y atributos de clase.
- Métodos de instancia, métodos estáticos (`@staticmethod`) y métodos de clase (`@classmethod`).
- Propiedades (`@property`) para encapsular getters/setters.
- Encapsulamiento: convenciones `_privado`, `__name_mangling`.
- Composición: "tiene un" vs "es un".
- Dataclasses: `@dataclass` para clases de datos concisas.
- Métodos mágicos básicos: `__str__`, `__repr__`, `__eq__`.

**Puente con C:**
Una clase puede entenderse inicialmente como un `struct` de C (que agrupa datos) pero que a su vez contiene la definición interna de las funciones (métodos) exclusivas para manipular esos datos.

**Ejemplo de mini herramienta:**
Gestor de Estudiantes. Clase `Estudiante` que almacena matrícula, nombre y notas. Contiene métodos para añadir calificaciones y calcular el promedio, encapsulando la lógica que antes estaba dispersa en diccionarios y listas.

**Restricción del ejercicio:**
No se usarán aún características avanzadas como herencia de otras clases o sobrecarga de operadores complejos.

---

### Clase 14 — POO Avanzada: Herencia, Polimorfismo y Métodos Mágicos
**Duración estimada:** 90 minutos
**Recursos base:** sección "Programación Orientada a Objetos" del Recurso A + páginas 218-237 del Recurso B
**Notebook de apoyo:** `14_poo_avanzada.ipynb`

**Contenido:**
- Herencia: reutilización de comportamiento, `super().__init__()`.
- Herencia múltiple y MRO (Method Resolution Order).
- Polimorfismo: sobreescritura de métodos, duck typing.
- Métodos mágicos (dunder): `__str__`, `__repr__`, `__len__`, `__eq__`, `__lt__`, `__add__`, `__iter__`, `__next__`.
- Sobrecarga de operadores aritméticos.
- Clases abstractas (ABC): `abc.ABC`, `@abstractmethod`.
- Composición vs Herencia: cuándo usar cada una.
- `__slots__` para optimizar memoria.

**Puente con C:**
La herencia y el polimorfismo no tienen un equivalente directo sintáctico en C puro (solo implementable manualmente mediante punteros a funciones en structs y castings); Python lo hace de manera nativa e intuitiva.

**Ejemplo de mini herramienta:**
Librería para el manejo de vectores o números complejos. Clase `Vector` que sobrescribe los métodos `__add__` y `__str__` para poder sumar matemáticamente instancias como `v3 = v1 + v2`.

**Restricción del ejercicio:**
El diseño debe seguir el principio de responsabilidad única, pero no se exigirán patrones de diseño arquitectónicos complejos.

---

### Clase 15 — El Zen de Python y PEPs Importantes
**Duración estimada:** 90 minutos
**Recursos base:** PEPs oficiales ([peps.python.org](https://peps.python.org/)) + documentación de Python
**Notebook de apoyo:** `clases/clase_15.ipynb`

**Nota sobre esta clase:** Rara vez se enseña en cursos introductorios, pero marca la diferencia entre código que funciona y código "pitónico" de calidad.

**Contenido:**
- El Zen de Python (PEP 20): los 19 aforismos explicados con ejemplos.
- ¿Qué es un PEP? El proceso de propuesta, discusión y aceptación.
- PEP 8: Style Guide for Python Code (resumen de reglas principales).
- PEP 257: Docstring Conventions (estilos Google, NumPy, Sphinx).
- Otros PEPs importantes: PEP 1, PEP 328, PEP 484, PEP 572.
- Cómo leer un PEP: abstract, motivation, specification.
- Ejercicio: refactorizar código aplicando el Zen.

**Puente con C:**
En C no existe una "guía de estilo" oficial comparable a PEP 8. Python tiene una filosofía explícita ("The Zen") y documentos formales (PEPs) que guían la evolución del lenguaje. Seguir PEP 8 es como seguir las convenciones de `K&R` o `Linux kernel style` en C, pero con autoridad oficial.

**Ejemplo de mini herramienta:**
Refactorizar un código que viola el Zen y PEP 8 (variables mal nombradas, funciones largas, anidamiento excesivo) a una versión limpia usando nombres descriptivos, guard clauses, y docstrings.

**Restricción del ejercicio:**
No usar `Any` en type hints (degrada la verificación). Todas las funciones deben tener type hints completos, docstrings estilo Google, y seguir PEP 8.

---

### Clase 16 — Type Hints y el Módulo `typing`
**Duración estimada:** 90 minutos
**Recursos base:** PEP 484, PEP 585, documentación de `typing`
**Notebook de apoyo:** `clases/clase_16.ipynb`

**Nota sobre esta clase:** Los type hints son una de las adiciones más importantes de Python moderno. Permiten detectar errores antes de ejecutar y mejorar el autocompletado.

**Contenido:**
- ¿Qué son los type hints? Anotaciones opcionales para documentar tipos.
- Sintaxis básica: `: tipo` para variables, `-> tipo` para retornos.
- Tipos compuestos: `List[T]`, `Dict[K, V]`, `Tuple`, `Set` (o built-ins en Python 3.9+).
- `Optional[X]`, `Union[X, Y]`, y la sintaxis moderna `X | Y` (Python 3.10+).
- `Callable`, `Iterator`, `Generator` para funciones y objetos iterables.
- `Any`, `NoReturn`, `Never` para casos especiales.
- `TypedDict` para diccionarios con schema, `Protocol` para duck typing estático.
- `TypeAlias` y `NewType` para tipos derivados.
- `mypy`: verificación estática de tipos.
- Ejercicio: sistema de calificaciones con type hints completos.

**Puente con C:**
En C, los tipos se declaran explícitamente en cada variable (`int x`). En Python, son implícitos pero opcionales. Los type hints añaden la opción de verificación estática sin sacrificar la flexibilidad dinámica. Es como tener un compilador que verifica tipos **antes** de ejecutar, similar a cómo un IDE de C puede detectar errores antes de compilar.

**Ejemplo de mini herramienta:**
Sistema de calificaciones con `TypedDict Estudiante`, `NewType Matricula`, type hints completos, docstrings estilo Google, y verificación con `mypy`.

**Restricción del ejercicio:**
No usar `Any` (degrada la verificación). Todas las funciones deben tener type hints completos y seguir PEP 8.

---

### Clase 17 — Programación Funcional
**Duración estimada:** 90 minutos
**Recursos base:** sección "Programación Funcional" del Recurso A
**Notebook de apoyo:** `clases/clase_17.ipynb`

**Contenido:**
- Funciones puras: misma entrada = misma salida, sin efectos secundarios.
- Inmutabilidad: por qué importa y cómo lograrla.
- Funciones de orden superior: funciones que reciben o retornan funciones.
- `map()`: aplicar una función a cada elemento de un iterable.
- `filter()`: filtrar elementos según un predicado.
- `reduce()`: acumular valores (de `functools`).
- Comprehensions: list, dict, set comprehensions.
- Generator expressions: `(x for x in ...)`.
- Closures y lambdas como funciones de orden superior.
- `functools.partial`, `functools.lru_cache`.

**Puente con C:**
La POO organiza el código alrededor de objetos con estado; la programación funcional lo organiza alrededor de transformaciones de datos sin estado. En C, simular esto requiere disciplina manual; en Python, las funciones de primera clase lo hacen natural.

**Ejemplo de mini herramienta:**
Pipeline de procesamiento de datos: leer lista de números → filtrar pares → elevar al cuadrado → calcular suma, todo usando `map`, `filter`, `reduce` y lambdas.

**Restricción del ejercicio:**
Evitar mutaciones de variables; preferir expresiones que retornan nuevos valores.

---

### Clase 18 — Decoradores, Generadores y Context Managers
**Duración estimada:** 90 minutos
**Recursos base:** sección "Programación Funcional" del Recurso A
**Notebook de apoyo:** `clases/clase_18.ipynb`

**Contenido:**
- Funciones como objetos: asignar a variables, pasar como argumentos, retornar funciones.
- Closures: funciones que capturan variables del scope externo.
- **Decoradores:** funciones que envuelven otras funciones para extender su comportamiento.
- Decoradores con argumentos (decorador de tres niveles).
- `functools.wraps` para preservar metadata.
- Decoradores de clase: `@staticmethod`, `@classmethod`, `@property`.
- **Generadores:** funciones con `yield`, evaluación perezosa.
- Expresiones generadoras: `(x for x in iterable)`.
- Protocolo de iteración: `__iter__`, `__next__`.
- **Context managers:** protocolo `__enter__`/`__exit__`.
- `contextlib.contextmanager` para crear context managers con generadores.

**Puente con C:**
Los decoradores son syntactic sugar para funciones de orden superior. En C, el equivalente serían los punteros a función pasados como callbacks, pero sin la sintaxis elegante de `@decorator`.

**Ejemplo de mini herramienta:**
Decorador `@timer` que mide el tiempo de ejecución de cualquier función, `@retry` que reintenta una función N veces si falla, y context manager para medir tiempo de bloques de código.

**Restricción del ejercicio:**
Implementar todo desde cero; no usar librerías externas de decoradores.

---

### Clase 19 — Patrones de Diseño
**Duración estimada:** 90 minutos
**Recursos base:** sección "Patrones de Diseño" del Recurso A
**Notebook de apoyo:** `clases/clase_19.ipynb`

**Contenido:**
- ¿Qué son los patrones de diseño? Soluciones reutilizables a problemas recurrentes.
- **Singleton:** una sola instancia de una clase.
- **Factory:** creación de objetos sin especificar la clase exacta.
- **Observer:** notificación de cambios a múltiples objetos (eventos).
- **Strategy:** selección de algoritmo en tiempo de ejecución.
- **Decorator (patrón):** añadir funcionalidad sin modificar la clase (distinto del syntactic sugar de Python).
- Cuándo usar cada patrón y cuándo evitarlos.
- Anti-patrones comunes.

**Puente con C:**
Los patrones de diseño son soluciones conceptuales que se pueden implementar en cualquier lenguaje. Python tiene soporte de primera clase para muchos de ellos (funciones de orden superior, decoradores), lo que reduce el código boilerplate comparado con C++/Java.

**Ejemplo de mini herramienta:**
Sistema de notificaciones con patrón Observer: múltiples suscriptores reciben actualizaciones cuando cambia el estado de un objeto (por ejemplo, un sensor de temperatura notifica a un display, un logger y una alarma).

**Restricción del ejercicio:**
No usar frameworks de inyección de dependencias; implementar los patrones desde cero con clases y funciones.

---

### Clase 20 — Cierre del Curso: Comprehensions, Regex, Async y Herramientas Modernas
**Duración estimada:** 90 minutos
**Recursos base:** secciones "Asincronía", "Regex" e "IA" del Recurso A
**Notebook de apoyo:** `clases/clase_20.ipynb`

**Contenido:**
- List Comprehensions: `[expr for item in iterable if condition]`.
- Dict Comprehensions: `{key: value for item in iterable}`.
- Set Comprehensions: `{expr for item in iterable}`.
- Expresiones Regulares (Regex) básicas: `re.match`, `re.search`, `re.findall`, `re.sub`.
- Patrones comunes: `\d`, `\w`, `\s`, `[a-z]`, `^`, `$`, `*`, `+`, `?`, `{n,m}`.
- Grupos y captura: `(...)`, `(?P<name>...)`.
- Asincronía: `async def`, `await`, `asyncio.run()`.
- `asyncio.gather()` para ejecutar corrutinas en paralelo.
- Principios de diseño: Clean Code, refactoring, nombres descriptivos.
- Herramientas de IA: uso de MCP, RAG, y creación del archivo `AGENTS.md`.
- Proyecto integrador final.

**Puente con C:**
Las List Comprehensions proveen una forma declarativa de generar arreglos filtrados en una sola línea, abstrayendo por completo el anidamiento de bucles `for` y `if` requeridos en C.

**Ejemplo de mini herramienta:**
Script "Scraper Inteligente". Utiliza regex para extraer correos electrónicos de un bloque de texto, list comprehensions para filtrar y transformar los resultados rápidamente, e incluye un `AGENTS.md` configurado con reglas para el proyecto.

**Restricción del ejercicio:**
Las peticiones de red asíncronas completas no son mandatorias, pero se espera el diseño concurrente simulado o la limpieza de datos avanzada en crudo.

---

## Tabla de progresión

| Clase | Tema central | Recurso dominante | Mini herramienta |
|---|---|---|---|
| 1 | Introducción y Entorno | Ambos | Hola Mundo IA |
| 2 | Sintaxis, `print()`, Modelo de Objetos | Ambos | Script modular con `main()` |
| 3 | Keywords y Punto de Entrada | Recurso B | Script modular |
| 4 | Control de Flujo | Recurso B | Validador de contraseñas |
| 5 | Funciones y Recursividad | Ambos | Librería matemática |
| 6 | Listas y Tuplas | Recurso B | Organizador de tareas |
| 7 | Diccionarios y Sets | Recurso B | Directorio de contactos |
| 8 | Strings en Profundidad | Recurso B | Procesador de texto |
| 9 | Pilas, Colas, Árboles, Grafos | Recurso A | Navegación de mapa |
| 10 | Algoritmos y Complejidad | Recurso A | Comparador de ordenación |
| 11 | Módulos y Paquetes | Ambos | Paquete mi_libreria |
| 12 | Archivos y Excepciones | Ambos | Procesador de logs |
| 13 | POO Fundamental | Recurso B | Gestor de Estudiantes |
| 14 | POO Avanzada | Recurso B | Librería de Vectores |
| 15 | El Zen de Python y PEPs | PEPs oficiales | Refactorización de código |
| 16 | Type Hints y módulo `typing` | PEP 484, `mypy` | Sistema de calificaciones tipado |
| 17 | Programación Funcional | Recurso A | Pipeline de datos |
| 18 | Decoradores y Generadores | Recurso A | Decorador timer/retry |
| 19 | Patrones de Diseño | Recurso A | Sistema de notificaciones |
| 20 | Cierre: Regex, Async, IA | Recurso A | Scraper Inteligente |
| Especial | Funciones Integradas (built-in) | Doc. oficial | Procesador con `sum()`, `sorted()`, etc. |

---

## Curso especial (este semestre)

Para el semestre actual, se cubrirán 9 clases (las marcadas con prioridad alta):

| # | Clase | Estado |
|---|---|---|
| 1 | Introducción | Presencial (existente) |
| 2 | Tipos y Operadores | ✅ Hecha |
| 4 | Control de Flujo | ❌ Por hacer |
| 5 | Funciones y Recursividad | ❌ Por hacer |
| 12 | Archivos y Excepciones | ❌ Por hacer |
| 13 | POO Fundamental | ❌ Por hacer |
| 14 | POO Avanzada | ❌ Por hacer |
| 18 | Decoradores y Generadores | ❌ Por hacer |
| 19 | Patrones de Diseño | ❌ Por hacer |

---

### Clase Especial — Funciones Integradas de Python (Built-in Functions)
**Duración estimada:** 60-75 minutos (clase complementaria, no obligatoria en el flujo principal)
**Recursos base:** documentación oficial de Python ([docs.python.org/3/library/functions](https://docs.python.org/3/library/functions.html))
**Notebook de apoyo:** `clases/clase_builtins.ipynb`

**Nota sobre esta clase:** No es una de las 18 clases numeradas. Es una clase complementaria que se creó para cubrir un tema que no tiene un lugar natural en la secuencia: las 75 funciones integradas de Python. Sirve como referencia y se puede estudiar en cualquier momento después de la Clase 2 (donde se introducen `print()`, `type()`, `id()` y `len()`).

**Contenido:**
- ¿Qué son las funciones integradas? (~75 funciones siempre disponibles).
- Cómo descubrirlas: `dir(builtins)`, `help()`, `builtins.__doc__`.
- Conversión de tipos: `int()`, `float()`, `str()`, `bool()`, `list()`, `dict()`, `set()`, `bin()`, `hex()`.
- Numéricas y matemáticas: `abs()`, `round()`, `pow()`, `sum()`, `min()`, `max()`, `divmod()`.
- Secuencias e iteración: `len()`, `range()`, `enumerate()`, `zip()`, `map()`, `filter()`, `sorted()`, `reversed()`, `all()`, `any()`.
- Entrada/Salida: `print()`, `input()`, `open()`, `format()`, `repr()`, `chr()`, `ord()`.
- Introspección: `type()`, `isinstance()`, `dir()`, `callable()`, `hasattr()`, `getattr()`, `setattr()`, `id()`, `hash()`.
- Funciones y clases: `staticmethod`, `classmethod`, `property`, `super`, `type` (como metaclass).
- Ejecución dinámica: `eval()`, `exec()`, `compile()` (con advertencias de seguridad).
- Tabla resumen de las 15 funciones más usadas con su frecuencia.
- Ejercicio práctico: procesador de calificaciones usando 10+ funciones integradas.

**Ejemplo de mini herramienta:**
Procesador de calificaciones que usa `sum()`, `len()`, `min()`, `max()`, `sorted()`, `enumerate()`, `zip()`, `filter()`, `round()`, `dict()` para calcular promedios, encontrar mejor/peor estudiante, contar aprobados y generar un reporte.

**Restricción del ejercicio:**
Solo se pueden usar funciones integradas (no se permite `import` de módulos como `statistics` o `numpy`).

---

## Notas de articulación

1. **Equilibrio Conceptual vs Sintáctico:** El "Recurso A" (Guía Junior MoureDev) aborda conceptos teóricos e ingeniería de software, mientras que el "Recurso B" (IntroPython) es estrictamente técnico-sintáctico. La articulación ideal usa el Recurso B para la sintaxis de las clases y el Recurso A como filosofía guía.

2. **Profundización en Estructuras de Datos:** El Recurso A enfatiza la importancia algorítmica y la complejidad (Big O), mientras que el Recurso B enseña la sintaxis de Listas/Diccionarios en Python. Las clases 9 y 10 complementan la sintaxis de B con las advertencias de rendimiento de A.

3. **Manejo de Asincronía:** El Recurso B carece de asincronía, pero el Recurso A destaca fuertemente `async/await`. La clase 18 introduce el concepto teóricamente basado en A.

4. **Enfoque de POO:** El Recurso A recomienda "Composición sobre Herencia". La clase 13 enseña composición primero; la clase 14 introduce herencia pero advierte sobre sus problemas en diseños grandes.

5. **Testing y Buenas Prácticas:** El Recurso A pone el "Manejo de Errores" y el "Testing" como herramientas imprescindibles. La clase 12 adelanta el enfoque de "Fail Fast" y "Guard Clauses".

6. **Estrategia de implementación:** Se priorizan las clases con notebooks de ejemplo existentes. Las clases 9, 10, 15, 16, 17 requieren investigación adicional para crear contenido desde cero. Los libros de Python que se agreguen después se usarán para enriquecer ejercicios y ejemplos adicionales.
