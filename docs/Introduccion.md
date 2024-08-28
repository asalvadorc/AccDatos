# Introducción

¿A qué nos referimos cuando hablamos de **acceso a datos** en una aplicación informática?

Podemos afirmar que en la inmensa mayoría de aplicaciones informáticas se pueden diferenciar, a grandes rasgos, en dos partes:

- Por un lado, el programa propiamente dicho, que realiza las operaciones deseadas con los datos necesarios.
- Por otro lado, los datos con los que opera le programa. Esos datos pueden ser obtenidos por el programa mediante diversos métodos: leídos mediante teclado, escaneados, leídos de algún soporte de almacenamiento secundario, etc.
En la mayoría de los casos, cuando programamos, nos interesa que el programa guarde los datos que le hemos introducido, o los resultados que dicho programa haya obtenido, de manera que si el programa termina su ejecución, los datos no se pierdan y puedan ser recuperados posteriormente, es decir, persistan. Una forma tradicional de hacer esto es mediante la utilización de ficheros o de bases de datos que se guardarán en un dispositivo de memoria no volátil (normalmente un disco).

Te habrás dado cuenta de que el almacenamiento en memoria RAM, mediante variables o vectores, es temporal, los datos se pierden cuando el programa termina. Quizás te habrá pasado alguna vez que, debido a un apagón eléctrico, has perdido el trabajo que estabas haciendo, que todavía no habías grabado. Los datos que se guardan en almacenamiento secundario, como ficheros o bases de datos, se denominan datos persistentes, porque existen, o persisten más allá de la ejecución de la aplicación.

Ese almacenamiento secundario de datos que acabamos de mencionar, habitualmente suele consistir en una base de datos relacional, si bien, a veces, hay otros métodos de almacenamiento, y por tanto, métodos de acceso a esos datos. De conocer esos tipos de almacenamiento y cómo acceder a ellos es de lo que trata este módulo.

En esta unidad inicial, vas a ver una panorámica de los diversos métodos de persistencia que encontramos en el mercado.

# Acceso a Datos

Hay diversas estrategias de acceso a datos para gestionar la persistencia de los datos:

- Mediante ficheros.
- Bases de datos, que pueden ser:
Relacionales, Orientadas a objetos,
Objeto-relacionales.
- Mapeo objeto relacional (ORM).
- Bases de datos XML (eXtensible Markup Language).
- Componentes.

Al principio, en los primeros tiempos de la informática, los datos se guardaban en ficheros convencionales. Con el tiempo, y la experiencia de trabajar con dichos ficheros, se observaron los inconvenientes de los ficheros, y para intentar solucionar los inconvenientes que se observaron surgieron las bases de datos, que entre otras ventajas permitían:

- Eliminar el problema de la información redundante.
- Eliminar información inconsistente.
- Globalizar o centralizar la información.
- Garantizar el mantenimiento de la integridad en la información. Únicamente se almacena la información correcta.
- Independencia de datos. La independencia de datos implica una separación entre programas y datos, es decir, se pueden hacer cambios en la información que contiene la base de datos, o tener acceso a la base de datos de diferente manera, sin tener que hacer cambios en las aplicaciones o en los programas.

## Qué estrategia o método de acceso a datos usar.

Posteriormente, con la aparición y expansión de la programación orientada a objetos, empezaron a surgir las Bases de datos orientadas a objetos, y también se ampliaron algunas bases de datos relacionales, añadiéndoles extensiones de orientación a objetos.

Entonces ¿qué método de acceso a datos es mejor? ¿Cuál deberías utilizar en la próxima aplicación que construyas?

Pues..., no hay una respuesta fácil para esas preguntas, no se puede afirmar que haya un método que sea el mejor de manera absoluta. Más bien, la cuestión es tener claro qué tipo de aplicación hay que construir y, según eso, estudiar qué tipo de sistema de almacenamiento será mejor usar: si una base de datos orientada a objetos, o una base de datos XML, etc.

Conociendo el funcionamiento de las diferentes alternativas podemos comparar sus prestaciones al problema de la persistencia concreto que se nos presente. Cada una de las tecnologías tiene su propio origen y filosofía para alcanzar el mismo fin y, por esta razón, no es fácil analizar sus ventajas y desventajas frente a las demás alternativas.

Por poner un ejemplo, lo más sencillo posible: si voy a crear una base de datos para guardar mi colección de vídeos, probablemente no me va a interesar utilizar una base de datos Oracle, sino un producto mucho más barato, y sencillo de instalar y mantener.

