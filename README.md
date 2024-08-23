## Opciones de Etiquetado en Markdown

### Encabezados
En Markdown, puedes crear encabezados usando el símbolo `#`. 
- `#` para un encabezado de nivel 1.
- `##` para un encabezado de nivel 2.
- `###` para un encabezado de nivel 3, y así sucesivamente.

### Listas
- Puedes crear listas no ordenadas con `-`, `*`, o `+`.
1. Las listas ordenadas se crean usando números seguidos de un punto (`1.`).

### Enlaces
Puedes crear enlaces con `[texto del enlace](URL)`.

### Imágenes
Para añadir una imagen, usa `![texto alternativo](URL de la imagen)`.

## Comandos de Git

### Verificar el Estado del Repositorio Local
- `git status`: Muestra el estado actual del repositorio, incluyendo cambios que aún no se han añadido o confirmado.

### Añadir Archivos al Repositorio
- `git add [archivo]`: Añade un archivo específico a la zona de preparación (staging area).
- `git add .`: Añade todos los archivos cambiados en el directorio actual a la zona de preparación.

### Añadir Comentarios a un Commit
- `git commit -m "Descripción del commit"`: Realiza un commit con un mensaje descriptivo.

### Subir Cambios al Repositorio Remoto
- `git push`: Sube los commits locales al repositorio remoto.

### Manejo de Ramas
- `git branch [nombre-rama]`: Crea una nueva rama.
- `git checkout [nombre-rama]`: Cambia a la rama especificada.
- `git branch -d [nombre-rama]`: Elimina la rama especificada.

### Retroceder a un Commit Específico (Rollback)
- `git reset --hard [commit]`: Retrocede el repositorio al commit especificado, descartando cualquier cambio posterior.
  - **Ejemplo:** Si deseas retroceder a un commit específico con el hash `abc123`, ejecutarías `git reset --hard abc123`.
- `git revert [commit]`: Crea un nuevo commit que deshace los cambios de un commit específico sin alterar el historial de commits. Este comando es útil si quieres revertir un cambio pero conservar el historial.
- `git checkout [commit]`: Te permite navegar a un commit específico en modo "detached HEAD". Esto es útil para explorar el estado del repositorio en un punto específico sin hacer cambios permanentes.
