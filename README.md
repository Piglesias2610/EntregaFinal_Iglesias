# Proyecto Final - Web de Informacion Gaming
## Descripción General

Este proyecto es una web de Informacion Gaming desarrollado con Django, diseñado para gestionar usuarios y recursos relacionados con consolas, funkos, juegos y periféricos. La aplicación está compuesta por dos módulos principales: `users` para la gestión de usuarios y `AppBcs` para la gestión de consolas y otros objetos coleccionables.

El sistema permite realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) en cada uno de los módulos y está configurado para permitir la autenticación de usuarios y la asignación de permisos administrativos.

### Directorio Principal (`ProyectoFinal`)

Este directorio contiene los archivos de configuración principales del proyecto, incluyendo `settings.py`, `urls.py`, y otros archivos de configuración.

- **`__init__.py`**: Marca el directorio como un paquete Python.
- **`settings.py`**: Contiene la configuración global del proyecto, como la configuración de la base de datos, aplicaciones instaladas, y más.
- **`urls.py`**: Define las rutas URL para todo el proyecto.
- **`wsgi.py`**: Utilizado para desplegar la aplicación en servidores web compatibles con WSGI.
- **`asgi.py`**: Utilizado para desplegar la aplicación en servidores compatibles con ASGI (para WebSockets y otros).
### Aplicación `users`

Este módulo gestiona la autenticación y la administración de usuarios. Incluye modelos personalizados para extender el modelo de usuario predeterminado de Django.

- **`models.py`**: Define el modelo de usuario extendido, si lo hay.
- **`views.py`**: Contiene las vistas para el registro, inicio de sesión, perfil de usuario, y más.
- **`forms.py`**: Formularios para el registro y edición de perfil de usuario.
- **`urls.py`**: Define las rutas específicas para la gestión de usuarios, como `/login/`, `/register/`, y `/profile/`.
- **`admin.py`**: Configura el acceso al modelo de usuario desde el panel de administración de Django.

### Aplicación `AppBcs`

Este módulo gestiona la información relacionada con consolas, funkos, juegos y periféricos. Ofrece CRUD para cada uno de estos elementos.

- **`models.py`**: Define los modelos `Consola`, `Funko`, `Juego`, y `Periferico`.
- **`views.py`**: Contiene las vistas que manejan las operaciones CRUD para cada modelo.
- **`urls.py`**: Define las rutas para acceder a las vistas de `AppBcs`, como `/AppBcs/listar_consolas/`, `/AppBcs/create_consola/`.
- **`templates/AppBcs/`**: Contiene las plantillas HTML utilizadas por las vistas de `AppBcs`.
- **`static/AppBcs/`**: Archivos estáticos como CSS y JS específicos para `AppBcs`.
- **`admin.py`**: Configura los modelos de `AppBcs` en el panel de administración de Django.
## Descripción de las Funcionalidades

El proyecto ofrece las siguientes funcionalidades:

- **Autenticación de Usuarios**:
  - Registro de nuevos usuarios.
  - Inicio de sesión y cierre de sesión.
  - Edición del perfil de usuario.

- **Gestión de Consolas**:
  - Crear, listar, editar y eliminar consolas.

- **Gestión de Funkos**:
  - Crear, listar, editar y eliminar figuras Funko Pop.

- **Gestión de Juegos**:
  - CRUD completo para gestionar títulos de videojuegos.

- **Gestión de Periféricos**:
  - CRUD completo para la gestión de periféricos asociados a consolas.
## Detalles Técnicos

### Modelos

- **`Consola`**: Modelo que representa una consola de videojuegos.
- **`Funko`**: Modelo que representa una figura Funko Pop.
- **`Juego`**: Modelo para títulos de videojuegos.
- **`Periferico`**: Modelo que representa un periférico de consola.

### Vistas

Las vistas están organizadas de acuerdo a las operaciones CRUD:

- **`create_*`**: Vistas para crear nuevos registros en la base de datos.
- **`list_*`**: Vistas para listar todos los elementos de un tipo específico.
- **`update_*`**: Vistas para actualizar elementos existentes.
- **`delete_*`**: Vistas para eliminar elementos.

### URLs

Las rutas de acceso están definidas en `urls.py` para cada aplicación:

- **Usuarios**: `/login/`, `/register/`, `/profile/`.
- **AppBcs**:
  - **Consolas**: `/AppBcs/listar_consolas/`, `/AppBcs/create_consola/`, etc.
  - **Funkos**: `/AppBcs/listar_funkos/`, `/AppBcs/create_funko/`, etc.
  - **Juegos**: `/AppBcs/listar_juegos/`, `/AppBcs/create_juego/`, etc.
  - **Periféricos**: `/AppBcs/listar_perifericos/`, `/AppBcs/create_periferico/`, etc.

## Descripción de las Funcionalidades

El proyecto ofrece las siguientes funcionalidades:

- **Autenticación de Usuarios**:
  - Registro de nuevos usuarios.
  - Inicio de sesión y cierre de sesión.
  - Edición del perfil de usuario.

- **Gestión de Consolas**:
  - Crear, listar, editar y eliminar consolas.

- **Gestión de Funkos**:
  - Crear, listar, editar y eliminar figuras Funko Pop.

- **Gestión de Juegos**:
  - CRUD completo para gestionar títulos de videojuegos.

- **Gestión de Periféricos**:
  - CRUD completo para la gestión de periféricos asociados a consolas.
## Detalles Técnicos

### Modelos

- **`Consola`**: Modelo que representa una consola de videojuegos.
- **`Funko`**: Modelo que representa una figura Funko Pop.
- **`Juego`**: Modelo para títulos de videojuegos.
- **`Periferico`**: Modelo que representa un periférico de consola.

### Vistas

Las vistas están organizadas de acuerdo a las operaciones CRUD:

- **`create_*`**: Vistas para crear nuevos registros en la base de datos.
- **`list_*`**: Vistas para listar todos los elementos de un tipo específico.
- **`update_*`**: Vistas para actualizar elementos existentes.
- **`delete_*`**: Vistas para eliminar elementos.

### URLs

Las rutas de acceso están definidas en `urls.py` para cada aplicación:

- **Usuarios**: `/login/`, `/register/`, `/profile/`.
- **AppBcs**:
  - **Consolas**: `/AppBcs/listar_consolas/`, `/AppBcs/create_consola/`, etc.
  - **Funkos**: `/AppBcs/listar_funkos/`, `/AppBcs/create_funko/`, etc.
  - **Juegos**: `/AppBcs/listar_juegos/`, `/AppBcs/create_juego/`, etc.
  - **Periféricos**: `/AppBcs/listar_perifericos/`, `/AppBcs/create_periferico/`, etc.

### Plantillas

Las plantillas HTML están organizadas por aplicación y utilizan el sistema de plantillas de Django. Se encuentran en los directorios `templates/users/` y `templates/AppBcs/`.

### Archivos Estáticos

Los archivos estáticos como CSS y JS específicos para cada aplicación están en `static/users/` y `static/AppBcs/`.



## Contribución

Si deseas contribuir a este proyecto, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`).
3. Realiza los cambios necesarios y haz un commit (`git commit -m 'Añadir nueva funcionalidad'`).
4. Envía los cambios a la rama principal (`git push origin feature/nueva-funcionalidad`).
5. Crea un Pull Request.

Las contribuciones son bienvenidas y apreciadas.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

Desarrollado por Piero Alejandro Iglesias Perez








