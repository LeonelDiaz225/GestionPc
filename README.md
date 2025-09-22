# Software de Gestión para Técnico de PC 🖥️

Un sistema completo de gestión diseñado específicamente para técnicos de PC, que permite organizar clientes, equipos, reparaciones y el flujo de trabajo diario de manera eficiente.

## 🛠️ Tecnologías Utilizadas

Este proyecto utiliza un stack de tecnologías moderno y escalable, dividiendo la aplicación en frontend y backend para una mejor organización y mantenimiento.

### 🎨 Frontend: Next.js, TypeScript y Shadcn/ui

El frontend se encarga de toda la interfaz de usuario (UI) y la interacción directa con el técnico.

- **Next.js**: Framework de React que optimiza el rendimiento y la experiencia del usuario. Permite el renderizado del lado del servidor (SSR) y la generación de sitios estáticos, lo que hace que la aplicación sea increíblemente rápida.

- **TypeScript**: Un superconjunto de JavaScript que añade tipado estático. Esto permite escribir código más robusto, reducir errores en tiempo de desarrollo y facilitar el mantenimiento a largo plazo del proyecto.

- **Shadcn/ui**: Un conjunto de componentes de UI personalizables y accesibles. Está construido sobre Radix UI y Tailwind CSS, lo que proporciona control total sobre el diseño y una base sólida para crear una interfaz moderna y profesional.

### ⚙️ Backend: Node.js, Express y Prisma

El backend es el corazón de la aplicación, manejando la lógica de negocio, la autenticación y la conexión con la base de datos.

- **Node.js**: Entorno de ejecución de JavaScript en el servidor. Es la elección perfecta para construir APIs rápidas y eficientes gracias a su modelo asíncrono.

- **Express.js**: Un framework minimalista y flexible para Node.js. Ayuda a crear de forma sencilla las rutas (endpoints) de la API que el frontend consumirá para obtener y modificar los datos.

- **Prisma**: Un ORM (Object-Relational Mapper) de última generación que simplifica la interacción con la base de datos. En lugar de escribir código SQL, utiliza un cliente tipado para realizar consultas de forma segura e intuitiva. Prisma también gestiona las migraciones de la base de datos de manera automática.

### 🗄️ Base de Datos: MySQL

Se utiliza un sistema de gestión de bases de datos relacionales robusto y confiable.

- **MySQL**: Reconocido por su rendimiento y escalabilidad, MySQL es ideal para almacenar la información del software de gestión.

- **Prisma**: Se encarga de toda la comunicación con MySQL, permitiendo definir el esquema de datos de manera declarativa y ejecutar migraciones de forma segura a medida que el proyecto evolucione.

## 🏗️ Arquitectura del Sistema

El flujo de información de la aplicación se estructura de la siguiente manera:

```
[FRONTEND (Next.js)] <--- Peticiones HTTP ---> [BACKEND (Express)]
       |                                                |
(Shadcn/ui, TypeScript)                           (Prisma, Node.js)
       |                                                |
  Interfaz de Usuario                           Lógica del Negocio y API
       |                                                |
       -----------------> [BASE DE DATOS (MySQL)] <-----
             (Almacenamiento de datos, relaciones)
```

Este stack tecnológico permite construir una aplicación sólida, mantenible y con excelente rendimiento.

## 🚀 Características Principales

- **Gestión de Clientes**: Registro y seguimiento completo de clientes
- **Control de Equipos**: Inventario detallado de equipos en reparación
- **Seguimiento de Reparaciones**: Estado y progreso de cada trabajo
- **Interfaz Moderna**: Diseño intuitivo y responsive
- **Tipado Fuerte**: Código más seguro y mantenible con TypeScript
- **Base de Datos Robusta**: Almacenamiento confiable con MySQL

## 🛠️ Instalación y Configuración

### Prerrequisitos

- Node.js (versión 18 o superior)
- MySQL (versión 8.0 o superior)
- npm o yarn
