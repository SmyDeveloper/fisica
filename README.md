# Auditoría de una IA astrónoma

Laboratorio educativo para estudiantes de 3.º o 4.º año. Combina exploración de
datos estelares, primer intento obligatorio, auditoría de afirmaciones e
interacción socrática con Groq.

## Publicación en Netlify

1. Subir esta carpeta a un repositorio de GitHub.
2. En Netlify, seleccionar **Add new project → Import an existing project**.
3. Conectar el repositorio. Netlify leerá automáticamente `netlify.toml`.
4. En **Project configuration → Environment variables**, crear:
   - `GROQ_API_KEY`: la clave privada de Groq.
   - `GROQ_MODEL` (opcional): por defecto usa `openai/gpt-oss-20b`.
5. Realizar un nuevo deploy después de guardar las variables.
6. Probar la conversación en la etapa **Auditoría**.

Nunca colocar la API key en `index.html`, JavaScript público, GitHub ni este archivo.

## Prueba local opcional

Con Netlify CLI instalado:

```bash
netlify dev
```

Crear localmente un archivo `.env` con `GROQ_API_KEY`. Está excluido de Git.

## Integración en Campus ORT

Crear un botón o enlace que abra la URL publicada por Netlify en una pestaña nueva.

