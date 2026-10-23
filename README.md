# Parcial 2 - Django Backend

Sistema para gestionar proyectos y sus tareas, hecho con Django nativo y SQLite.

- Proyecto Django: `config`
- Aplicación: `gestion`
- Modelos: `Proyecto` (nombre, descripcion, fecha_inicio) y `Tarea` (titulo, completada, proyecto → ForeignKey a Proyecto con `on_delete=models.CASCADE`)
- Ambos modelos registrados en el administrador.
- `db.sqlite3` incluye 3 proyectos con 2 tareas cada uno.

## Cómo ejecutarlo

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Luego entrar a http://127.0.0.1:8000/admin/

Capturas del administrador en la carpeta `capturas/`.
