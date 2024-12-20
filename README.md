# Docker - Reto parte 1 y 2
## Trabajo Acceso a Datos Docker

### Parte 1
Las tareas para generar nuevas versiones de nuestra imagen docker son repetitivas. Vamos a automatizar el proceso. Para ello abre un chat con ChatGPT e inserta el siguiente prompt:

```
Tengo un repositorio remoto en github con un fichero Dockerfile. Quiero que me muestre paso a paso como puedo automatizar la publicacion de esas imagenes en dockerhub haciendo uso de github actions. Muestra detalles de como crear y configurar la cuenta en docker hub y como obtener un token de acceso y como guardarlos de manera segura en github.  Muestra como crear un tag. Quiero que el trigger lo dispare cuando creo un tag sobre el repositorio. La imagen que suba a docker hub, tiene que tener como versión el contenido de ese tag. En el ejemplo, supongo que el tag es v3.
```

Realiza todos los pasos necesarios y genera una nueva versión en DockerHub. Ahora en tu máquina, ejecuta docker run -d -p 80:80 <usuario>/<imagen>:<version> para arrancar un servicio web con todos los cambios que incluya la versión publicada.

Pasos:

    - Crear un repositorio en Docker hub
    - Crear un token y añadirlo a GitHub secrets
    - Crear un archivo .yaml con el script de GitHub Actions

### Parte 2

El reto consistirá en generar otro contenedor workspace para otro framework. Puedes elegir entre frameworks frontend: VueJs, angular, React o backend: SpringBoot, Django. Se debe entregar a través del Aula Virtual los enlaces a un contenedor disponible a través de DockerHub y un repositorio público en GitHub con el Dockerfile y una carpeta del proyecto.
