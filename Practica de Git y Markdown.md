# Practica de Git y Markdown



## INDICE:
```
- ¿Qué es git?

- Rendimiento

- Seguridad

- Flexibilidad

```

## **CONTENIDO**


 ###  **¿Qué es git?**
 ```


Hoy en día, Git es, con diferencia, el sistema de control de versiones moderno más utilizado del mundo. Git es un proyecto de código abierto maduro y con un mantenimiento activo que desarrolló originalmente Linus Torvalds, el famoso creador del kernel del sistema operativo Linux, en 2005. Un asombroso número de proyectos de software dependen de Git para el control de versiones, incluidos proyectos comerciales y de código abierto. Los desarrolladores que han trabajado con Git cuentan con una buena representación en la base de talentos disponibles para el desarrollo de software, y este sistema funciona a la perfección en una amplia variedad de sistemas operativos e IDE (entornos de desarrollo integrados).
```

###  **Rendimiento**

```
Las características básicas de rendimiento de Git son muy sólidas en comparación con muchas otras alternativas. La confirmación de nuevos cambios, la ramificación, la fusión y la comparación de versiones anteriores se han optimizado en favor del rendimiento. Los algoritmos implementados en Git aprovechan el profundo conocimiento sobre los atributos comunes de los auténticos árboles de archivos de código fuente, cómo suelen modificarse con el paso del tiempo y cuáles son los patrones de acceso.

A diferencia de algunos programas de software de control de versiones, Git no se deja engañar por los nombres de los archivos a la hora de determinar cuál debería ser el almacenamiento y el historial de versiones del árbol de archivos; en lugar de ello, se centra en el contenido del propio archivo. Al fin y al cabo, los archivos de código fuente se cambian de nombre, se dividen y se reorganizan con frecuencia. El formato de objeto de los archivos del repositorio de Git emplea una combinación de codificación delta (que almacena las diferencias de contenido) y compresión, y guarda explícitamente el contenido de los directorios y los objetos de metadatos de las versiones.
```
### **Seguridad**

```
Git se ha diseñado con la principal prioridad de conservar la integridad del código fuente gestionado. El contenido de los archivos y las verdaderas relaciones entre estos y los directorios, las versiones, las etiquetas y las confirmaciones, todos ellos objetos del repositorio de Git, están protegidos con un algoritmo de hash criptográficamente seguro llamado "SHA1". De este modo, se salvaguarda el código y el historial de cambios frente a las modificaciones accidentales y maliciosas, y se garantiza que el historial sea totalmente trazable.

Con Git, puedes tener la certeza de contar con un auténtico historial de contenido de tu código fuente.

Algunos otros sistemas de control de versiones carecen de protección contra las modificaciones ocultas realizadas con posterioridad, algo que puede suponer una grave vulnerabilidad de seguridad de la información para cualquier organización que se base en el desarrollo de software.
```

### **Flexibilidad**

```
Uno de los objetivos clave de Git en cuanto al diseño es la flexibilidad. Git es flexible en varios aspectos: en la capacidad para varios tipos de flujos de trabajo de desarrollo no lineal, en su eficiencia en proyectos tanto grandes como pequeños y en su compatibilidad con numerosos sistemas y protocolos.

Git se ha ideado para posibilitar la ramificación y el etiquetado como procesos de primera importancia (a diferencia de SVN) y las operaciones que afectan a las ramas y las etiquetas (como la fusión o la reversión) también se almacenan en el historial de cambios. No todos los sistemas de control de versiones ofrecen este nivel de seguimiento.
```




## **GLOSARIO**

### **repository**
```
Un repositorio es el elemento más básico de GitHub. Es más fácil imaginarlos como carpetas de proyecto. Un repositorio contiene todos los archivos de un proyecto (incluyendo la documentación), y almacena el histórico de modificaciones de cada archivo. Los repositorios pueden tener múltiples colaboradores y pueden ser tanto públicos como privados.
```


### **commit**
```
Un commit se puede entender como la confirmación de una modificación individual en un archivo (o serie de archivos). Es como cuando guardas un archivo, excepto que con Git, cada vez que haces commit se crea un ID único (también conocido como SHA o hash) que te permite registrar qué cambios se hicieron y quién los hizo. Los commits generalmente contienen un mensaje de commit que consiste en una breve descripción de los cambios realizados.
```


### **push**
```
Literalmente, empujar. Se refiere a enviar tus cambios confirmados (tus commits) a un repositorio remoto, como por ejemplo un repositorio alojado en GitHub. Si cambias algo localmente, querrás hacer push de esos cambios para que los demás miembros de tu equipo puedan acceder a ellos.
```


### **pull**
```
Literalmente, tirar. Se refiere a traer los cambios del servidor remoto y combinarlos con tu copia local. Por ejemplo, si alguien ha editado el archivo remoto en el que ambos estáis trabajando, querrás hacer pull de esos cambios a tu copia local para que esté actualizada.
```


### **issue**
```
Los issues son sugerencias de mejora, tareas o cuestiones relacionadas con el repositorio o el proyecto. Cualquiera puede crear issues (en un repositorio público), y los moderan los colaboradores del repositorio. Cada issue contiene su propio foro de dissusión, y se puede etiquetar y asignar a un usuario.
```


### **pull request**
```
Los pull requests o, literalmente, solicitudes de tirar, son cambios propuestos para un repositorio que un usuario ha enviado, y que pueden ser aceptados o rechazados por los colaboradores del repositorio. Igual que los issues, los pull requests tienen cada uno su propio foro de discusión.
```


### **branch**
```
Un branch o, literalmente, rama, es una versión paralela de un repositorio. Está contenido dentro del repositorio, pero no afecta al branch principal o master, permitiéndote trabajar libremente sin estropear la versión “real”. Cuando has terminado de realizar los cambios que querías hacer, puedes hacer merge de tu branch al branch principal para publicar tus cambios.
```


### **merge**
```
Literalmente, combinar. Hacer merge toma los cambios de un branch (en el mismo repositorio o también desde un fork), y los aplica en otro. Esto a menudo ocurre como un pull request (que se puede entender como una solicitud de hacer merge), o a través de la línea de comandos. Un merge puede realizarse automáticamente a través de un pull request en la interfaz web de GitHub siempre y cuando no haya cambios que generen conflictos, o puede hacerse siempre via línea de comandos.
```


### **remote**
```
La versión remota es una versión de algo que está alojada en un servidor, muy probablemente GitHub en este contexto. Puede estar conectado a clones locales de forma que los cambios se sincronicen.
```


### **local**
```
La versión local es la copia que tienes del repositorio en tu ordenador, sobre la que trabajas.
```


### **clone**
```
Un clon es la copia de un repositorio que se aloja en tu ordenador, en lugar de en un servidor en alguna parte, o el acto de realizar esa copia. En tu clone puedes editar los archivos en tu editor preferido y utilizar Git para llevar un registro de esas modificaciones sin necesidad de tener conexión a internet. Sin embargo, este clon está conectado a la versión remota de forma que los cambios se puedan sincronizar entre ambos. Puedes hacer push de tus cambios locales a la versión remota para mantenerlas sincronizadas cuando estés online.
```


### **fork**
```
Un fork o, literalmente, tenedor, es una copia personal de un repositorio de otro usuario que se aloja en tu cuenta. Los forks te permiten modificar libremente cualquier proyecto sin alterar el original. Los forks se mantienen relacionados con el original, de manera que puedes enviar un pull request al autor del repositorio original para que lo actualice con tus cambios. También puedes mantener tu fork actualizado haciendo pull de las modificaciones del original.
```