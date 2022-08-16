# 1. Monolitos

Aplicacion que funciona como un solo proceso, que lo hace costoso en hardware
y carente de escalabilidad.

# 2. Microservicios

Pueden ser levantados **individualmente** en servidores separados, sin necesidad
de brindales demasiados recursos.

# 3. Arquitectura de Microservicios

La arquitectura basada en microservicios esta alineada a los principios de:

	* Arquitectura impulsada por eventos
	* Arquitectura orientada a servicios

En donde aplicaciones complejas se componen de *pequeños, **independientes** procesos*
que se comunican entre si por medio de un **API**, la cual, a su vez les permite
acceder a otros servicios internos de la misma aplicacion, incluso a servicos de
terceros y monolitos.

Esto provee a los microservicios de, por un lado cierta complejidad en su arquitectura
pero tambien brinda escalabilidad a la aplicacion. Cuando una aplicacion se vuelve modular, cada microservicios puede escalar
individualmente, basado en la demanda de uso.

**No todo monolito puede ser transformado en microservicos**, la solucion para esto
es un refactorizacion, modernizar partes de la aplicacion poco a poco.
Esto trajo consigo otro problema, los modulos podrian generar conflictos al se
desplegados en un mismo servidor.

La mejor solucion a esto fueron los contenedores, entornos aislados y encapsulados
para los modulos. Incluso se podrian levantar varias aplicaciones en un mismo
servidor, cada una con su propio entorno isolado.

4. Contenedores
