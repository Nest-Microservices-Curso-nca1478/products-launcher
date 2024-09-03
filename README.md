# Products App con Microservicios (Launcher)

Esta es una aplicación en nestjs donde se aplica el concepto de microservicios y submódulos de github.

## Levantar Aplicación (dev)

1. Clonar el repositorio.
2. Inicializar y actualizar Sub-módulos `git submodule update --init --recursive`.
3. Crear un .env basado en el .env.template.
4. Ejecutar el comando `docker compose up --build`.

## Agregar submódulos al repo

Leer el procedimiento para agregar y actualizar submódulos [aquí](./pasos-submodules.md)

## Levantar Aplicación (prod)

1. Clonar el repositorio.
2. Inicializar y actualizar Sub-módulos `git submodule update --init --recursive`.
3. Crear un .env basado en el .env.template.
4. Construir la imagen de prod `docker compose -f docker-compose.prod.yml build`.
5. Levantar la imagen `docker compose -f docker-compose.prod.yml up`.
6. Eliminar los contenedores `docker compose down`
