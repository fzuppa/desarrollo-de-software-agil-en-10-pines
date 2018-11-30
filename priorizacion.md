# ![](/assets/Priorizaciones.png)

# **Saber qué es lo importante es lo importante**

** **Un consultor amigo siempre decía que las metodologías ágiles no son más que un compendio de prácticas para reducir el riesgo. En este sentido,desarrollar las funcionalidades más importantes primero es fundamental, ya que muy probablemente el dinero no alcance para todas las que el cliente desea. Al usar un proceso de desarrollo iterativo e incremental, podemos hacer _releases_ tempranos que las implementen, dejando el resto para otros posteriores. De esta manera, optimizamos el retorno de inversión y minimizamos el riesgo del proyecto.

¿Cuál es la funcionalidad más importante? Elproduct ownery todas las personas vinculadas al negocio, seguramente,conocen mejor la funcionalidad que aporta más valor. En otras palabras, la que generará mayores ingresos resolverá más problemas u optimizará los procesos más importantes. Este no es el único factor que debemos tener en cuenta al priorizar. Otro, sumamente importante, es el riesgo tecnológico. Debemos ‘atacar’ rápidamente todas las áreas tecnológicas que provoquen mayor incertidumbre, ya que, si no pudiésemos resolver los problemas del modo imaginado, esto podría provocar que el producto final no aportase el valor de negocios inicialmente esperado.Reducir el riesgo tecnológico también es un factor preponderante a la hora de priorizar.

Es importante que todo el equipo colabore en la priorización del producto. Elproduct ownerserá, sin embargo, el actor más importante, quien determine lo que el negocio espera. Por su parte, el equipo técnico debe colaborar activamente, identificando los riesgos tecnológicos y las dependencias.La priorización, así como el diseño, debe ser el resultado de la colaboración del equipoen pos de un objetivo compartido.

El trabajo de priorización no concluye con la escritura delbacklogpreliminar. Desde el inicio de su construcción, se genera conocimiento que puede impactar en la prioridad de las funcionalidades planeadas. También pueden tener lugar eventos externos \(como un anuncio de un competidor o un cambio en un proveedor\) que modifiquen nuestro plan. Elbacklogserá la herramienta utilizada para reflejar todas las decisiones de priorización tomadas durante el transcurso del proyecto.

En este capítulo, trataremos principalmente la priorización dentro del contexto de desarrollo de un producto nuevo, transmitiendo los factores a tener en cuenta y algunas herramientas utilizadas.

## **¿Qué debe tenerse en cuenta al priorizar?**

El factor más importante es el valor de negocios, que, en su acepción más sencilla, implica cuánto dinero ganaremos. Sin embargo, este podría no llegar a ser tan directo. Existen otras aristas que influyen, como ganar nuevos clientes o una porción de mercado donde no existan otros competidores. En definitiva, el valor de negocios que una funcionalidad entrega es el beneficio que la organización obtiene a partir de él. Nuestro objetivo debe ser maximizarlo.

El 2do factor a tener en cuenta es el riesgo tecnológico. Si existieran componentes,frameworkso servicios que no sabemos como funcionan, es importante despejar esta incertidumbre lo más rápido posible. No deseamos progresar en el desarrollo del producto para luego darnos cuenta de que algo no va a funcionar y que, en consecuencia, el valor entregado sea inferior al esperado. En el mundo ágil dicen falla rápido \(‘fail fast’\) o, para decirlo en otras palabras tomadas de Alistair Cockburn, aprende rápido \(‘learn fast’\).

Otra perspectiva desde la que podemos mirar este tópico de priorización es la del aprendizaje. Estamos aprendiendo y debemos lidiar con riesgos e incertidumbres. En consecuencia, deberíamos priorizar todo aquello que nos permita incrementarlo.

Otro factor que podríamos llegar a tener en cuenta, aunque de menor importancia, es el esfuerzo \(o costo\). Conociéndolo, elproduct ownerpodrá decidir que una funcionalidad es demasiado costosa para el valor que arroja o, por el contrario, construir otra menos valiosa, solamente porque el esfuerzo requerido es menor. Para ponerlo en términos formales, la razón costo-beneficio puede influir en la priorización.

Ninguno de estos factores decide la priorización por sí mismo, ya que tanto los de negocios, como los tecnológicos, deben ser tenidos en cuenta. Como ya mencioné anteriormente, las decisiones de priorización serán el resultado de la colaboraciónentre todos los miembros del equipo.

## **Releases Cortos**

Antes de interiorizarnos en muchas de las herramientas utilizadas, les mostraré la heurística más importante a la hora de priorizar y de planear. Acoten, tanto como sea posible, la cantidad de trabajo. En otras palabras, en lugar de hacerreleasesgrandes y riesgosos, háganlos simples y breves. Les resumo las ventajas que obtendrán:

* Maximiza el retorno de inversión del proyecto: desde el punto de vista financiero, no hay dudas de que es sumamente beneficioso, ya que, en un periodo de tiempo mucho menor, obtendremos parte del valor de negocios prometido \(que puede ser usado para financiar el resto del proyecto\).

* Minimiza el riesgo: Tener mucho trabajo en progreso representa un riesgo, porque las condiciones \(internas o externas\) pueden cambiar. Al construir el MVP, debemos acotar estereleaseal mínimo posible, para testear la hipótesis única de valor \(que tiene un riesgo muy grande\) al menor costo posible.

* Minimiza la incertidumbre: No olvidemos que, antes de construir el producto y testearlo con usuarios reales, solo hipotetizamos. Testear el producto nos ayudará a despejar muchas de las incógnitas existentes.

Verán menciones a esta heurística en toda la literatura ágil. Kent Beck incluyó, entre las reglas de planeamiento deExtreme Programming, una que denominó ‘[releasescortos y frecuentes](http://www.extremeprogramming.org/rules/releaseoften.html)’. Probablemente fue quien luego propició uno de los[principios ágiles](http://agilemanifesto.org/principles.html)que afirma: ‘buscamos satisfacer a los clientes a través de la entrega continua de software con valor’. La[declaración de interdependencia](http://pmdoi.org/), escrita porproject managers, específica que ‘se aumenta el retorno de inversión, haciendo foco en tener un flujo continuo de valor’. Las reglas de[Lean Software Development](https://en.wikipedia.org/wiki/Lean_software_development)van en la misma dirección. Una de ellas proclama: ‘debemos entregar software rápidamente, ya que implica una ventaja competitiva’. Finalmente,[Kanban](https://www.crisp.se/gratis-material-och-guider/kanban)hace de todo esto su leitmotiv. Sus reglas principales comprenden ‘visualizar el flujo de valor’, para ‘limitar el trabajo en progreso’ y, de esta manera, ‘maximizarlo’.

En estos días, muchos de nuestros clientes, que ya poseen un producto en funcionamiento, usan[continuous delivery](https://continuousdelivery.com/). El precepto es el mismo. De este modo, agregan valor diariamente o, incluso, varias veces en un día. Losreleasespequeños y frecuentes de los que hablaba Beck en los años 90 se llevaron al extremo.

Ahora sí, veamos algunas de las herramientas que usamos frecuente en distintas etapas del proceso de priorización.

## **Herramientas**

Utilizo frecuentemente las que a continuación describiré porque permiten visualizar y facilitar el proceso de priorización. Además, resultan simples para entender y livianas de implementar. Existen otras más sofisticadas, por ejemplo las financieras, que calculan el retorno de inversión, sobre las que no profundizaré aquí.

Empezaré por eluser story map, detallando su empleo a la hora de priorizar, durante elproduct discovery. Seguiré con una herramienta extremadamente simple, pero muy útil al mismo tiempo, llamada MoSCoW. A continuación, les mostraré algunas herramientas para visualizar la razón costo-beneficio y finalmente terminaré con otra, llamadaproduct roadmap, muy útil a la hora de facilitar la priorización de funcionalidades nuevas para un producto ya implementado.**      
**

### **User Story Mapping**

Esta herramienta nos permite visualizar el producto completo rápidamente, resultando de gran utilidad para facilitar la priorización. Lo usamos durante las sesiones deproduct discovery, ya que nos permite comprender el orden de importancia de las tareas detectadas y también el conjunto mínimo necesario para una primer versión.

Como ya vimos en el capítulo 1, la manera de indicar que una tarea resulta más importante que otra consiste en situarla sobre la de menor importancia. Esta decisión siempre es precedida por interesantes discusiones plasmadas, de modo visual, en elstory map.

Eluser story mapes una herramienta muy útil también para decidir cuál será el MVP, es decir, el producto que nos permite testear la hipótesis única de valor. Simplemente trazamos una línea por debajo de todas las tareas incluidas en él. Aquellas, situadas por sobre ésta, representan el MVP. Frecuentemente, vemos una gran cantidad depost-itspor sobre la línea, lo que nos permite comprender, instantáneamente, que el MVP seleccionado es demasiado grande. En esos casos, procuramos mover la línea hacia arriba. Como ya mencioné en la sección anterior, prefieroreleasescortos.

![](/assets/product_discovery_mvp.png)

Soy un fan de esta herramienta. Todas las conversaciones empleadas en la toma de estas decisiones tienen lugar frente al ‘mapa’ del producto, quedando inmediatamente plasmadas.**      
**

### **MoSCoW**

Esta técnica de priorización es la más sencilla de todas. Consiste en categorizar lasuser storieso las épicas según su importancia. Las categorías, cuyas iniciales dan nombre a la técnica, son:

* Must: Tienen que estar sí o sí.

* Should: Deberían estar.

* Could: Podrían estar

* Won’t: No van a estar

Pese a su simpleza, esta herramienta resulta sumamente útil, ya quenos obliga a consensuar, entre todo el equipo, una categoría para cada uno de losítems.

> \[Dibujo de gente consensuando la categoría frente al afiche\]

Podemos usarla para priorizar un conjunto deuser storieso épicas de un producto nuevo y también funcionalidades que queremos agregar a uno en funcionamiento. Un ejemplo muy interesante de esta última situación tuvo lugar dentro de un equipo con el que colaboré: 3product ownersdebían priorizar las épicas del bimestre venidero. Resultó muy interesante observar como reconocían la imposibilidad para completar el trabajo, al visualizar la gran cantidad de épicas categorizadas en ‘Must’, y decidían las que podían posponerse. Como ya les mencioné, la utilidad de la herramienta yace en que obliga a un conjunto de personas a consensuar categorías para un conjunto de ítems de un modo muy visual.

Con este equipo, solíamos priorizar también las épicas de cada categoría, sobre todo, las de la categoría ‘Must’. Así, lográbamos categorizar las épicas por bimestre, así como también conocer el orden de las que desarrollaríamos próximamente.**      
**![](/assets/moscow.png)

### **Puntos de Valor de Negocios**

Otra herramienta de gran utilidad durante el proceso de priorización es la asignación de ‘puntos de valor de negocios’ \(business value points\) a las diferentes funcionalidades, haciendo una comparación similar a la utilizada al estimarstory points, pero, esta vez, asignando valores relativos en lugar de esfuerzos relativos. Las piezas de funcionalidad a las que asignamos puntos deben ser necesariamente mayores que lasuser stories, ya que estas últimas, por sí mismas, son unidades funcionales muy pequeñas para representar un valor de negocios.

Como en la técnica de MoSCoW, también nos fuerza a consensuar y explicitar valores. Decimos que una épica es más importante que otra, pero, ¿cuánto? ¿Estamos todos de acuerdo en eso? Explicitar esos puntos de valor de negocio puede resultar un ejercicio muy fructífero para todos.

Además, estimar los puntos de valor de negocios de las épicas nos permite establecer la razón costo-beneficio de cada una de ellas. Existen varios modos de visualización, que transmitiré mediante el ejemplo del sistema para el cajero de supermercados del capítulo 1. Debemos agregar las épicas que presento a continuación, a las cuales asignaremos los siguientes puntos de valor de negocios y esfuerzo. Obtendremos es algo similar a la tabla siguiente:**      
**

| **Épica** | **Valor de Negocios** | **Puntos de Esfuerzo** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2** | **1** | **2** |
| **Pago con Tarjeta de Descuentos** | **5** | **3** | **1.66** |
| **Reportes real-time para Jefes** | **8** | **5** | **1.6** |

La 4ta columna es la razón entre el valor de negocios y los puntos de esfuerzo, es decir, la división entre el valor de la 2da columna y la 3ra. Aquí pueden ver como la épica más beneficiosa es ‘Pago con Bitcoins’, con un beneficio de 2. El valor de negocios es el más pequeño, pero el esfuerzo también. Elproduct ownerpodría decidir priorizar ‘la fruta que cuelga baja en el árbol’ \([low hanging fruit\)](https://www.merriam-webster.com/dictionary/low-hanging fruit). Paradójicamente, la épica menos beneficiosa es la de mayor valor de negocios, justamente porque implica un esfuerzo importante.

En mi experiencia, el costo es un factor sustancialmente menos importante que los demás \(valor de negocios y riesgo\). En contadas ocasiones observé que unproduct ownertomara la decisión de priorizar una funcionalidad solamente porque su desarrollo no fuera costoso. Para resolver esto, podemos añadir ‘pesos’ para cada uno de los factores. Siguiendo el ejemplo anterior, si especificáramos un peso de 0.7 para el valor de negocios y 0.3 para el esfuerzo, obtendríamos los siguientes resultados.

**      
**

| **Épica** | **Valor de Negocios \(0.7\)** | **Puntos de Esfuerzo \(0.3\)** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2 \[1.4\]** | **1 \[0.3\]** | **4.66** |
| **Pago con Tarjeta de Descuentos** | **5 \[3.5\]** | **3 \[0.9\]** | **3.88** |
| **Reportes real-time para Jefes** | **8 \[5.6\]** | **3 \[0.9\]** | **6.22 ** |

[Jim Highsmith](https://g.co/kgs/dNXTTD)argumenta la visualización de los beneficios como porcentajes ya que esto prevendría que, al trabajar con diferentes equipos, se exageren los puntos de valor. Los resultados para el ejemplo serían los que presento a continuación, donde calculamos el porcentaje de valor para cada una de las épicas, el porcentaje de esfuerzo y luego la razón.**      
**

| **Épica** | **Valor de Negocios \(0.7\)** | **% de Valor** | **Puntos de Esfuerzo \(0.3\)** | **% de Esfuerzo** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2** | **0.13** | **1** | **0.14** | **0.92** |
| **Pago con Tarjeta de Descuentos** | **5** | **0.33** | **3** | **0.42** | **0.78** |
| **Reportes real-time para Jefes** | **8** | **0.53** | **3** | **0.42** | **1.26** |
| **Total** | **15** | ** ** | **7** | ** ** | ** ** |

**      
**Todas las técnicas mostradas son similares, ya que nos fuerzan a explicitar valores y esfuerzos y nos devuelven un indicio de lo que podría ser la funcionalidad de mayor beneficio. Pueden incluso agregarse columnas, modificando consecuentemente la fórmula, para incorporar otros factores, por ejemplo, una penalidad \(si la épica no fuera desarrollada\) o el riesgo \(como en el ejemplo delpaperde[Karl Wiegers](http://www.processimpact.com/articles/prioritizing.pdf)\). En definitiva, el valor de la herramienta consiste en que fuerza a volcar toda la subjetividad existente en nuestras cabezas sobre una tabla con números explícitos, que calculan un beneficio a través de una fórmula acordada.

### **Product Roadmap**

Esta es una herramienta utilizada por una experimentadaproduct ownercon la que tuve la oportunidad de trabajar, para priorizar y organizar el trabajo de los próximos meses para los diferentes grupos de los que formaba parte. Después de conocerla, leí el libro [Managing your Project Portfolio](https://g.co/kgs/auAsDJ)de Johanna Rothman, quien la explica detalladamente.

Al observar la imagen siguiente, probablemente alcancen a comprender su funcionamiento. En un eje, se especifican las unidades de tiempo y en el otro, los diferentes equipos. Luego grafican el periodo que, estiman \(de modo superficial\), consumirá cada una de las épicas que tienen priorizadas en la columna correspondiente al equipo al que se asignará.**      
**

![](https://lh5.googleusercontent.com/wjcw73pHK1KI62xEyw6c4Xex8f64og8tnzKig8K10Z5j7gsICpb1L5jMAU5wOumDj3t_41SrJyW0Cyl8mRAyDUiHiKLjl0UDa-82L5_gyjKgRz-TgeZbpC4LT3y07qRxMlfEwso5)

**      
**La única herramienta digital que conozco, sin haber utilizado, es[Roadmunk](https://roadmunk.com/jira-roadmap-integration). Lo bueno de que sea unpluginde[Jira](https://www.atlassian.com/software/jira)reside en que las mismas épicas planeadas en elroadmapson usadas posteriormente en la herramienta de gestión, una vez iniciada la construcción.** **

## **Priorizando Experimentos**

Cuando hablamos de valor de negocios en esta etapa, en la que todavía no existe un producto, en realidad hipotetizamos sobre el potencial que, creemos, entregará. Nos queda validar estas hipótesis con usuarios reales, ¿estarán dispuestos a pagar por nuestro producto?

Haremos esto mediante experimentos, que testean si lo supuesto se cumple. Teniendo esto en cuenta, la priorización consiste en determinar el modo de testeo de las hipótesis. En otras palabras, pensar y priorizar experimentos y, de acuerdo a ésto, decidir qué funcionalidad incluir en cada uno de ellos. De este modo, el producto mínimo viable \(MVP\) no es más que el primero de nuestros experimentos, que valida la hipótesis única de valor.

Todos estos conceptos están tomados de la metodología de[Lean Startups](https://g.co/kgs/dkPNEB), de Eric Ries.Planear, construir y validar con usuarios reales. Los lineamientos generales son muy similares a los de las metodologías ágiles, pero van un paso más allá.

Uno de los puntos fundamentales de esta metodología consiste en definir cómo vamos a medir el funcionamiento del experimento. De haber realizado ellean canvas, mencionado en el capítulo 1, recordarán que una de las secciones consistía en describir, explícitamente, estos experimentos. En muchos de los desarrollos en los que trabajé, no existía certidumbre acerca de cómo se validaría lo construido. Sin embargo, esto es fundamental, ¡debemos saber lo que se quiere lograr!

Cheryl Quirion compartía estos experimentos, visualmente, con todo el equipo de desarrollo, usando una técnica que denominó[Lean Visual Strategy](https://leanvisualstrategy.com/what-is-lean-visual-strategy-4b4dc9df610d). Compartir esta información con el equipo permite que esté alineado y entienda por qué lo está construyendo. Hacerlo de manera visual ayuda a que todos incorporen esta información mejor y más rápidamente.

## **Conclusiones**

Hacer una buena priorización antes de comenzar a trabajar en la construcción es fundamental. Establecemos un conjunto de funcionalidades que, consideramos, deben existir en el MVP y las priorizamos para empezar por las más importantes.Establecemos así un plan para agregar valor y bajar el riesgo.

Este camino que trazamoses creado colaborativamente y compartido por todos los participantes. Las herramientas que mencioné contribuyen en el proceso. Una vez iniciada la construcción resulta fundamental mantener unbacklogactualizado. Queremos estar seguros de estar trabajando, en todo momento, sobre las funcionalidades más importantes, es decir, las que aporten más valor y reduzcan más el riesgo.

