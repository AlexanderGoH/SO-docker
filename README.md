# Proyecto Docker
Este proyecto es una aplicación web la cual permite realizar operaciones CRUD (Create, Read, Update, Delete) en una base de datos de productos.

- **Base de datos**: Turso
- **Backend**: Node.js para manejar la lógica del negocio y las operaciones CRUD.
- **Frontend**: Angular para la interfaz de usuario.
- **Servidor web**: Nginx para servir la aplicación frontend.
- **Contenerización**: Docker para separar y gestionar los servicios de backend y frontend.

## Marco Teórico
### Node.js
Node.js es un entorno de ejecución de JavaScript que permite ejecutar código JavaScript en el servidor. Utiliza un modelo de E/S no bloqueante y orientado a eventos, lo que lo hace eficiente y adecuado para aplicaciones en tiempo real y de alta concurrencia.

### Angular
Angular es un framework de desarrollo de aplicaciones web desarrollado por Google. Utiliza TypeScript y ofrece una arquitectura basada en componentes, lo que facilita la creación de aplicaciones web dinámicas y de alto rendimiento.

### Docker
Docker es una plataforma de contenedorización que permite a los desarrolladores empaquetar aplicaciones y sus dependencias en contenedores. Los contenedores son ligeros, portátiles y aseguran que las aplicaciones se ejecuten de manera consistente en cualquier entorno.

### Docker Compose
Docker Compose es una herramienta para definir y ejecutar aplicaciones multi-contenedor. Utiliza un archivo YAML (docker-compose.yml) para configurar los servicios de una aplicación, y permite iniciar y gestionar todos los contenedores con un solo comando.

### Nginx
Nginx es un servidor web de código abierto y de alto rendimiento. Se utiliza para servir aplicaciones web, actuar como proxy inverso, balanceador de carga, y más. En este proyecto, Nginx se utiliza para servir la aplicación frontend construida con Angular.

### Turso
Turso es una base de datos distribuida que proporciona alta disponibilidad, escalabilidad y rendimiento. Se utiliza para almacenar y gestionar los datos de la aplicación, permitiendo realizar operaciones CRUD de manera eficiente y segura.

## Detalles Técnicos
### Backend (Node.js)
El backend está construido con Node.js y Express.js, y se encarga de manejar las operaciones CRUD en la base de datos. El código se encuentra en el directorio `backend/`.

### Frontend (Angular)
El frontend está construido con Angular y proporciona una interfaz de usuario para interactuar con los datos del backend. El código se encuentra en el directorio `frontend/`.

### Contenerización (Docker)
Ambos servicios (backend y frontend) están contenerizados usando Docker. Los archivos Dockerfile en los directorios `backend/` y `frontend/` definen cómo se construyen las imágenes Docker para cada servicio.
