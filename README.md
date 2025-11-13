# DevOps

Este directorio contiene recursos y documentación relacionada con las operaciones del proyecto (ci/cd, despliegue y orquestación).

## Contenido

- Archivo(s) Docker / Compose para entornos de desarrollo y producción.
- Scripts y configuración para Jenkins, imágenes de contenedores y demás herramientas de integración/entrega continua.

## Requisitos previos

- Docker y docker-compose instalados en la máquina local.
- Acceso al registry/credenciales si se requiere push de imágenes.

## Uso rápido

1. Para levantar servicios relacionados con devOps (si existe un compose específico):

```bash
cd devOps
docker-compose up -d
```

2. Para ver logs:

```bash
docker-compose logs -f
```

3. Para reconstruir imágenes:

```bash
docker-compose build --no-cache
```

## Jenkins

Si se utiliza Jenkins, consulte los `Jenkinsfile` dentro de cada servicio para definir pipelines. Algunos ejemplos y Dockerfiles de agentes están en este directorio o en subcarpetas relacionadas.

## Notas

- Este README es intencionalmente breve. Para documentación específica de cada servicio, revise los `README.md` dentro de las carpetas `apps/`, `auth/`, `profiles/`, `architecture/`, etc.
- Mantenga las credenciales fuera del repositorio (use vaults o variables de entorno en CI).

## Contacto

Para dudas sobre pipelines o despliegue, contactar al equipo de infraestructura o al autor del repositorio.

---
Archivo actualizado automáticamente.
