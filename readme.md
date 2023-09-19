# Configuración Básica de React con Vite

Este README te guiará a través de los pasos para configurar un proyecto de React utilizando Vite y crear un componente React básico.

## Requisitos Previos

Asegúrate de tener Node.js instalado en tu sistema. Puedes descargarlo desde [https://nodejs.org/](https://nodejs.org/).

## Creación del Proyecto

1. Abre tu terminal y navega hasta la ubicación donde deseas crear tu proyecto.

2. Ejecuta el siguiente comando para crear un nuevo proyecto Vite con React:

   ```bash
   npx create-react@latest my-react-vite-app
   ```

   Esto creará un directorio llamado `my-react-vite-app` con la estructura básica del proyecto.

3. Navega al directorio del proyecto:

   ```bash
   cd my-react-vite-app
   ```

## Estructura de Carpetas

La estructura de carpetas básica de tu proyecto se verá así:

```
my-react-vite-app/
│
├── node_modules/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── App.css
│   ├── App.js
│   ├── index.css
│   └── index.js
├── .gitignore
├── package.json
├── README.md
└── ...
```

## Creación de un Componente React

1. Dentro del directorio `src`, puedes crear un componente React. Por ejemplo, crearemos un componente llamado `MiComponente.js`.

   ```jsx
   // src/MiComponente.jsx
   import React from "react";

   function MiComponente() {
     return (
       <div>
         <h1>Mi Componente React</h1>
         <p>Este es un componente React básico.</p>
       </div>
     );
   }

   export default MiComponente;
   ```

2. Ahora, puedes importar y utilizar este componente en `src/App.js` o en cualquier otro archivo donde lo necesites.

   ```jsx
   // src/App.jsx
   import React from "react";
   import "./App.css";
   import MiComponente from "./MiComponente";

   function App() {
     return (
       <div className="App">
         <MiComponente />
       </div>
     );
   }

   export default App;
   ```

## Ejecución del Proyecto

Para iniciar tu proyecto y verlo en un navegador, ejecuta el siguiente comando en la terminal dentro del directorio del proyecto:

```bash
npm install   # Instala las dependencias (solo la primera vez)
npm run dev   # Inicia el servidor de desarrollo
```

Esto iniciará un servidor de desarrollo y abrirá tu proyecto en el navegador predeterminado.

¡Ahora estás listo para comenzar a desarrollar tu aplicación React con Vite!
