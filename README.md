# Quietud y Belleza

Este es un sistema web que desarrollé para administrar un centro estético. La idea nace de la necesidad de tener en un solo lugar las citas, los clientes y los servicios, sin depender de agendas físicas ni de hojas de cálculo separadas.

El proyecto está pensado para que la persona encargada del negocio pueda revisar rápidamente qué citas tiene en el día, organizar su agenda, conocer el historial de cada cliente y mantener actualizado su catálogo de tratamientos.

## ¿Qué se puede hacer?

- Iniciar sesión en el panel de administración.
- Ver un dashboard con el resumen de citas, clientes y servicios más solicitados.
- Registrar, confirmar, reprogramar, completar y eliminar citas.
- Consultar la agenda por día, semana o mes.
- Buscar clientes, revisar su información, preferencias e historial de visitas.
- Crear y editar clientes.
- Crear, editar y filtrar servicios por categoría.
- Ver notificaciones de citas pendientes.
- Usar el sistema en modo demostración sin conectarse a una base de datos.
- Usar el panel desde computadora, tablet o celular.

## Pantallas principales

El sistema cuenta con cinco vistas principales:

| Vista     | Descripción                                                          |
| --------- | -------------------------------------------------------------------- |
| Login     | Acceso al panel de administración.                                   |
| Inicio    | Resumen general del negocio y las citas del día.                     |
| Agenda    | Calendario para organizar y dar seguimiento a las citas.             |
| Clientes  | Directorio de clientes, datos de contacto, preferencias e historial. |
| Servicios | Catálogo de tratamientos, precios, duración y rendimiento.           |

## Tecnologías utilizadas

- Angular 21
- TypeScript
- SCSS
- Node.js y Express
- PostgreSQL / Supabase
- JSON Web Token para la sesión

## Estructura del proyecto

```text
src/ng/             Pantallas y componentes de Angular
server/             API, rutas y conexión a base de datos
public/assets/      Imágenes e ilustraciones usadas en la interfaz
tests/              Pruebas del proyecto
docs/screenshots/   Capturas de las pantallas
```

## Ejecutar el proyecto

Primero instala las dependencias:

```bash
npm install
```

Para ejecutar solo la interfaz:

```bash
npm run dev
```

Luego abre:

```text
http://127.0.0.1:5173
```

Desde el login puedes presionar **Explorar demostración** para navegar por todas las pantallas con información de ejemplo.

## Conectar la base de datos

Para utilizar el acceso real y guardar información, crea un archivo `.env` a partir de `.env.example` y completa tus variables:

```env
DATABASE_URL=tu_cadena_de_conexion
ADMIN_USER=tu_usuario
ADMIN_PASSWORD=tu_contrasena
JWT_SECRET=una_clave_larga_y_segura
```

Después ejecuta frontend y backend juntos:

```bash
npm run dev:all
```

La API se ejecuta en el puerto `3001` y Angular en el puerto `5173`.

## Pruebas

```bash
npm test
npm run build
```

## Capturas

Las capturas de la interfaz se encuentran en la carpeta [`docs/screenshots`](docs/screenshots).

---

Proyecto desarrollado por **Aaron Silva**.
