

# Proyecto Docker con Bash Script

Este proyecto crea un servidor web Nginx utilizando Docker y automatiza las tareas comunes con un script de Bash.

## Requisitos

- Docker instalado
- Bash (Linux o WSL en Windows)

## Estructura del proyecto

- `Dockerfile`: Define la imagen personalizada de Nginx.
- `index.html`: Archivo HTML que se servirá desde el servidor.
- `script.sh`: Script de Bash para automatizar tareas.
- `README.md`: Documentación del proyecto.

## Uso

1. **Clonar el repositorio**:
   ```bash
   git clone <url-del-repositorio>
   cd mi-proyecto-docker 

2. **Dar permisos de ejecución al script**:
   ```bash
   chmod +x script.sh
   ```

3. **Ejecutar el script**:
   ```bash
   ./script.sh
   ```

4. **Seleccionar una opción del menú**:
   - Opción 1: Construir la imagen Docker
   - Opción 2: Ejecutar el contenedor (accesible en http://localhost:8080)
   - Opción 3: Detener y eliminar el contenedor
   - Opción 4: Eliminar la imagen Docker
   - Opción 5: Salir

## Detalles técnicos

- La imagen Docker utiliza Nginx como base
- El servidor web se expone en el puerto 8080 del host
- El contenido servido es una página HTML simple con un mensaje de bienvenida
