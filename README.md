# Portafolio BlandsKron

Este es el repositorio del proyecto Portafolio BlandsKron, un sitio web construido con Django y estilizado con Tailwind CSS.

## Requisitos Previos

- Python 3.x
- Node.js y npm
- Git

## Instalación

Sigue estos pasos para descargar e iniciar el proyecto en tu entorno local.

### 1. Clonar el Repositorio

Primero, clona este repositorio en tu máquina local.

```bash
git clone <URL-DEL-REPOSITORIO>
cd portfolioblandskron
```

### 2. Crear y Activar un Entorno Virtual

Crea un entorno virtual para el proyecto.

```bash
python -m venv env
```

Activa el entorno virtual:

- En Windows:
  ```bash
  .\env\Scripts\activate
  ```

- En macOS y Linux:
  ```bash
  source env/bin/activate
  ```

### 3. Instalar las Dependencias de Python

Con el entorno virtual activado, instala las dependencias de Python listadas en el archivo `requirements.txt`.

```bash
pip install -r requirements.txt
```

### 4. Instalar las Dependencias de Node.js

Navega al directorio donde está el archivo `package.json` e instala las dependencias de Node.js.

```bash
npm install
```

### 5. Compilar Tailwind CSS

Compila el archivo CSS de Tailwind.

```bash
npx tailwindcss -i ./static/css/tailwind.css -o ./static/css/output.css --watch
```

### 6. Ejecutar las Migraciones

Ejecuta las migraciones de la base de datos de Django.

```bash
python manage.py migrate
```

### 7. Recolectar Archivos Estáticos

Recoge los archivos estáticos de Django.

```bash
python manage.py collectstatic
```

### 8. Iniciar el Servidor de Desarrollo

Finalmente, inicia el servidor de desarrollo de Django.

```bash
python manage.py runserver
```

Abre tu navegador y ve a `http://127.0.0.1:8000/` para ver el sitio web en funcionamiento.

## Selector de Modo Light/Dark/System

El proyecto incluye un selector para cambiar entre los modos Light, Dark y System. Puedes encontrar los botones en la cabecera del sitio web.

## Estructura del Proyecto

- `myproject/`: Contiene los archivos principales del proyecto Django.
- `myapp/`: Contiene la aplicación Django.
- `static/`: Archivos estáticos incluyendo CSS compilado de Tailwind.
- `templates/`: Plantillas HTML del proyecto.
- `env/`: Entorno virtual (ignorado en Git).
- `node_modules/`: Dependencias de Node.js (ignorado en Git).

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o envía un pull request para cualquier mejora o corrección.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
