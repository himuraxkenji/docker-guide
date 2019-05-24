# ¿Qué es Docker?

**Docker** es una herramienta de Código Abierto que nos permite realizar una ***"virtualización ligera"***. Se puede empaquetar entornos y aplicaciones para posterior despliegue.
Para ello Docker extiende de LXC (LinuX Containers), un sistema de virtualización que permite crear múltiples sistemas totalmente aislados entre sí, sobre la misma máquina o sistema anfitrión.
Docker utiliza características de aislamiento de recursos del kernel Linux, tales como cgroups y espacios de nombres (namespaces) para permitir que ***"contenedores"*** independientes se ejecuten dentro de una sola instancia de Linux, evitando la sobrecarga de iniciar y mantener máquinas virtuales.
Docker es una herramienta que puede empaquetar una aplicación y sus dependencias en un contenedor virtual que se puede ejecutar en cualquier servidor Linux. Esto ayuda a permitir la flexibilidad y portabilidad en donde la aplicación se puede ejecutar, ya sea en las instalaciones físicas, la nube pública, nube privada, etc.
Docker se emplean dos términos, las imágenes y los Contenedores. Las imágenes en Docker se podrían ver como un componente estático, pues no son más que un sistema operativo base, con un conjunto de aplicaciones empaquetadas, mientras que un contenedor es la instancia o ejecución de una imagen, pudiendo ejecutar varios contenedores a partir de una misma imagen.

# Docker VS Máquinas Virtuales
La principal diferencia es que una máquina virtual necesita contener todo el sistema operativo mientras que un contenedor Docker aprovecha el sistema operativo sobre el cual se ejecuta, por lo tanto, comparte el núcleo del sistema operativo anfitrión e incluso las librerías. De esta manera podemos arrancar o parar el contenedor rápidamente, mientras que máquinas virtuales, como Vmware, Citrix o Virtualbox, se aíslan del sistema operativo sobre el que trabajan y se comunican a través del hypervisor.
