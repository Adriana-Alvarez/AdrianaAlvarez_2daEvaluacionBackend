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



# Endpoint desarrollado
- POST /usuarios/crear/
Encargado de registrar un nuevo usuario en la base de datos

# Prueba el endpoint con POSTMAN
- Se debe levantar el servicio con ayuda de
    -- python manage.py runserver
- Se debe copiar la ruta en la que se levanta el servicio acompañado de usuarios/crear/
    -- http://127.0.0.1:8000/usuarios/crear/
- Se debe poner en metodo POST pegando la ruta permitiendo el ingreso del registro en JSON
- Ejemplo en JSON para poder ingrear un nuevo usuario

{
    "usuario": "nombre_usuario",
    "contrasenia": "contraseña_plana",
    "correo": "email@ejemplo.com",
    "rol": "usuario" 
}

- En caso de una introducción correcta se muestra el siguiente JSON

{
    "idusuario": 11,
    "usuario": "nombre_usuario"
}
