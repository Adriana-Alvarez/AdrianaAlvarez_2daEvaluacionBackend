# Sitio de Podcast del bicentenario - Registro de Usuarios

con el endpoint desarrollado el ingreso de nuevos usuarios a nuestra plataforma se podrá ingresar un nuevo usuario con el objetivo de guardar su información en la base de datos y poder darle vida al proyecto

##  Características

- Registro de usuarios vía API REST.
- Almacenamiento de la información en la base de datos 
- Compatible con Postman y clientes HTTP.

## Requisitos

- Python 3.8+
- Django 4.0+
- Supabase (cuenta gratuita)
- Librerías: `django`, `supabase`, `python-dotenv`
- dependencias 
-- pip insttall django
-- pip install psycopg2-binary
-- pip install supabase

## 📦 Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/usuario/nombre-proyecto.git


# Endpoint desarrollado
- POST /usuarios/crear/
Encargado de registrar un nuevo usuario en la base de datos

- Ejemplo en JSON para poder ingrear para probar con POSTMAN

{
    "usuario": "nombre_usuario",
    "contrasenia": "contraseña_plana",
    "correo": "email@ejemplo.com",
    "rol": "usuario"  # Opcional
}

en caso de una introducción correcta se muestra el siguiente JSON

{
    "idusuario": 11,
    "usuario": "nombre_usuario"
}
