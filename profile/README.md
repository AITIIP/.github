# Git Conventional Commits [![starline](https://starlines.qoo.monster/assets/qoomon/git-conventional-commits)](https://github.com/qoomon/starlines)

Tal como indica su página oficial, Conventional Commits es una especificación para dar significado a los mensajes de commits haciéndolos comprensibles tanto para las máquinas como para las personas. Proporciona un conjunto sencillo de reglas para crear un historial de commits explícito, lo que hace más fácil poder escribir herramientas automatizadas.

Dicha especificación o convención define una serie de reglas para escribir los mensajes de commit que consiguen mejorar la legibilidad del histórico del repositorio y posibilitan tener herramientas que automaticen procesos basados en el historial de commits.

Al poder describir en los mensajes de los commits las funcionalidades, arreglos y cambios de ruptura hechos, esta convención encaja a la perfección con Semantic Versioning o Semver.

La página que se seguirá para los patrones de diseño es la siguiente https://refactoring.guru/

**Se trata de la convención más extendida para establecer un versionado a librerías, paquetes o dependencias, estableciendo tres bloques separados:**

- **MAJOR**: número de versión que se incrementa cuando se rompe la compatibilidad de versiones anteriores.
- **MINOR**: número de versión que se incrementa cuando se añade funcionalidad y esta es compatible en la versión MAJOR actual.
- **PATCH**: número de versión que se incrementa cuando se arreglan errores en la versión MAJOR.MINOR actual.

## Estructura
Según esta especificación, un mensaje de commit debe estructurarse de la siguiente forma:

- **TIPO**: tipo de commit, refiriéndose a su contenido.
- **ÁMBITO**: opcional, sirve para dar información contextual. Ej.: nombre del módulo o paquete
- **DESCRIPCIÓN**: el asunto del commit
- **CUERPO**: opcional, debería aportar más información que la descripción
- **NOTA AL PIE:** opcional, se usa para indicar meta información sobre el commit

## Tipo
Indica el tipo de commit, refiriéndose a su contenido.

La especificación ofrece una guía para los tipos, aunque puede modificarse y/o adaptarse a las necesidades de cada equipo o empresa.

Existen diferentes listas de tipos recomendados, la que más nos gusta es la siguiente:

- **BUILD**: cambios relacionados con la construcción o compilación, por ejemplo, cuando se añaden herramientas externas.
- **CHORE**: un cambio en el código que un usuario externo no verá, por ejemplo, un cambio en el archivo .gitignore
- **FEAT**: una característica nueva
- **FIX**: una corrección de errores
- **DOCS**: cambios relacionados con la documentación
- **REFACTOR**: un cambio que no corrige un error ni añade una característica, por ejemplo, cuando se renombra una variable o función.
- **PERF**: código que mejora el rendimiento
- **STYLE**: un código relacionado con el estilo
- **TEST**: añadir un nuevo test o hacer cambios en un test existente

## Ámbito
El campo ámbito es opcional y sirve para dar información contextual como por ejemplo indicar el nombre del módulo o paquete al que afecta el commit.

Puede ser complicado determinar si se tiene que usar o no, pero en caso de usarse tiene que ir entre paréntesis.

Un listado de posibles ámbitos es:

- THEME
- INIT
- RUNNER
- WATCHER
- CONFIG
- WEB-SERVER
- PROXY

## Descripción
Se trata del asunto del commit, debe cumplir las siguientes reglas:

###### 1. Debemos usar el imperativo en inglés o el infinitivo en español
###### 2. La primera letra siempre irá en minúscula
###### 3. No tenemos que escribir un punto al final
###### 4. El tamaño no debería exceder los 50 caracteres

## Cuerpo
Es opcional y solo se debería añadir si aporta más información que la descripción.

Las reglas para crear la descripción son:

###### 1. Empieza después de una línea en blanco.
###### 2. Se usa el imperativo/infinitivo, al igual que en la descripción
###### 3. Debe tener una anchura máxima de 72 caracteres, aunque se pueden tener múltiples líneas.
###### 4. Solamente debe contener explicaciones de “¿Qué?” (what) y “¿Por Qué?” (why), nunca de ¿Cómo? (How). Esta explicación del “¿Cómo?” se debería hacer en la documentación, si es necesario.

## Nota al pie
Es opcional y se usa para indicar meta información sobre el commit.

Las reglas para la escritura de las notas al pie son:

###### 1. Empieza después de una línea en blanco.
###### 2. Debería usarse en las siguientes situaciones
###### 3. Para indicar cambios que rompan la compatibilidad de la versión actual
###### 4. Para mostrar uno o varios pull-request relacionados
###### 5. Para mostrar los revisores del commit
###### 6. Si se incluyen varios de estos temas, cada uno de ellos en una línea independiente
###### 7. Algunos ejemplos del uso de esta especificación en nuestros proyectos





