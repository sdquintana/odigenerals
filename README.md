# odigenerals
pregunstas basicas odi



**PREGUNTAS TÉCNICAS**

Indicaciones

Contesta las siguientes preguntas, lo más breve posible

Gracias

1.Diferencia entre ETL y ELT.

El proceso de integración tradicional etl consiste en realizar las cargas en 3 pasos, extraer, transformar dentro en una etapa intermedia los datos y finalmente integrarlos en una fuente, mientras que el proceso E-LT altera un poco los pasos para realizar una extracción de la fuente y una carga y transformación en el mismo destino.


2.Secciones del ODI Studio.

- **Topology** : se encarga de administras las conexiones a los servidores de datos y la asociación de schemas lógicos y físicos con el contexto.

- **Designer** : es la sección donde se encuentra el desarrollo. Encontraremos variables, procedimientos, escenarios, mappings (interfaces en la versión 11g o menores), modelos y módulos de conocimiento.

- **Operator** : es la sección donde se visualiza el estatus de las ejecuciones de cualquiera de los objetos.

3.Tipos de Repositorios.

- **Master** : se encuentran la información de la topología, seguridad y metadatos que necesita ODI.

- **Work** : contiene información del desarrollo como es los proyectos, modelos, variables, ejecuciones de objetos. En caso de que el repositorio sea de tipo ejecución solo contiene información de los scenarios y las ejecuciones.

4. Tipos de Esquemas o topologías.

- **Lógico** : es una representación de la conexión que usaremos.

- **Físico** : con tiene la conexión directa con el servidor de datos.

Nota: La relación de los esquemas es a través del contexto el cual nos indicará que conexión física (url de base de datos) está ligada al esquema físico



5. **¿Qué es un agente?**

Es el encargado de orquestar las ejecuciones de escenarios y load plans.

Un agente puede ser local o por medio de un webservice dependiendo de la instalación del ambiente.

6. **¿Qué es un modelo de datos en ODI?**

Un modelo es el conjunto de data source (fuentes de datos) que están basadas en una misma tecnología, como puede ser archivos planos, base de datos oracle, sql server, xml, etc.



7. **¿Qué es y para qué sirve un módulo de conocimiento?**

Son con conjunto de instrucciones base, las cuales contienen código general para realizar integraciones de datos. El código que utiliza es groovy y el api de odi (sunopsis api) el cual nos ayuda a manipular el metadata de los modelos e indicar que tipo de integración de datos realizaremos



8. **¿Qué es y para qué sirve un escenario?**

Un escenario es una unidad de ejecución que puede contener uno o más pasos a ejecutar de un objeto odi.

El escenario es el ejecutable compilado de odi en términos coloquiales por lo cual nos sirve para poder realizar ejecuciones  a través del agente.


9. **Tipos de objetos que existen en ODI**

- Variables
- Mappings(interfaces en la versión 11g o menores)
- Procedimientos
- User funcions
- Paquetes
- Scenarios
- Modelos
- Data stores



10. **¿Qué es una interfaz?**

Es el objeto que nos indica la lógica de como haremos las extracciones y transformaciones de datos para poder cargar información de una fuente de datos hacia otra.

En la versión 11g o anteriores se llamaban interfaces en odi 12c estos objetos se renuevan y adoptan el nombre de mappings
