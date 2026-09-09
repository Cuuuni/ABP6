# Preparación ABP M6

Proyecto de ejemplo: gestión de usuarios con Express y Handlebars.

## Descripción

Aplicación Node.js que muestra y permite gestionar usuarios (operaciones básicas desde la interfaz). Utiliza Express como servidor, Handlebars para las vistas y un fichero JSON local para persistir los datos de ejemplo.

## Tecnologías

- Node.js
- Express
- Express Handlebars
- Moment, UUID, Chalk

## Estructura principal

- `server.js` - punto de entrada que inicia la app y acepta el puerto por argumento.
- `src/app.js` - configuración de Express y middlewares.
- `src/routes/` - rutas de la aplicación (`users.routes.js`, `views.routes.js`).
- `src/controllers/` - controladores para lógica de rutas.
- `src/models/User.model.js` - modelo/funciones relacionadas con usuarios.
- `src/data/users.json` - datos persistidos de ejemplo.
- `public/` - assets estáticos (CSS, JS, imágenes).
- `src/views/` - plantillas Handlebars.

## Instalación

1. Asegúrate de tener instalado Node.js (versión 16+ recomendada).
2. Desde la raíz del proyecto, instala dependencias:

```bash
npm install
```

## Ejecución

- Modo producción:

```bash
npm start
```

- Modo desarrollo (observa cambios):

```bash
npm run dev
```

- Ejecutar en un puerto distinto (por ejemplo 3001):

```bash
node server.js -p 3001
# o
npm start -- -p 3001
```

Por defecto el servidor escucha en `http://localhost:3000`.

## Rutas y uso

- Las vistas principales (interfaz) se sirven desde las rutas definidas en `src/routes/views.routes.js`.
- Las operaciones relacionadas con usuarios están en `src/routes/users.routes.js` y usan los controladores en `src/controllers/`.
- Los cambios de usuarios se guardan en `src/data/users.json`.

## Notas

- Es un proyecto didáctico: no está pensado para producción ni para manejar datos sensibles.
- Para pruebas, abre el navegador en `http://localhost:3000` (o el puerto que indiques).

Si quieres, puedo añadir una sección con ejemplos de peticiones (cURL/Postman) o mejorar la documentación de las rutas.# ABP6
