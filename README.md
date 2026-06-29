# Trabajo final Angular — Gestión académica

Sistema de gestión de alumnos y cursos desarrollado con Angular. Incluye autenticación, autorización por roles, estado global con NgRx y una suite de pruebas unitarias para las principales piezas de la aplicación.

## Funcionalidades

- Inicio de sesión y administración de sesión.
- Protección de rutas mediante guards.
- Permisos específicos para administradores.
- Alta, edición y listado de alumnos.
- Alta, edición, detalle y tarjetas de cursos.
- Pipes personalizados para fechas y estados.
- Manejo de autenticación y cursos con NgRx.
- Página de inicio y manejo de rutas inexistentes.

## Stack

- Angular 15
- TypeScript
- Angular Material y CDK
- NgRx Store, Effects y DevTools
- RxJS
- Jasmine, Karma y Angular Testing

## Arquitectura

El código se divide en módulos funcionales: `autenticacion`, `alumnos`, `cursos`, `core` y `shared`. Cada dominio contiene componentes, servicios, rutas y estado cuando corresponde. `core` concentra guards y servicios de sesión; `models` contiene las interfaces de negocio.

## Ejecución local

```bash
npm install
npm start
```

Abrir `http://localhost:4200`.

## Comandos

```bash
npm run build
npm run watch
npm test
```

La configuración del entorno se encuentra en `src/environment/environment.ts`.

> Proyecto educativo orientado a demostrar routing modular, formularios, estado reactivo, permisos y testing en Angular.