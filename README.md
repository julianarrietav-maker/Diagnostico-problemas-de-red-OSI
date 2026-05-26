# Diagnostico-problemas-de-red-OSI
problemas de red OSI
# Diagnóstico de Problemas por Capa OSI

Aplicación web educativa desarrollada en HTML, CSS y JavaScript puro para identificar en qué capa del modelo OSI puede encontrarse una falla de red, a partir de un problema seleccionado por el usuario.

## Objetivo

Ayudar al estudiante a relacionar fallas comunes de red con la capa correspondiente del modelo OSI, mostrando una descripción del problema, su posible causa y una recomendación básica de solución.

## Tema del proyecto

Modelo OSI y TCP/IP

## Idea de la aplicación

La aplicación permite seleccionar un problema de red desde una lista desplegable. Luego, al presionar el botón de diagnóstico, muestra:

- El problema seleccionado.
- La capa OSI relacionada.
- Una breve descripción.
- La posible causa.
- Una recomendación básica.

## Tecnologías utilizadas

- HTML5
- CSS
- JavaScript

```

## Arquitectura por capas
mi-proyecto/
│
├── index.html
├── css/
│   └── estilos.css
├── js/
│   ├── datos.js
│   ├── logica.js
│   └── presentacion.js
├── assets/
│   └── image.jpg
└── docs/

El proyecto está organizado en tres capas, de acuerdo con la guía del taller:

### 1. Capa de presentación
Archivos:
- `index.html`
- `css/estilos.css`
- `js/presentacion.js`

Responsabilidades:
- Mostrar la interfaz.
- Capturar la selección del usuario.
- Escuchar eventos.
- Mostrar resultados en pantalla.

### 2. Capa de lógica
Archivo:
- `js/logica.js`

Responsabilidades:
- Validar la entrada.
- Buscar el problema seleccionado.
- Devolver el diagnóstico correspondiente.
- No acceder al DOM.

### 3. Capa de datos
Archivo:
- `js/datos.js`

Responsabilidades:
- Almacenar la información del dominio.
- Guardar problemas, capas, descripciones, causas y recomendaciones.
- No hacer cálculos ni acceder al DOM.

## Flujo de funcionamiento

1. El usuario abre la aplicación.
2. Selecciona un problema de red.
3. `presentacion.js` captura el evento del botón.
4. `presentacion.js` llama a `logica.js`.
5. `logica.js` consulta la información en `datos.js`.
6. `logica.js` devuelve el resultado.
7. `presentacion.js` muestra el diagnóstico en pantalla.

## Cómo ejecutar el proyecto

1. Descargar o clonar este repositorio.
2. Abrir la carpeta en Visual Studio Code.
3. Verificar que la imagen esté dentro de la carpeta `assets`.
4. Abrir el archivo `index.html` en el navegador.

## Autor

Oscar  
Estudiante de Ingeniería de Sistemas

## Observación

Este proyecto fue desarrollado como parte de un taller académico sobre redes y cableado estructurado, aplicando arquitectura por capas y uso guiado de IA como apoyo al desarrollo.
