# Arquitectura monolitica vs microservicios:computer:
## Definicion
### Arquitectura monolitica
La arquitectura monolítica implica la creación de una aplicación autónoma que contenga absolutamente toda la funcionalidad que necesita para realizar tareas de diseño, sin dependencias externas que agreguen a su funcionalidad.
### Arquitectura microservicios
La arquitectura de microservicios es un método para desarrollar aplicaciones de software que brindan una funcionalidad comercial completa como una colección de pequeños servicios que operan de forma independiente y autónoma.
![ImagenMonovsMicro](https://nutech.lat/wp-content/uploads/2021/07/Monolitico-vs-Microservicios.jpg)
> Tech, N. (2021, 26 julio). Monoliticos vs Microservicios [Comparacion]. https://nutech.lat/migrar-de-una-arquitectura-monolitica-a-una-arquitectura-de-microservicios-mejores-practicas/
## Caracteristicas
### Arquitectura monolitica
1. Son aplicaciones autosuficientes.
2. Realizan de punta a punta todas las operaciones para terminar una tarea.
3. Son por lo general aplicaciones grandes.
4. Son por lo general silos de datos privados, cada instalación administra su propia base de datos.
5. Todo el sistema corre sobre una solo plataforma.
### Arquitectura microservicios
1. Alto nivel de desacoplamiento.
2. Nombres únicos.
3. En caso de que den algún problema, pueden iniciarse en otra máquina de forma que así no perderemos ningún dato ni información.
4. Su implementación, escalado y actualización se hace de manera independiente.
5. Están enfocados para desarrollarse en función de cada negocio o de cada cliente.
## Ventajas y desventajas
### Arquitectura monolitica
#### Ventajas :+1:
- Fácil para un equipo pequeño de desarrollo iniciar un nuevo proyecto y ponerlo en producción rápidamente.
- Fácil de escalar.
- El hecho de no depender de nadie más, mitiga gran parte de los errores de comunicación, red, integraciones, etc.
- Al ser autonomo permite funcionar independientemente del resto de aplicaciones.
- Las aplicaciones Monolíticas son significativamente más rápidas debido que todo el procesamiento lo realizan localmente.
- Toda la funcionalidad está disponible desde el principio de la aplicación, por lo que puede ejecutar todas las pruebas necesarias sin depender de nada más.
#### Desventajas:-1:
- Dado que todo el software es una sola pieza, significa que se usa el mismo conjunto de tecnologías para todo, eliminando el uso de otras tecnologías.
- Escalar una aplicación monolítica significa escalar toda la aplicación usando recursos para la funcionalidad que puede que no necesite ser escalada.
- Las aplicaciones monolíticas son fáciles de ejecutar en equipos pequeños, pero a medida que crece la aplicación y crece el equipo de desarrollo, se vuelve cada vez más difícil dividir el trabajo sin comprometer la funcionalidad.
- Cualquier mínimo cambio en la aplicación implicará realizar una compilación del todo el artefacto y con ello una nueva versión que tendrá que ser administrada.
- A menos que se tenga alta disponibilidad, si la aplicación Monolítica falla, falla todo el sistema, quedando totalmente inoperable.
- En proyectos muy grandes, puede ser abrumador para un nuevo programador hacer un cambio en el sistema.
### Arquitectura microservicios
#### Ventajas:+1:
- Al tratarse de servicios autónomos, se pueden desarrollar y desplegar de forma independiente. Además un error en un servicio no debería afectar la capacidad de otros servicios para seguir trabajando según lo previsto.
- Como es una aplicación modular, se puede escalar horizontalmente cada parte según sea necesario, aumentando el escalado de los módulos que tengan un procesamiento más intensivo.
- Se pueden usar diferentes tecnologías y lenguajes de programación. Lo que permite adaptar cada funcionalidad a la tecnología más adecuada y rentable.
- El reducido tamaño de los microservicios permite un desarrollo menos costoso, así como el uso de “contenedores de software” permite que el despliegue de la aplicación se pueda llevar a cabo rápidamente.
- Al poder hacerse mejoras de un solo módulo y no tener que intervenir en toda la estructura, el mantenimiento es más sencillo y barato que en otras arquitecturas.
- Se pueden utilizar funcionalidades típicas (autenticación, trazabilidad, etc.) que ya han sido desarrolladas por terceros.
#### Desventajas:-1:
- Al tener cada microservicio sus propios recursos y bases de datos, consumen más memoria y CPU.
- Al crear la arquitectura, se necesita más tiempo para poder fragmentar los distintos microservicios e implementar la comunicación entre ellos.
- Los microservicios requieren desarrolladores experimentados con un nivel muy alto de experiencia y un control exhaustivo de las versiones. Además de conocimiento sobre solución de problemas como latencia en la red o balanceo de cargas.
- Aunque disponer de un equipo tecnológico diferente para cada uno de los servicios tiene sus ventajas, si no se gestiona correctamente, conducirá a un diseño y arquitectura de aplicación poco uniforme.
- Debido a que los componentes de la aplicación están distribuidos, las pruebas y test globales son más complicados de realizar.
- Una arquitectura de microservicios puede suponer un alto coste de implantación debido a costes de infraestructura y pruebas distribuidas.
## Comparacion :coffee:
![Compa](https://i0.wp.com/msaffirio.com/wp-content/uploads/2018/11/microservicios-vs-monolitico.png?resize=900%2C547&ssl=1)
> Safirio, M. (2018, 3 diciembre). Comparacion [Imagen]. https://i0.wp.com/msaffirio.com/wp-content/uploads/2018/11/microservicios-vs-monolitico.png?resize=900%2C547&ssl=1
## Casos de aplicabilidad
### Arquitectura monolitica
Algunos ejemplos pueden ser áreas comunes como la gestión de archivos de medios o externos, la autenticación con sistemas externos, los sistemas de notificaciones, funciones específicas de negocio en una aplicación tradicional.
### Arquitectura microservicios
- Netflix : Esta plataforma tiene una arquitectura generalizada que desde hace ya un par de años, se pasó a los microservicios para el funcionamiento de sus productos.
- Amazon : Migró hace tres años a la arquitectura de microservicios siendo una de las primeras grandes compañías que la implementaban en producción.
## Fuentes
- Nuñez, E. A. (2020, 4 junio). Qué son Microservicios y ejemplos reales de uso. OpenWebinars.net. https://openwebinars.net/blog/microservicios-que-son/
- Arquitectura de Monolítico. (2020). reactive programming. Recuperado 3 de septiembre de 2022, de https://reactiveprogramming.io/blog/es/estilos-arquitectonicos/monolitico
