# 🎓 Sistema de Gestión de Estudiantes — ITB

Este es un sistema de escritorio clásico **CRUD** (Crear, Leer, Actualizar, Eliminar) diseñado en **Python**. Utiliza una interfaz gráfica amigable construida con **Tkinter** y gestiona la persistencia de datos de forma local mediante **SQLite3**.

El sistema permite administrar de manera ágil el registro de alumnos, sus carreras y sus calificaciones académicas.

---

## 🚀 Características

* **Persistencia Local:** Base de datos ligera e integrada con `SQLite3` (no requiere instalaciones de servidores externos).
* **Interfaz Gráfica (GUI):** Ventana intuitiva y adaptable construida con `Tkinter` y componentes `ttk`.
* **Operaciones CRUD Completas:**
    * **Agregar:** Inserta nuevos registros con validación de campos vacíos y formatos numéricos.
    * **Leer/Actualizar:** Carga automática de datos en un componente `Treeview` interactivo.
    * **Editar:** Modificación ágil seleccionando directamente la fila en la tabla.
    * **Eliminar:** Borrado seguro con ventana emergente de confirmación.
* **Autocompletado:** Al hacer clic en cualquier estudiante de la tabla, sus datos se cargan automáticamente en los campos de edición.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Python 3.x
* **Interfaz Gráfica:** Tkinter / TTK
* **Base de Datos:** SQLite3

---

## 📦 Estructura de Datos

La aplicación genera automáticamente un archivo llamado `estudiantes.db` al iniciar por primera vez. La estructura de la tabla es la siguiente:

| Campo | Tipo de Datos | Descripción |
| :--- | :--- | :--- |
| `id` | INTEGER | Clave primaria, autoincremental |
| `nombre` | TEXT | Nombre completo del alumno |
| `carrera` | TEXT | Carrera universitaria/técnica |
| `nota` | REAL | Calificación final |

---

## ⚙️ Requisitos e Instalación

Para ejecutar este proyecto no necesitas instalar librerías externas de terceros (`pip`), ya que tanto `tkinter` como `sqlite3` forman parte de la librería estándar de Python.

1. **Clona este repositorio** o descarga el archivo del código fuente.
2. Asegúrate de tener Python instalado en tu sistema.
3. Ejecuta el script desde tu terminal o consola de comandos:

```bash
python nombre_de_tu_archivo.py
