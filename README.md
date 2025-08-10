# ExpressServerRGH

Página personal de Raúl González construida con Express.js para servir contenido estático y dar acceso a diferentes proyectos de prueba.

## Instalación

1. Clona el repositorio
2. Instala las dependencias:
```bash
npm install
```

## Cómo arrancar la aplicación

Para iniciar el servidor de desarrollo:

```bash
npm start
```

La aplicación se ejecutará en `http://localhost:3000` y se recargará automáticamente cuando hagas cambios en los archivos gracias a nodemon.

## Cómo añadir un nuevo enlace

Para agregar un nuevo proyecto a la página:

1. **Crea la carpeta del proyecto** en el directorio raíz:
   ```bash
   mkdir proyectoX
   ```

2. **Añade el contenido** de tu proyecto dentro de la carpeta (debe incluir un `index.html`):
   ```
   proyectoX/
   └── index.html
   ```

3. **Actualiza la lista de proyectos** en `index.html`. Busca la sección con id `proyectos` y añade un nuevo elemento a la lista:
   ```html
   <section id="proyectos">
     <h2>Proyectos</h2>
     <ul>
       <li><a href="proyecto1/index.html">Proyecto 1 - Nombre del Proyecto 1</a></li>
       <li><a href="proyecto2/index.html">Proyecto 2 - Nombre del Proyecto</a></li>
       <li><a href="proyectoX/index.html">Proyecto X - Descripción del nuevo proyecto</a></li>
     </ul>
   </section>
   ```

4. **Guarda los cambios** - el servidor se recargará automáticamente y el nuevo enlace estará disponible.

## Estructura del proyecto

```
ExpressServerRGH/
├── app.js              # Servidor Express principal
├── index.html          # Página de inicio
├── styles.css          # Estilos CSS
├── package.json        # Configuración del proyecto
├── proyecto1/          # Ejemplo de proyecto
└── proyecto2/          # Ejemplo de proyecto
```

## Tecnologías utilizadas

- **Express.js** - Framework web para Node.js
- **nodemon** - Herramienta de desarrollo para reinicio automático
- **HTML5/CSS3** - Frontend estático