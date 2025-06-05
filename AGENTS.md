# AGENTS.md

## Descripción General

Este repositorio contiene una plantilla para proyectos de Google Apps Script administrados con `clasp`. Está diseñada para facilitar la colaboración entre desarrolladores humanos y agentes de IA, permitiendo la edición y despliegue desde editores compatibles como Cursor.

## Estructura del Proyecto

```
/src/               # Código fuente de Apps Script
```

> Los directorios `/tests/`, `/docs/`, `/lib/` y `/.github/` pueden crearse cuando sea necesario para pruebas, documentación, bibliotecas compartidas y configuraciones de GitHub.

## Convenciones de Codificación

* **Lenguaje:** JavaScript (ECMAScript 2020) con V8 Runtime
* **Estilo:** Airbnb JavaScript Style Guide
* **Nomenclatura:** CamelCase para variables y funciones; PascalCase para clases
* **Comentarios:** JSDoc para todas las funciones públicas
* **Linter:** ESLint con configuración en `.eslintrc.json`

## Requisitos de Pruebas

* **Framework:** Jest adaptado para Google Apps Script mediante `gas-local`
* **Cobertura mínima:** 90% de líneas y funciones

> Aún no se han configurado los comandos `npm run test` ni `npm run coverage`.

## Integraciones y Servicios Avanzados

Este proyecto puede emplear los siguientes servicios avanzados de Google Apps Script:

* **Sheets API**
* **Drive API**
* **Gmail API**

Asegúrate de habilitar estos servicios en el editor de Apps Script bajo "Servicios Avanzados de Google".

## Directrices para Agentes de IA

* **Modularidad:** Cada función debe estar en su propio archivo dentro de `/src/` y exportarse adecuadamente.
* **Documentación:** Todas las funciones deben tener comentarios JSDoc que describan sus parámetros, retorno y propósito.
* **Pruebas:** Por cada nueva función, se debe crear una prueba correspondiente en `/tests/`.
* **Dependencias:** Evitar añadir nuevas dependencias externas sin aprobación previa.
* **Seguridad:** No almacenar credenciales o información sensible en el código fuente.

## Configuración de Entorno

* **Variables de entorno:** Definidas en un archivo `.env` (excluido del repositorio).
* **Despliegue:** Utilizar las funciones de despliegue de Apps Script para publicar versiones estables.

## Recursos Adicionales

* [Guía de Servicios Avanzados de Google Apps Script](https://developers.google.com/apps-script/guides/services/advanced)
* [Documentación de Google Apps Script](https://developers.google.com/apps-script)
* [Estilo de Código JavaScript de Airbnb](https://github.com/airbnb/javascript)
