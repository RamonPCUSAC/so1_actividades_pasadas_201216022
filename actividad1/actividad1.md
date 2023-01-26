# ACTIVIDAD 1

## TIPOS DE KERNEL

### Monolíticos

* Abarca todos los servicios del sistema
* Es modular
* Los cambios implementados requieren reiniciar y recompilar el kernel
* Los errores pueden propagarse a la totalidad del kernel

### Micronúcleo

* Contiene un conjunto de llamadas mínimas al sistema
* Las funcionalidades restantes se agregan mediante módulos
* Fácil escalabilidad
* Brindan mayor seguridad que los monolíticos
* Descentralizan los fallos
* Creación y depuración de controladores de dispositivos de manera ágil
* Al poseer varios módulos su sincronización es compleja

### Híbrido
* Arquitectura basada en la combinación de microkernel y núcleo monolítico
* Para mejorar el rendimiento agrega código extra
* Los controladores pueden ser detenidos temporalmente por actividades más relevantes
* Adoptado en la mayoría de sistemas operativos

### Exonúcleo

* Creado con fines de investigación
* El desarrollador tiene permisos para tomar todas las decisiones relativas al rendimiento.
* Limitan sus funciones a la multiplexación y protección de recursos.
* La totalidad de su funcionalidad deja de estar residente en memoria y esta contenida en librerías dinámicas. 

## User mode vs Kernel mode

El user mode se da cuando el sistema operativo ejecuta una aplicación de usuario. Se transiciona del modo usuario al modo kernel cuando la aplicación solicita la ayuda del sistema operativo o se produce una interrupción o una llamada al sistema.

El sistema se inicia en modo kernel cuando arranca y después de cargar el sistema operativo, ejecuta aplicaciones en modo usuario.