# Caching Proxy Server CLI

Challenge basado en [Caching Proxy](https://roadmap.sh/projects/caching-server)
Este proyecto es una herramienta de línea de comandos (CLI) que permite iniciar un servidor proxy de
caché. Este servidor intercepta las solicitudes, las redirige al servidor de origen y almacena las
respuestas en caché. Si se realiza la misma solicitud nuevamente, el servidor de caché devuelve la
respuesta almacenada en lugar de reenviar la solicitud al servidor de origen, lo que reduce la
latencia y optimiza el rendimiento.

## Características

* Iniciar el servidor proxy de caché en un puerto específico.
* Redirigir solicitudes a un servidor de origen definido por el usuario.
* Almacenar en caché las respuestas de solicitudes realizadas para que se puedan reutilizar en
  futuras solicitudes idénticas.
* Incluir un encabezado X-Cache en las respuestas para indicar si la respuesta proviene de la
  caché (HIT) o del servidor de origen (MISS).
* Comando para limpiar la caché cuando sea necesario.