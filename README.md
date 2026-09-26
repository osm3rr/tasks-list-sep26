# Tasks List

Aplicación sencilla de Django para gestionar una lista de tareas.

## Descripción

Este proyecto incluye:

- Un modelo de `Task` con título, fecha de creación y fecha de actualización.
- Una vista basada en `ListView` para mostrar todas las tareas.
- Una plantilla HTML para listar tareas.
- Configuración base de Django para ejecutar la app localmente.

## Requisitos

- Python 3.10 o superior
- pip
- Virtualenv (opcional, pero recomendado)

## Instalación

1. Clona el repositorio.
2. Entra a la carpeta del proyecto.
3. Crea un entorno virtual:

```bash
python -m venv .venv
```

4. Activa el entorno:

- Windows:

```bash
.venv\Scripts\activate
```

- macOS/Linux:

```bash
source .venv/bin/activate
```

5. Instala las dependencias:

```bash
pip install -r requirements.txt
```

## Configuración

Aplica las migraciones:

```bash
python manage.py migrate
```

## Ejecutar la app

```bash
python manage.py runserver
```

Luego abre en tu navegador:

```text
http://127.0.0.1:8000/
```

## Estructura principal

```text
.
├── django_base/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── tasks/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── migrations/
├── templates/
│   └── tasks-list.html
├── manage.py
├── requirements.txt
├── db.sqlite3
└── README.md
```

## Notas

- El proyecto usa SQLite por defecto.
- Si deseas ampliar la app, puedes agregar funciones como crear, editar, eliminar o marcar tareas como completadas.
