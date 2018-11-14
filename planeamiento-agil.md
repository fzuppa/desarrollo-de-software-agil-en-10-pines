# **Introducción**

Ya hicimos el _Product Discovery_ y descubrimos qué se quiere construir y cómo brindará valor el producto. Entendemos mejor qué es lo más importante y también qué se considera indispensable para la primera versión. Escribimos las _user stories_ y las estimamos. Tenemos una idea vaga, por supuesto, del tamaño. **Resta ahora pensar cuál es la mejor manera de construirlo, dadas las restricciones existentes**, que pueden ser de tiempo \(por ejemplo, ¿es necesario que el MVP esté en el mercado para cierta fecha?\) o de dinero \(los clientes cuentan con un presupuesto\).

Es momento de definir un plan, una primera versión de él, que esboce el camino para alcanzar nuestros objetivos. Retomando lo dicho por Marty Cagan: ‘para que un producto sea exitoso, debe ser **valioso, usable y factible de desarrollar**’. Aquí debemos pensar la última parte: ¿Podemos construirlo en los tiempos necesarios y con los recursos con los que contamos? ¿Cómo lo haremos? ¿Qué tecnología usaremos? ¿Quiénes trabajarán en la construcción? ¿Por cuánto tiempo? ¿Cómo atacaremos los riesgos identificados? ¿Cuál será el costo? El plan representa una primera versión de las respuestas a todas estas preguntas y la visión conjunta necesaria, de todo el equipo, para alcanzar estos objetivos.

Un proyecto, según la definición de Johana Rothman en [Manage It!](https://www.amazon.com/Manage-Modern-Pragmatic-Project-Management/dp/0978739248), ‘es un esfuerzo novedoso para crear un nuevo producto o servicio, cuya entrega señala la finalización. Los proyectos implican riesgos y generalmente poseen recursos limitados’. Tiene un _driver_ \(o un conjunto de _drivers_\), una duración específica, marcada por el momento en que se alcanzan los objetivos, y restricciones de tiempo/dinero que los _project managers_ deben gestionar. El plan define el curso de acción del mismo.

Haremos un plan para marcar el rumbo, pero no para seguirlo en detalle, ya que no es nuestro objetivo. Deseamos construir el mejor producto posible. En el libro ‘[Planning Extreme Programming](http://www.informit.com/articles/article.aspx?p=26024)’, Beck y Fowler metaforizan los cambios necesarios durante la ejecución de un proyecto con las ‘constantes correcciones a realizar en el volante, cuando conducimos para mantener el recorrido. Nuestro plan se ajustará, ágilmente, con los cambios que surjan durante la construcción y, principalmente, con todo el aprendizaje que ésta dispare.

En este capítulo hablaremos sobre planeamiento: qué tienen nuestros planes y cuáles son sus características principales. Luego, evaluaremos en detalle las aristas principales englobadas en la gestión de un proyecto, ¿cómo mediremos el éxito? A continuación, detallaré algunas herramientas que permiten visualizar el progreso del mismo. Finalmente, nos ocuparemos de algunas situaciones frecuentes que atentan contra los planes y su ejecución.

# **¿Qué tiene el Plan?**

Componentes esenciales:

**La visión de negocios**: ¿A dónde queremos llegar? ¿Cuáles son los objetivos principales? **Todos debemos compartirlos. En consecuencia, deben quedar claramente plasmados**. Haberlos obtenido a través de las sesiones colaborativas del _product discovery_ simplifica esto enormemente.

**El backlog**: el _backlog_ inicial, que contiene _user stories_ sin mucho detalle. **Representa el entendimiento colectivo de cómo va a descomponerse el trabajo** en incrementos de funcionalidad que después nos permitan trabajar con un proceso de desarrollo iterativo e incremental. Podemos también tener identificadas las _user stories_ que tienen que completarse para el MVP \(de hecho, lo mejor es que el plan corresponda a este grupo solamente\).

**El equipo**: definido en base a las tecnologías que, se prevea, pueden ser usadas \(hasta este momento\), al tamaño de lo que se quiere construir y a las restricciones de tiempo y dinero.**Será multidisciplinario**, es decir, contará con todos los skills necesarios para hacer un incremento de funcionalidad. Además, **las personas estarán asignadas **_**full-time**_ al proyecto.

**El schedule inicial**: En base a las estimaciones realizadas y a la _velocity_ prevista, se puede fijar un _schedule_ inicial. Podrían existir _deadlines_ fijados por el negocio \(por ejemplo, pensando en una presentación o en la competencia\) que deberán ser cumplidos. Estos deben estar bien visibles en el plan, ya que deberemos ajustar otras aristas si la _velocity_ no fuera la esperada.

**Consideraciones tecnológicas**: En el plan, incluimos la visión tecnológica del producto, es decir, el _stack_ de tecnología, las opciones para _hosting_, las herramientas principales, etc. Debe existir una visión tecnológica para alcanzar los objetivos, que será descrita en esta sección.



## **Atributos**

Repasemos los atributos principales de nuestros planes:

* **Está basado en funcionalidades**: El atributo más importante. El plan es, en síntesis, un conjunto de funcionalidades priorizadas. Está pensado para trabajar iterativa e incrementalmente. El progreso se irá midiendo en base a los incrementos completados.

* **Es un artefacto liviano**: Contiene un bosquejo del camino creado a partir de la información de la que disponemos hasta el momento. No se hace futurología, ni se desperdicia tiempo en detalles que puedan ser decididos responsablemente más tarde. Hacer esto volvería al plan más pesado, quitaría tiempo para empezar a construir y daría una falsa sensación de seguridad.

* **Es fácil de cambiar**: Está pensado para ‘abrazar el cambio’. Creamos el plan partiendo de la incertidumbre. Aprenderemos muchísimo durante el camino. Todo este nuevo conocimiento deberá plasmarse en el plan.

* **Es corto**: No creo en planes que duren muchos meses ¿Con cuánto tiempo pueden planear y seguir sintiéndose confidentes?

* **Es creíble**: He visto _project managers_ crear planes con _deadlines_ y _milestones_, para luego transmitir al equipo el ‘cronograma’, ¿qué sentido tiene esto? ¿Podrías, como desarrollador, comprometerte con algo que no creaste y con lo que no crees? El plan debe ser producto de una visión conjunta consensuada.

* **Visible a todo el equipo**: Claramente, si fue creado y consensuado por todos, el plan es accesible a los integrantes en todo momento ¿Podrías alcanzar las metas propuestas, si el equipo no dispone de toda la información?

* **No es un artefacto estático**: Este plan inicial, esbozado a partir del _Product Discovery_ y que contiene mucha incertidumbre aún, se refinará a medida que aprendamos: ¿Es factible tecnológicamente? ¿Podemos construir el producto a la _velocity_ que habíamos estimado previamente? Este nuevo conocimiento, de negocios, tecnológico y del equipo, generado en la etapa de construcción, debe plasmarse en el plan, ya que sería una pena no usarlo a nuestro favor. Por las razones previamente mencionadas, Mike Cohn denominó a su libro ‘[_Estimating & Planning_](https://g.co/kgs/e8NNf4)’. No es un plan. Es planeamiento, continuo. Y Jim Highsmith llamó a esta etapa ‘Especulación’. Es un nombre muy acertado, ya que, en cualquier plan, existe incertidumbre. ‘Cuando especulamos, establecemos un objetivo y una dirección, pero, al mismo tiempo, esperamos cambios en el camino’.



## **Aristas**

Hablemos por unos minutos como _project managers_, para entender las variables que llevan en sus cabezas cuando gestionan un proyecto. En este plan definimos 3 aristas:

* _**Scope**_: El alcance. Los planes ágiles se basan en un conjunto de funcionalidad priorizada.

* **Recursos**: Humanos y monetarios. Estas restricciones determinarán lo que podamos lograr.

* **Tiempos**: El calendario tentativo, incluyendo _milestones_ y _deadlines_, que deben ser tenidos en cuenta para alcanzar los objetivos.

Existe una 4ta arista, la de calidad, que no se especifica en el plan, sino que es el resultado de todos estos factores.

Estas aristas están vinculadas, unas con otras, en modos no lineales. Si alguna de ellas se modifica, alguna de las otras debe modificarse también. Cuando se descubre nueva funcionalidad \(_scope creep_, decían en mi época\), el proyecto claramente implicará más tiempo. Podríamos intentar sumar ‘recursos’ para aumentar la _velocity_, pero los ‘recursos’ son personas, que deben ser entrenadas, con el impacto consecuente sobre el proyecto \(como enunció Fred Brooks en su famosa [Ley de Brooks](https://en.wikipedia.org/wiki/Brooks%27s_law)\). Si no quisiéramos correr la fecha y no sumáramos ‘recursos’, la calidad seguramente se verá afectada.

En mis ‘años mozos’, conocí el [Triángulo de Acero de la Gestión de Proyectos](https://en.wikipedia.org/wiki/Project_management_triangle), un modelo que permitía visualizar estas restricciones: si se ‘tira’ de alguna de las aristas, alguna de las otras deberá moverse forzosamente.

![](https://lh4.googleusercontent.com/H3-34QZ2T0SvSDetM6ei6Gu2ss58fI9Kg2uEoPZ7xd1anR0on8R1V33sKZC1-1zoipbIP5bZ0_yrgZldgynJuyDG7McpA1QzpdjjdQr9zKU4UjV-KiJu9QnPcxAoNDF9knjoevOj)

En el libro de Management 3.0, Jurgen describe el Cuadrado de Acero, incluyendo en la 4ta arista la calidad.



![](https://lh4.googleusercontent.com/krWT3LTEsnNCo8moHT5MpUIGjUev7rlzmbjKScwF8x2iIsOlWoN0OlBs4QJEn_Av4wlBXQ1ksVPb1lSVoXogZOqTOonyqiiKSx3yJovaRG6NiyzziEL-7vFZUUKCzQGaEckASgdj)



La idea del cuadrado de acero es que ‘la modificación de una de las aristas en una dirección tiene un efecto similar en alguna de las aristas adyacentes o el efecto contrario en la opuesta. Por ejemplo: ampliar la funcionalidad implica más recursos o extender la fecha o una calidad inferior \(interna y/o externa\). Una pérdida de recursos llevaría a tener que incluir menos funcionalidad o bajar la calidad o extender el tiempo.

El _project manager_ tiene como objetivo gestionar estas aristas para que el proyecto sea exitoso. La pregunta es: ¿Qué significa que el proyecto sea exitoso? El Standish Group popularizó una métrica errónea, basándose en el cumplimiento de las aristas del triángulo de acero. Así, un proyecto resultaba exitoso en caso de completar el _scope_ planeado a tiempo y con los recursos estimados. Aprendí, a través de Jim Highsmith, que debemos tener en cuenta los factores de negocio al evaluar el resultado ¿Cuánto valor de negocios entregamos? ¿Resolvimos los problemas de los usuarios? ¿Es usable? Las decisiones que tomemos, durante la ejecución del proyecto, deben estar guiadas por estas preguntas. Nuestro objetivo debe ser la construcción de un producto que genere la mayor cantidad de valor de negocios y que sea usable, cumpliendo con las restricciones, es decir, dentro de los tiempos y el presupuesto con el que se cuenta. Con este objetivo en mente, el plan es otro artefacto que nos ayudará a ir decidiendo y visualizando cuál es la mejor manera de lograrlo.

Highsmith sugirió modificar el triángulo de acero para hacerlo compatible con los valores ágiles. Si el objetivo es maximizar el valor de negocios, este debía estar incluido en el triángulo:

**  
**

![](https://lh3.googleusercontent.com/qo75s_6RRSUt8ejH1zt7dZse2fQTDZevaKo9dsWqFt87b_lZ45JTpufRonbqfqa6HGJYCDPBgeifSXY74nVyalu0nAEuGPg786cm6IxZBV9Hgs6gHEOCs7dNdehCBUs1TyQ-XwEr)



Como pueden ver, en una de las aristas se encuentra el valor, en forma de un producto implementable, la 2da equivale a la calidad interna, que permite al producto ser confiable y adaptable, y finalmente la 3ra, conformada por las restricciones \(costo, calendario y _scope_\).

Mike Cottmeyer escribió un [post](https://www.leadingagile.com/2010/01/replacing-the-iron-triangle-of-project-management/) en el que coincide en mover el foco de las restricciones al valor que el producto puede generar, pero no cree que el triángulo sugerido represente correctamente las relaciones entre las diferentes aristas, como sí lo hace el triángulo de acero. Sugiere incluir la calidad y el valor como parte del _scope_, es decir, de la _definition of done_. ¿Estaría algo terminado si el _product owner_ no aceptara su valor o si su calidad fuera pobre?

![](https://lh4.googleusercontent.com/8y3bOYWGsNyZsZweqJjuceZ7qtOao1t-ibibbjQTHClmgasGuPpE4yop4d1WyajzVlghC_z6YOLaiRLMcLKoGpR2cBPIy_n8yYXz5k1slaV6-hmChNRdaUaV1LoTi9116i-Pn3k2)

Personalmente, no logro visualizar las relaciones del triángulo original en ninguna de estas últimas variantes. Creo que entregar la funcionalidad imaginada, con la calidad esperada, es lo que permite generar el beneficio planeado. Si no cumplimos con el presupuesto, no podremos entregar nada. Y si no lo hacemos dentro de los tiempos esperados, otro lo hará. El valor de negocios es un _tradeoff_ complejo entre todas estas aristas y por eso no creo que pueda ser ubicado dentro de ellas.

Para finalizar, detallaré las heurísticas que sigo cuando gestiono un proyecto. El costo es una restricción fija, depende del presupuesto con el que contamos. No es una arista que se pueda modificar. Tampoco lo es la calidad interna. Creo que, en cualquier emprendimiento tecnológico, el _codebase_ debe mantenerse en buena forma, bien diseñado y testeado. De otra manera, no será ni confiable ni extendible. Restan el tiempo y la funcionalidad, aristas que iremos moviendo cual _sliders_, para obtener el mejor producto posible en tiempos razonables.







  


