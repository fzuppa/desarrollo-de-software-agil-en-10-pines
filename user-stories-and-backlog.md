# **Introducción**

Ya terminamos la fase de _Product Discovery_, que nos permitió tener una visión compartida acerca de lo que deseamos construir y por qué, quiénes serán los usuarios principales y cuál será el modelo de negocios. Ahora, debemos refinar nuestro entendimiento de la funcionalidad detectada, descomponiéndola en ítems o incrementos de funcionalidad, que usaremos, primero para planear y luego para ir construyendo el producto incrementalmente, con el involucramiento cercano de los _product owners_.

Kent Beck bautizó estos incrementos de funcionalidad con el nombre de _user stories_ o historias de usuario. El proceso que imaginó, y plasmó en la metodología _Extreme Programming_, implicaba que los usuarios pensaran la funcionalidad, la escribieran en una tarjeta y esto desencadenara el relato de la ‘historia’ del usuario. Noten que lo importante de todo esto no es la tarjeta, sino la conversación que ésta provoca entre usuarios y desarrolladores para refinar el entendimiento de la funcionalidad.

Por una cuestión de organización y gestión, ‘planchamos’ las _user stories_ descubiertas en una lista priorizada \(que luego estimaremos\) llamada _Product Backlog_. Considero este artefacto esencial para realizar el planeamiento y luego para gestionar el progreso, aunque sé, como contrapartida, que se pierde la visión completa del producto.

En este capítulo ahondaré sobre estas herramientas, describiendo sus características principales, cómo las creamos y cómo las usamos.

# **User Stories**

## **Un Poco de Historia**

**      
**Durante los años 90, Kent Beck \(quizás, la persona más influyente en el nacimiento del mundo de desarrollo ágil?\) sugirió que la manera que usábamos para especificar el producto a desarrollar era tremendamente ineficiente. ¿Qué hacíamos? Una parte del equipo, conformado generalmente por los analistas, intentaba describir mediante un documento, en la fase de Análisis del Proceso del Desarrollo en Cascada, todo lo que el sistema a desarrollar debía contener. Luego, este documento era entregado a los desarrolladores para que empezaran a trabajar a partir de él. ¿Difícil, no? Difícil especificar lo que se tiene que hacer en un documento, que éste sea completo y entender qué hay que hacer a partir del mismo. Beck propuso un cambio radical, paradigmático y revolucionario desde la simplicidad: **que los usuarios de negocio escribieran una tarjeta por cada una de las funcionalidades que deseaban ver en el sistema **y que esa tarjeta fuera el disparador de un **conjunto de conversaciones que sirvieran para clarificar qué se deseaba** o, en otras palabras, para hacer el análisis.

Ron Jeffries capturó los componentes de las _user stories_ en la famosa fórmula de las 3C’s, en inglés: _Card_, _Conversation_ & _Confirmation_ \(en español, sería TCC por Tarjeta\):

* Una tarjeta, tangible, que representa una funcionalidad.

* Una conversación, que se da entre todos los integrantes del equipo, clientes, usuarios, desarrolladores, testers, etc.

* La confirmación, formal, que los objetivos han sido alcanzados.

Así nacieron lo que hoy llamamos _user stories_, que detallaré en las secciones que siguen. Sin embargo, nunca olviden que éstas toman su nombre a partir de cómo deben ser empleadas: **justamente para contar historias!**

## **Atributos de las User Stories**

Antes de contarles cómo escribir _user stories_, les voy a contar algo que considero más importante: cuáles son los atributos que éstas deben poseer. En un rapto de honestidad brutal, les digo que si tienen estos atributos, poco me importa si usan el formato clásico de escritura de user stories!

Las _user stories_ **deben estar escritas en el lenguaje de los usuarios finales**, **deben explicar el que** \(por sobre el como\), **deben contener alguna funcionalidad visible al **_**Product Owner**_ y **deben ser gestionables**.

Profundizo en cada una de estos atributos:

**Escritas en el lenguaje del usuario final**: ¿Queremos entender el dominio que estamos modelando? Entonces ¿qué mejor que describir cada una de estas funcionalidades empleando la jerga de estos usuarios en sus tareas diarias? Esto nos forzará a tener las conversaciones necesarias para entender, en profundidad, cada uno de los conceptos que estamos modelando. Por ejemplo, si estamos construyendo un software para un cajero de supermercados, deberemos entender cómo denominan a cada uno de los productos, qué significa un arqueo de la caja y cualquier otro concepto que forme parte de su área de competencia.

**Deben explicar el que**: Es importante en este momento que se ponga el foco en describir qué es lo que se quiere construir por sobre el como. Esta característica se vuelve fundamental en los casos en que las user stories sean escritas sin el aporte del equipo de desarrollo. Product Owners! No prescindan de un aporte tan fundamental como el del área técnica para el diseño de una solución, porque se perderían de una perspectiva fundamental. Desarrolladores! Si las _user stories_ ya describen la solución, vuelvan un paso atrás y pregunten qué se quiere lograr. Mantengan su cabeza abierta para evaluar otras alternativas.

**Contener Alguna Funcionalidad Visible al **_**Product Owner**_: Debe ser una vista nueva, algún mensaje que reciba \(basado en un conjunto de condiciones\), el envío de un email, etc. Esta característica es fundamental, teniendo en cuenta que emplearemos un proceso de desarrollo iterativo e incremental donde el _Product Owner_ estará involucrado. Hacer incrementos de funcionalidad pequeños para obtener _feedback_ lo más rápido posible es clave. Por supuesto que, para lograr esto, cada funcionalidad que desarrollemos incluirá trabajo en cada una de las capas que formen parte del _stack_ de tecnología que hayamos elegido \(por ejemplo, en una arquitectura clásica contendrá funcionalidad de la vista, el modelo y la base de datos\).

**Gestionables**: Queremos ‘partir’ el trabajo en ítems relativamente pequeños, para entenderlos mejor y para reducir la incertidumbre. El tamaño de estos ítems es bastante subjetivo, ya que depende del equipo, las tecnologías y, quizás, hasta de la duración de la iteración. Para dar una idea, prefiero _user stories_ que puedan terminarse en un lapso comprendido entre 2 y 5 días. Hacer cosas más pequeñas representa demasiado _overhead_ administrativo. Hacer cosas más grandes resulta peor aún, ya que el _feedback_ se hace demasiado lento y puede no haber sensación de progreso. El equipo técnico es quien mejor conoce el esfuerzo requerido para desarrollar una _user story_ y es el que deberá aconsejar partirla si ésta fuese demasiado grande.**      
**

## **Escribiendo User Stories**

**      
**

**Ya sabemos que lasuser storiessirven para contar historias. También enumeramos sus atributos más importantes. Ahora describiré el formato clásico para escribirlas. Sin embargo, no quiero que tomen este formato como una regla que no pueden romper. En mi opinión, ustedes deben buscar el mejor modo de escribirlas en su contexto particular, siempre cumpliendo con los atributos que les mencioné.**

**      
**

**El formato clásico para las user stories es:**

**      
**

**Como &lt;un rol&gt;**

**Deseo &lt;hacer algo&gt;**

**Para &lt;obtener algún valor&gt;**

**      
**

**Por ejemplo, siguiendo con nuestro cajero:**

**      
**

**Como cajero**

**Deseo ingresar un producto manualmente**

**Para seguir con la compra en los casos en que elscannerno funcione**

**      
**

**Éste es el template clásico de escritura de user stories. Noten que está descrita desde la perspectiva de uno de los usuarios finales y constituye alguna funcionalidad que éste empleará. Escribirlas de este modo nos asegura que lo desarrollado será algo visible.**

**La 3ra sentencia, que explica el valor, tiene el objetivo que los usuarios expliquen por qué necesitan esa funcionalidad. En mi experiencia, muchas veces se hace difícil o un poco inútil explicar la razón de una funcionalidad tan pequeña. Creo que uno explica el porqué de módulos grandes de funcionalidad y no el de sus partes.**

**      
**

**Esta breve descripción servirá para tener una idea, superficial, de la funcionalidad esperada aunque probablemente no contenga todos los detalles necesarios para que el equipo pueda empezar a construirla. Tenemos que ampliar la descripción. Para tal fin, usaremos los‘criterios de aceptación’, que no son más que descripciones adicionales, ejemplos de uso, reglas que se deben cumplir o inclusomocksde las pantallas. Cualquier información que ayude a entender la funcionalidad, en el mejor formato \(el más claro\), ‘suma’ dentro de los criterios de aceptación.**

**      
**

**Para agregar un ejemplo, podemos usar este template, tan conocido para los desarrolladores que hacen tests automatizados:**

**      
**

**Given \(dado\)**

**When \(cuando\)**

**Then \(entonces\)**

**      
**

**Es decir, dado un conjunto de precondiciones, cuando ejecutamos cierta acción, deberíamos ver cierto resultado. Escribir los criterios de aceptación de esta manera permite traducirlos en tests automatizados, que pasarán a constituir ‘documentación viva’ \(como lo denominó**[**Gojko Adzik**](https://www.amazon.com/Specification-Example-Successful-Deliver-Software/dp/1617290084)**\).**

**      
**

**Por ejemplo, si quisiera dar un criterio de aceptación que describa qué pasa con el cálculo de todos los ítems, podría especificarlo así:**

**      
**

**Dado que la suma de mis ítems es 100**

**Y el costo de la manteca es 20**

**Cuando ingreso manualmente el código de la manteca**

**Entonces la suma de mis ítems será 120**

**      
**

**A veces, en vez de utilizar un ejemplo, podemos especificar una regla, que nos permita entender qué hacer en cualquier situación. Imaginen que el supermercado aplica un descuento del 10% en la compra de 3 productos iguales.**

**      
**

**El criterio de aceptación podría ser una regla escrita del siguiente modo:**

**      
**

**Si escaneo o ingreso 3 ítems iguales =&gt; aplico 10% sobre esos productos**

**Así, el costo de 3 mantecas será 3\*20 - 6 = $54**

**      
**

**Otras veces, los criterios de aceptación no corresponden a ninguna de estas características o simplemente es mejor describirlos de otra manera. Si tuviera que especificar la funcionalidad para emitir un recibo, que consiste en enviar un conjunto de información a un controlador fiscal, lauser storyconsecuente podría plasmarse del siguiente modo:**

**      
**

**Como cajero**

**Deseo emitir un recibo fiscal**

**      
**

**Y dentro de los criterios de aceptación, debería especificar todos los datos que enviaré:**

**      
**

* **Total**

* **IVA**

* **Descuentos**

**      
**

**Un punto muy importante, cuando escriban los criterios de aceptación, es que todo debería ser lo más concreto posible, desplazarse de la subjetividad. No pueden especificar que algo debe ser rápido, o debe verse bien. ¿Qué implica que algo sea rápido? ¿Qué implica que se vea bien? Todo esto debe estar claramente definido.**

**      
**

**Cuando estamos construyendo una aplicación que tiene una interfase visual \(unaapp webomobile\), la mayoría de lasuser storiestendrán asociadas una vista en la que se desarrollará esta funcionalidad. El mejor modo para describirla es a través de unmockup, que podría ser dibujado a mano \(muchas veces lo hemos realizado junto con el usuario y luego tomada una captura fotográfica\) o ser confeccionado en una herramienta que sirva para este fin como**[**balsamiq**](https://balsamiq.com/)**. Dentro de estosmockupspodemos agregar cualquier descripción que sirva para refinar elscopede la funcionalidad a describir. Retomando el ejemplo del recibo de lauser storyanterior, podríamos haberlo imaginado en unmockup,como el de la imagen que sigue, donde especificamos la información esperada de un modo más visual:**

**      
**

![](https://lh3.googleusercontent.com/YP0UrP5HLq6FxxN5nbJyZ55NQRTe8EpZ89pLVfD4RGSwKyr0UPiEGZnipVhleh1X8fxCe_grH7-4Tc5cmRDO9IfiKhqDLLrkRCuqKSCj59-brHS5JrPQjEQCoMeDF-5-6akjx-bR)

**      
**

**Estemockup, precario \(porque lo hice yo\), tiene toda la información de los criterios mostrados en el ejemplo anterior, de modo más prolijo y con las aclaraciones pertinentes que hacen a lauser storymucho más comprensible. Una imagen vale más que mil palabras. Utilicen esto a su favor.**

**      
**

**Por supuesto que lasuser storiesno tienen que ser la única herramienta de documentación/especificación que usen. A continuación detallo otras que me han resultado muy útiles:**

**      
**

**Workflowde estados: En muchas herramientas que he construido, hemos necesitado describir unworkflowde estados para algunas de las entidades que modelamos. Hacerlo a través de lasuser storiesno hubiera tenido sentido. Es mucho mejor describirlo a través de un gráfico, que contenga los diferentes estados y sus transiciones.**

**      
**

**Flujo de Navegación de Pantallas: podríamos decir que se trata de un caso particular del anterior. Para visualizar la navegación entre las diferentes vistas, lo que hemos hecho es imprimir las pantallas \(una en cada hoja\) para luego vincularlas con flechas, describiendo las situaciones que causan los cambios de pantalla \(Balsamiq permite crear una aplicación para navegar entre las diferentes vistas y testear la usabilidad del producto muy realísticamente\).**

**      
**

**Éstos son ejemplos de herramientas adicionales que usamos para pensar y describir la funcionalidad que deseamos construir y que luego podemos vincular desde lasuser stories.**

**      
**

**Un punto muy importante que quiero mencionarles. Como en el caso del código, la duplicación es mala, ‘the root of all evils in software’, dice ‘Uncle Bob’ Martin ya que se vuelven obsoletas muy rápidamente. Si tuviéramos especificaciones duplicadas, tendríamos una carga mayor de trabajo para mantenerlas actualizadas y correríamos adicionalmente el riesgo de no entender cuál es la última versión.**

**      
**

**Me gustaría cerrar esta sección diciéndoles que, como en cualquier otra parte de su metodología, en la escritura de lasuser stories, ustedes, como equipo, deben ser críticos para refinar este proceso y encontrar el modo más claro y eficiente.**

**      
**

## **Proceso de Descubrimiento**

**      
**

**Paso a contarles cuál es el proceso de descubrimiento y refinamiento de lasuser stories. El resultado del product discovery nos brinda los artefactos que nos sirven como base. En particular, eluser story mappinges muy útil. Partiendo de las tareas que cada uno de los roles ‘hacen’ en el sistema inferimos la funcionalidad necesaria para escribirlas. Ya vimos el caso donde, para la tarea de escaneo manual que habíamos detectado, creamos unauser storypara detallarla con mayor profundidad. También habíamos descubierto que el cajero podía ‘**[**tomar un pago con tarjeta de crédito**](https://docs.google.com/document/d/1WbSA9Wr2Xxk_00sb_hV1P-lBoQC1IYE_LWEvG4Y2Cpc/edit#heading=h.o0pdhqkh7rii)**’. Seguramente, será mejor construir una funcionalidad tan compleja usando múltiplesuser stories, de manera de poder incluir alproduct ownerdurante la construcción y medir el progreso intermedio.**

**      
**

**En este trabajo de descubrimiento inicial, en el que vamos identificando lasuser storiesy las vamos incluyendo en unbackloginicial \(artefacto del que hablaré en breve\), no debemos preocuparnos por entender suscopeexacto,ya queiremos refinándolas a medida que avancemos en la construcción del producto. El objetivo no es comenzar el desarrollo inmediatamente, sino armar unbacklogque describa la funcionalidad más importante, priorizarlo y hacer una estimación que sea usada, posteriormente, al efectuar la planificación del proyecto.**

**      
**

### **\[TOOL\] Example Mapping**

**      
**

**Descubrí esta técnica en la conferencia XP 2016 y la he usado en un par de ocasiones para escribiruser storiesjunto a todo el equipo. Su creador es Matt Wynn. Pueden obtener más información**[**aquí**](https://cucumber.io/blog/2015/12/08/example-mapping-introduction)**.**

**      
**

**La idea de esta herramienta consiste en estructurar la conversación que se da al intentar escribirlas, partiendo de la base de que todas tienen un título, un conjunto de reglas, un conjunto de ejemplos que ayudan a clarificar esas reglas y un conjunto de preguntas abiertas. Utilizamos tarjetas de diferentes colores para cada uno de estos componentes:**

**      
**

* **Título: amarillas**

* **Regla: azules**

* **Ejemplos: verdes**

* **Preguntas: rojas**

**      
**

**Por cadauser story, se construirá un ‘mapa’ usando estas tarjetas, como muestra la imagen que sigue:**

**      
**

![](https://lh5.googleusercontent.com/nazwRXmui_qDxYsFKj5L5D2tnR8HQoshEDBS1zkRAbERQ4V2kjK4Jn_WbiHGJTL3Lsmj-AdlANKwhLtcXSW_e6dB_sNBq5-84CrdZn2VFEeLct0k7fa2dlExpomLbKYOXjZLbATc "map.png")

**      
**

**      
**

**Noten que los colores tienen el objetivo de poder visualizar ciertossmellsen las stories:**

**      
**

* **Muchas tarjetas rojas nos dicen que aún tenemos mucho que aprender.**

* **Muchas tarjetas azules nos dicen que es grande y complicada y quizás convenga partirla.**

* **Muchas tarjetas verdes para una regla nos dicen que quizás se trata de más de una regla.**

**      
**

**En las ocasiones en las que facilité esta actividad, me resultó útil bosquejar las pantallas en la cuáles sucedían estas funcionalidades. Creo que una tarjeta para poder hacer esto sería una buena adición a la herramienta.**

**      
**

**Esta técnica sirve para depurar lasuser storiesde una manera estructurada y efectiva. Si lo hace todo el equipo, repartiéndoselas y luego presentándolas, la actividad puede ser muy enriquecedora.**

**      
**

## **Partiendo User Stories**

**      
**

**Voy a hacer un paréntesis, para contarles sobre uno de los problemas que frecuentemente observo cuandocoacheoequipos externos: Hacer que lasuser storiessean visibles y pequeñas representa, en muchas ocasiones, una dificultad para equipos que recién están comenzando conAgile.**

**      
**

**Suelen decirme, vehementemente, que tenga en cuenta que involucra trabajo en todas las capas, que no es eficiente trabajar así. ¡Además, trabajamos en iteraciones sobre el mismocodebase, agregando funcionalidad, cambiándola y refactorizando todo el tiempo! Puede llegar a sonar ineficiente, pero yo estoy ahí para convencerlos de lo contrario. Se puede trabajar en incrementos pequeños de funcionalidad eficientemente, usando buenas prácticas de desarrollo de software, comoTest Driven DevelopmentyContinuous Refactor.**

**      
**

**Lo que tenemos por ganar es mucho:**

**      
**

* **Recibir elfeedbackde los usuarios del negocio rápidamente.**

* **Medir el progreso del proyecto en base a funcionalidad terminada.**

* **Hacer releases pequeños.**

**      
**

**Trabajar de esta manera requiere cambiar elmindsety pensar enslicesverticales en vez de pensar ensliceshorizontales. Podemos tener en cuenta estas maneras de ‘partir’ las stories cuando nos parezcan demasiado grandes:**

**      
**

* **Partir usando agrupaciones lógicas: Por ejemplo, si incluyera el alta de una persona y de sus datos de facturación, podríamos crear una para el alta de la persona y otra para el alta de sus datos de facturación.**

* **Separar el manejo de las condiciones excepcionales: Escribir una para el ‘camino feliz’ \(sin tener en cuenta las condiciones de error\) y otra para manejar los casos que puedan fallar.**

* **Separar las distintas operaciones: Por ejemplo, hacer una para cada operación de un ABM.**

* **Separar desde la GUI: Es decir, hacer una que contenga la funcionalidad, sin los detalles de diseño, y otra que contemple el diseño.**

* **Hacer unspike: Cuando existe demasiada incertidumbre \(y digo demasiada, porque siempre debemos resolver algo!\), podemos hacer unspikeque sirva para investigar y, posteriormente, lauser storypara hacer el trabajo propiamente dicho.**

**      
**

# **El Backlog**

## **Introducción**

**      
**

**A medida que vamos escribiendo user stories, las almacenamos en una lista, llamadaBacklogde Producto o, simplemente,Backlog, priorizando las más importantes, aquellas que deseamos desarrollar primero en el tope y dejando las de menor importancia al final.**

**      
**

**Cuando empezamos a construir elbacklog, nos focalizamos en descubrir todo el trabajo que tenemos por delante, sin ir a los detalles, haciendo un barrido horizontal de todo el producto y procurando identificar toda su funcionalidad. Hacemos, en este momento también, un trabajo importante de priorización: ¿cuáles son lasuser storiesque forman elcore? ¿Qué es lo más importante para el negocio? ¿Qué es lo más riesgoso? ¿Cuáles son lasuser storiesque debemos construir para edificar la arquitectura de la aplicación?**

**      
**

**Lasuser storiesdelbackloginicial no están refinadas, es decir, no está escrito el detalle de cada una de ellas. Antes de empezar, de la primera iteración, debemos tener un conjunto deuser storiesmínimo que habilite un flujo continuo de trabajo del equipo de desarrollo. Este proceso se va haciendo desde el tope hacia abajo, es decir, desde lasuser storiesmás prioritarias a las menos. No hay un máximo estipulado, pero tengan en cuenta que no deseamos refinarlas si noestamos seguros de ‘consumirlas’ luego.**

**      
**

**Elbacklogno es un artefacto estático, es un artefacto que muta en el transcurso del proyecto. Se modifica para reflejar, en todo momento, nuestro entendimiento del producto que estamos construyendo.**

**      
**

**Todo el equipo trabaja activamente en elbacklog, pero es elproduct owner, la persona que mejor conoce del negocio,quien debe encargarse de gestionarlode modo prolijo. Él procura que lasuser storiesestén bien escritas y de priorizarlas de acuerdo al valor de negocios. Muchas veces, a partir de conversaciones mantenidas entre los miembros del equipo o defeedbackexterno, pueden surgir cambios en funcionalidad que inicialmente se había pensado, que deben reflejarse prolijamente en elbackloga través delproduct owner.**

**      
**

## **¿Qué es el Backlog de Producto?**

**      
**

**Formalizando,el backlog es una lista priorizada y posiblemente estimada de lasuser storiesdel proyecto. Lo utilizamospara almacenar, comunicar, compartir y principalmente gestionar todo el conocimientoque adquirimos durante el transcurso del proyecto, a través de lasuser stories.Es, además, una herramienta de gestión fundamental durante la construcción del sistemaque nos permite visualizar quéuser storiesfueron terminadas, están en desarrollo o quedan por hacer.**

**      
**

## **Atributos Importantes**

**      
**

**Repasemos los atributos más importantes de este artefacto:**

**      
**

**Es un artefacto ‘vivo’: Su vida comienza en la fase de descubrimiento y planeamiento delreleasecon un conjunto de user stories, de las que se posee información superficial. Durante la fase de construcción, cada una de éstas se refinará, es decir, se profundizará el conocimiento delscopehasta contener toda la información necesaria para comenzar a desarrollar. Además, seguramente se descubrirán otras, ya que es imposible detectar toda la funcionalidad de un producto en un momento inicial. Nuestra cabeza no funciona así! Necesita retroalimentación. Observar funcionalidad dispara nuevas ideas, que deben ser plasmadas en nuevasuser stories.También es posible que otras resulten modificadas, repriorizadas o, incluso, eliminadas.El trabajo en elbacklogse extiende durante el transcurso del proyecto.**

**      
**

**Contiene ítems con niveles de refinamiento diferentes: Es decir, con diferentes niveles de entendimiento. Encontraremosuser storiescuyoscopeesté completamente definido y otras que serán simplemente ideas. También encontraremos algunas pequeñas, estimables y otras de gran tamaño, comúnmente llamadas épicas, conviviendo dentro del mismo backlog.**

**      
**

**Es liviano: Es muy fácil agregar, modificar, borrar y priorizaruser stories. Tiene que serlo, ya que el trabajo que se hará sobre él será intensivo.**

**      
**

**\[Se puede hacer un gráfico, que muestre todas estas caracteristicas, juntamente con gente interactuando a traves del backlog, etc\]**

**      
**

## **Herramientas Digitales**

**      
**

**Creo que es fundamental contar con una herramienta digital para la correcta gestión delbacklog, tanto para su conformación, como para la posterior administración del proyecto.**

**      
**

**En 10Pines trabajamos con clientes que utilizan diferentes herramientas como**[**Jira**](https://www.atlassian.com/software/jira)**,**[**VersionOne**](https://www.versionone.com/)**o**[**Pivotal Tracker**](https://www.pivotaltracker.com/)**. Otros clientes tienen su propia herramienta ágil que se adapta exactamente a su metodología, como 8thlight con**[**Artisan**](https://artisan.8thlight.com)**.**

**      
**

![](https://lh5.googleusercontent.com/az75-_H9BJPEve1XDwN5YpcWI7PiXdq_YCIaKRC8eiqHjLeePWy0DHgAYKpHqncFr8OCVVT1eZgg8aYaOrR4lyoYlnohL__tTO7eBUtJubzwXDRELmMUYEzX68vkxM-kVxLXODAt)

**Pivotal Tracker**

**      
**

**Mi herramienta preferida esJiraporque permite visualizar claramente elbacklog, las user stories y losstory boards. Además, elworkflowes configurable y soportaScrumyKanban. Como desventaja, contiene demasiada información en cada vista, lo que dificulta ubicar lo realmente necesario.**

**      
**

**      
**

**\[Agregar imagen de Jira\]**

# **Conclusiones**

**      
**

**Descomponemos el trabajo en un conjunto de incrementos funcionales pequeños, visibles alproduct ownerpara poder involucrarlo en el desarrollo y brindarfeedbacktempranamente. Hacer los incrementos pequeños permite reducir la incertidumbre y medir el progreso frecuentemente. Llamamos a estos incrementosuser stories. Conversar con los usuarios para que éstos nos ‘cuenten’ sus historias resulta esencial. La información procedente de este intercambio no puede compararse con ninguna otra escrita.**

**      
**

**Usamos unbacklogpara gestionar lasuser storiesy para facilitar las conversaciones. Se trata de un artefacto ‘vivo’, que el equipo consultará y modificará durante el transcurso del proyecto.**

