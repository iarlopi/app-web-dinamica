# Aplicación Web Dinámica

Esta es una aplicación web dinámica desarrollada con Node.js, Express y PostgreSQL, desplegada en la nube mediante Render.

## Enlace a la aplicación

Se puede acceder a la aplicación aquí:
https://app-web-dinamica.onrender.com

---

## Descripción

La aplicación permite visualizar y gestionar usuarios almacenados en una base de datos en la nube. Además, integra contenido externo mediante APIs y servicios en línea.

El sistema funciona con una arquitectura cliente-servidor, donde el frontend realiza peticiones al backend para obtener y modificar datos en tiempo real.

---

## Tecnologías utilizadas

* Node.js
* Express
* PostgreSQL
* HTML, CSS, JavaScript
* Render (deploy en la nube)

---

## Funcionalidades

* Visualización de usuarios desde la base de datos
* Agregar nuevos usuarios
* Editar usuarios existentes
* Eliminar usuarios
* Obtención de fecha desde la base de datos
* Integración de contenido externo (video y APIs)

---

## Base de datos

La base de datos está alojada en la nube mediante Render, lo que permite que todos los usuarios compartan la misma información en tiempo real.

La tabla principal utilizada es:

```sql
CREATE TABLE usuarios (
    id SERIAL PRIMARY KEY,
    nombre VARCHAR(100),
    email VARCHAR(100)
);
```

---

## Variables de entorno

Para el correcto funcionamiento, se utilizan variables de entorno para proteger credenciales sensibles.

Ejemplo:

```
DATABASE_URL=postgresql://usuario:password@host:puerto/db
```

Este archivo no se incluye en el repositorio por motivos de seguridad.

---

## Instalación local

1. Clonar el repositorio:

```
git clone https://github.com/tu-usuario/app-web-dinamica.git
```

2. Instalar dependencias:

```
npm install
```

3. Crear archivo `.env` con las credenciales de la base de datos

4. Ejecutar la aplicación:

```
node index.js
```

5. Abrir en el navegador:

```
http://localhost:3000
```

---

## Diseño responsivo

La interfaz se adapta a distintos tamaños de pantalla, permitiendo una experiencia adecuada tanto en dispositivos móviles como en escritorio.

---

## Seguridad

Se evitaron buenas prácticas como:

* No subir archivos `.env` al repositorio
* Uso de variables de entorno en producción
* Manejo de credenciales fuera del código fuente

---

## Autor

Proyecto desarrollado por Isis López

---
