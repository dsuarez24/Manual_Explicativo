# Manual de Referencia sobre SVG y Node.js

## Índice

1. [SVG](#svg)
   - [¿Qué es SVG?](#qué-es-svg)
   - [Cómo funciona SVG](#cómo-funciona-svg)
   - [Cómo utilizar SVG](#cómo-utilizar-svg)

2. [Node.js](#nodejs)
   - [¿Qué es Node.js?](#qué-es-nodejs)
   - [Cómo funciona Node.js](#cómo-funciona-nodejs)
   - [Cómo utilizar Node.js](#cómo-utilizar-nodejs)

---

## SVG

### ¿Qué es SVG?

SVG (Scalable Vector Graphics) es un formato de imagen basado en XML que se utiliza para describir gráficos vectoriales bidimensionales. A diferencia de los formatos de imagen rasterizados como PNG o JPG, los gráficos SVG se basan en geometría vectorial, lo que permite que se escalen sin pérdida de calidad.

### Cómo funciona SVG

SVG permite definir formas, líneas, texto, y otros elementos gráficos en un documento utilizando etiquetas XML. Al ser un lenguaje basado en XML, SVG permite la manipulación de gráficos mediante JavaScript y CSS, lo que lo convierte en una opción poderosa para gráficos interactivos en la web.

Cada elemento gráfico en SVG es una etiqueta específica como `<circle>`, `<rect>`, o `<path>`, donde cada una tiene atributos para definir el tamaño, la posición, el color, y otros estilos.

### Cómo utilizar SVG

SVG puede utilizarse en HTML directamente dentro de una página web o como un archivo externo. Aquí hay algunos ejemplos de cómo emplear SVG en diferentes contextos:

1. **Incrustado en HTML**:
   ```html
   <svg width="100" height="100">
       <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
   </svg>
2. **Archivo SVG externo**
   ```html
   <img src="imagen.svg" alt="Gráfico SVG" />
3. **Estilos con CSS**
    ```html
   <style>
    svg { width: 200px; height: 200px; }
    circle { fill: blue; }
   <style>
    
## Node.js

### ¿Qué es Node.js?

Node.js es un entorno de ejecución de JavaScript basado en el motor V8 de Google Chrome. Permite ejecutar JavaScript en el servidor, extendiendo las capacidades de JavaScript más allá del navegador. 
Node.js es especialmente popular para desarrollar aplicaciones en tiempo real y API gracias a su arquitectura asíncrona y basada en eventos.

### ¿Cómo funciona Node.js?

Node.js ejecuta JavaScript en el servidor y aprovecha su modelo de operación asíncrono, lo que significa que muchas operaciones pueden realizarse sin bloquear el hilo principal de ejecución. 
Esto permite que Node.js sea altamente eficiente para manejar múltiples aplicaciones y tareas simultáneamente.
Node.js utiliza un sistema de módulos (CommonJS) para organizar y reutilizar código, y cuenta con un amplio ecosistema de paquetes disponibles a través de npm (Node Package Manager).

### Cómo utilizar Node.js

 Para comenzar a utilizar Node.js, sigue estos pasos básicos:

1. **Instalación**:

   Puedes descargar e instalar Node.js desde nodejs.org .
   
   Después de instalar, verifique la instalación
   ```html
   node -v
   npm -v
2. **Hola Mundo en Node.js**

   Crea un archivo llamado app.js
   ```html
     // app.js
   console.log("¡Hola, mundo desde Node.js!");
3. **Ejecuta el archivo con el comando:**
    ```html
   node app.js
4. **Servidor básico**:
   ```html
   const http = require('http');
   const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('¡Hola desde Node.js!');
   });

   server.listen(3000, () => {
    console.log('Servidor escuchando en http://localhost:3000');
   });

2. **Iniciar el servidor con**
   ```html
   node app.js

## Canvas

   https://github.com/osanchez2019490/Tutorial_Canvas.git
