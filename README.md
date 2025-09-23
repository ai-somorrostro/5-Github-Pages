# Guía Rápida de MkDocs: De Local a GitHub Pages

Esta guía te mostrará los pasos esenciales para crear un sitio de documentación con MkDocs, probarlo localmente y publicarlo en internet utilizando GitHub Pages.

---

### 1. Creación del Entorno Virtual e Instalación de MkDocs

Primero, crearemos un entorno virtual para aislar las dependencias de nuestro proyecto.

*   **Crea el entorno virtual:**
    Abre tu terminal, navega a la carpeta donde quieras crear tu proyecto y ejecuta:
    ```bash
    python -m venv venv
    ```

*   **Activa el entorno virtual:**

    *   En macOS y Linux:
        ```bash
        source venv/bin/activate
        ```

*   **Instala MkDocs:**
    Con el entorno activado, instala MkDocs usando pip, el gestor de paquetes de Python:
    ```bash
    pip install mkdocs
    ```

---

### 2. Creación y Visualización del Sitio Local

Ahora, crearemos la estructura básica de nuestro sitio de documentación.

*   **Crea un nuevo proyecto:**
    Ejecuta el siguiente comando para crear un nuevo proyecto llamado `mi-proyecto`:
    ```bash
    mkdocs new mi-proyecto # PENSAD EL NOMBRE
    ```
    Esto generará una carpeta `mi-proyecto` con la siguiente estructura:
    ```
    mi-proyecto/
        ├── docs/
        │   └── index.md
        └── mkdocs.yml
    ```

*   **Inicia el servidor de desarrollo:**
    Navega a la carpeta de tu proyecto y ejecuta el servidor de MkDocs:
    ```bash
    cd mi-proyecto
    mkdocs serve
    ```
    Este comando inicia un servidor local. Abre tu navegador y ve a `http://127.0.0.1:8000` para ver tu sitio. El servidor se recargará automáticamente cada vez que guardes un cambio en los archivos del proyecto.

---

### 3. Añadir Contenido Básico

Añadiremos una nueva página y la incluiremos en la navegación del sitio.

*   **Crea un nuevo archivo:**
    Dentro de la carpeta `docs`, crea un nuevo archivo llamado `about.md`.

*   **Edita el contenido:**
    Abre `docs/index.md` y `docs/about.md` y añade el contenido que desees en formato Markdown.

*   **Configura la navegación:**
    Abre el archivo `mkdocs.yml` y modifícalo para añadir las páginas a la barra de navegación:
    ```yaml
    site_name: Mi Proyecto de Documentación
    nav:
      - 'Inicio': 'index.md'
      - 'Acerca de': 'about.md'
    ```
Guarda los cambios y el servidor local se actualizará automáticamente mostrando las dos páginas en la navegación.

---

