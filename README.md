


Proyecto Final: Pagina Informativa de Videojuegos,Consolas,Funkos y Periféricos
Descripción
Este es un proyecto web desarrollado con Django que se centra en la compra de productos relacionados con videojuegos, como periféricos, funkos, juegos y consolas. Incluye funcionalidades básicas como la gestión de productos.

Características Principales
Modelos Incluidos:

Consolas:Gestion de las consolas.
Juego: Gestión de los juegos en venta.
Funko: Control de los funkos disponibles.
Periférico: Gestión de los periféricos relacionados con videojuegos.
Funcionalidades:

Crear, actualizar y eliminar juegos y otros productos desde formularios personalizados.
Gestión de usuarios (registro, inicio de sesión).
Instalación y Uso
Requisitos Previos
Python 3.x
Django 3.x
Virtualenv (opcional pero recomendado)
Instrucciones de Instalación
Clona este repositorio:

bash
Copiar código
git clone https://github.com/tuusuario/proyecto-final.git
Accede al directorio del proyecto:

bash
Copiar código
cd proyecto-final
Crea y activa un entorno virtual (opcional):

bash
Copiar código
python -m venv venv
source venv/bin/activate  # En Windows usa: venv\Scripts\activate
Instala las dependencias:

bash
Copiar código
pip install -r requirements.txt
Realiza las migraciones:

bash
Copiar código
python manage.py makemigrations
python manage.py migrate
Ejecuta el servidor:

bash
Copiar código
python manage.py runserver
Accede a la aplicación en tu navegador en http://localhost:8000.

Estructura del Proyecto
El proyecto está organizado de la siguiente manera:

php
Copiar código
proyecto-final/
│
├── productos/         # Aplicación de gestión de productos
├── usuarios/          # Gestión de usuarios y autenticación
├── templates/         # Plantillas HTML
├── static/            # Archivos estáticos (CSS, JS, imágenes)
├── manage.py          # Script de gestión de Django
└── README.md          # Este archivo
Contribuciones
Las contribuciones son bienvenidas. Por favor, abre un "issue" antes de enviar un "pull request".

Licencia
Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para obtener más detalles.
