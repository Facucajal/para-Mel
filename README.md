# Para Mel

Una mini web romántica para invitar a Mel a salir.

## Cómo publicarla en GitHub Pages

1. Subí estos archivos al repositorio `Facucajal/para-Mel`.
2. En GitHub, abrí `Settings`.
3. Entrá a `Pages`.
4. En `Build and deployment`, elegí `Deploy from a branch`.
5. Elegí la rama `main` y la carpeta `/root`.
6. Guardá los cambios.

La URL debería quedar así:

```text
https://facucajal.github.io/para-Mel/
```

## Cómo conectar el email

La web ya tiene dos caminos:

- Si no configurás nada, al enviar el formulario abre un email listo con `mailto`.
- Para recibir el envío automáticamente sin que Mel tenga que mandar un email manual, creá un formulario en Formspree y reemplazá esta línea en `index.html`:

```js
const FORM_ENDPOINT = "";
```

por tu endpoint de Formspree:

```js
const FORM_ENDPOINT = "https://formspree.io/f/tu_codigo";
```

El fallback con `mailto` ya está configurado para `facucajal9@gmail.com`.
