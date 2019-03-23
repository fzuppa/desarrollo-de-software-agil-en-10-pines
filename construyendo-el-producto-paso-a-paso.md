

![](./assets/Tapa - Desarrollando Software.png)

# **Desarrollando software, paso a paso**

En capítulos anteriores, descompusimos nuestro trabajo en incrementos funcionales, que llamamos *user stories*, con el objetivo principal de involucrar a los usuarios de negocios durante la construcción del producto. En este capítulo describiré el proceso de desarrollo iterativo e incremental: cómo construimos esas *user stories*, por qué usamos iteraciones de duración fija y, finalmente, por qué trabajar de este modo resulta importante para lograr nuestros objetivos.



# Proceso de Desarrollo Iterativo e Incremental

Empezamos nuestro desarrollo por las *user stories* que priorizamos en nuestro backlog, que iremos construyendo gradualmente para obtener feedback rápido. Algunas de estas *stories* son bosquejos, esqueletos no terminados, partes incompletas de funcionalidad, que necesitan trabajo adicional para ser finalizadas. Otras son incrementos funcionales completos, listos para implementarse en producción. Las primeras corresponden a la estrategia iterativa. Las segundas, a la estrategia incremental. El proceso de desarrollo iterativo e incremental combina ambas estrategias. 

Jeff Patton, en un viejo [post](http://www.jpattonassociates.com/dont_know_what_i_want/), las detalla preguntándose cómo haríamos para pintar la Mona Lisa si lo hiciéramos de uno u otro modo.

Si lo hiciéramos de modo 100% iterativo, empezaríamos por dibujar un bosquejo del cuadro completo (paso 1), que iríamos refinando en versiones posteriores:

##### ![](./assets/iterating.jpg)

Al momento de pintar cada una de las versiones intermedias, **necesitaríamos tiempo para iterar sobre esta versión,** es decir cambiarla, mejorarla. [Alistair Cockburn](http://www.se.rit.edu/~swen-256/resources/UsingBothIncrementalandIterativeDevelopment-AlistairCockburn.pdf) describe este proceso como **una estrategia de retrabajo**. En cada una, agendamos tiempo para revisar y mejorar el cuadro.

¿Y si lo hiciéramos de modo 100% incremental? Descompondríamos el cuadro en diferentes partes, que iríamos pintando gradualmente:



![](./assets/incrementing.jpg)



Cada una de estas partes estaría completa, sin necesidad de retrabajo. Tendrían calidad de producción. Alistair describe este proceso como una estrategia de planeamiento. La alternativa sería hacer un desarrollo completo que contenga toda la funcionalidad.

El proceso de desarrollo iterativo e incremental combina las 2 estrategias. Algunas de nuestras *stories* son bosquejos que necesitan retrabajo. Por ejemplo, podemos hacer una *user story* para un formulario de alta, sabiendo que, más adelante, incorporaremos las validaciones y el *look & feel*. Otras son incrementos funcionales completos que podrían implementarse en producción una vez desarrollados. Durante el comienzo del proyecto, abordaremos las *stories* correspondientes a la estrategia iterativa, ya que necesitamos construir el esqueleto de la aplicación, su arquitectura. A medida que progresemos con el desarrollo, trabajaremos con más *stories* que correspondan a la estrategia incremental. 



# Trabajando en Iteraciones de duración fija

Con el plan y las *user stories* que tenemos, podríamos empezar con el desarrollo. Sin embargo, el horizonte apuntado quizás resulte demasiado lejano. ¿Podremos mantener el foco durante esos 3 meses que, estimamos, durará el desarrollo del MVP? Difícil.

Para lidiar con ésto, podemos dividir esos 3 meses en *slots*, de duración fija (por ejemplo 2 semanas), que se denominan iteraciones. En el comienzo de cada una de ellas, decidimos un conjunto de funcionalidad que consideramos apropiado para ese periodo. Con un horizonte tan cercano, **nos enfocaremos en terminar este subconjunto de funcionalidad** que nosotros mismos planeamos, sin desconcentrarnos con *features* futuros.

Al finalizar cada iteración “paramos la pelota”, como suele decirse en el ámbito futbolístico, **para medir la capacidad real del equipo** (su *velocity*) y también **para inspeccionar qué funcionó y qué podemos mejorar**. Usamos esta información para establecer acciones de mejora y [modificar el plan](planeamiento-agil.md).

Con el correr de las iteraciones, lograrmos un ritmo. Se acostumbrará a planear, enfocarse en terminar el trabajo planeado para la iteración, hacer introspección y comenzar el ciclo nuevamente. Los agilistas llaman a esto cadencia.



## ¿Siempre usamos iteraciones fijas?



Me gusta trabajar con iteraciones fijas (*timeboxed iterations*), sobre todo en proyectos como los descritos en este libro. Creo que el equipo gana foco en periodos cortos, mejora el proceso entre las iteraciones y mantiene una cadencia. Sin embargo, tenemos otros clientes, que desarrollan mejoras evolutivas o soporte de producción, donde no las usamos. En estos casos, al suprimir las iteraciones, estamos pasando a un sistema ‘*pull*’ donde, en vez de ‘empujar’ un conjunto de trabajo hacia una iteración, lo ‘pulleamos’ (una *user story*) cuando tenemos la capacidad. En sistemas Kanban como el previamente descripto, el foco se mantiene a partir del límite de trabajo en progreso, la capacidad se mide a partir del *leadtime* y el *throughput* y la cadencia se logra a partir de [otros mecanismos](http://www.djaa.com/kanban-cadences). Lo esencial, trabajar iterativa e incrementalmente con equipos multidisciplinarios y auto-organizados, se mantiene. 



# El trabajo de una Iteración

Como ya les comenté en la sección anterior, el equipo se auto-organiza para seleccionar el conjunto mínimo de *user stories* que puede construir eficientemente. Los desarrolladores somos quienes mejor conocemos el tamaño de éstas y quienes mejor podemos dividir y organizar el trabajo que debe realizarse. 

Intentaremos terminar la mayor cantidad de *user stories*, abordándolas en base a su prioridad. **La heurística que propongo para lograr este objetivo consiste en maximizar el flujo, minimizando el trabajo en progreso**. ¿Qué significa esto? Trabajar en la menor cantidad de *user stories*, siempre que esto sea eficiente. ¿Cuántos desarrolladores pueden trabajar eficientemente en cada *story*? Nuevamente, el equipo es quien mejor sabe cómo responder esta pregunta.

Antes de empezar cada *story*, reunimos a los desarrolladores involucrados y los integrantes de negocios para refinar los últimos detalles. Se pulen los bordes. Se discute sobre los argumentos que vuelven necesaria esa funcionalidad, una vez más. También, cómo se testeará y validará. Entramos así de lleno en el diseño, que hacemos con la colaboración de todos los integrantes del equipo.

Desarrollamos pensando, en primer lugar, en los tests automatizados que validarán la funcionalidad y procurando obtener ‘calidad de producción’, como dice la guía de Scrum. Este es el momento de hacer el producto con calidad. La calidad se ‘hornea desde el principio’ [[1]](construyendo-el-producto-paso-a-paso.md#notas-al-pie), no puede incorporarse al final. 

Una vez que terminamos el desarrollo y testeo de una *user story*, realizamos un proceso de aceptación formal, donde repasamos, una vez más, el cumplimiento de todos los criterios de aceptación. También podemos repasar nuestra ‘[definition of done](https://www.agilealliance.org/glossary/definition-of-done/)’ para estar completamente seguros de que hemos terminado.

Todo este proceso, altamente concurrente, involucra un grado de comunicación muy intenso. El *Product Owner* y los usuarios de negocios trabajan de la mano con los desarrolladores para construir el producto que desean, comunicando claramente y validando cada incremento. Todo este feedback, brindado a tiempo, se incorpora dentro del producto.



# ¿Qué logramos trabajando de esta manera?

El desarrollo iterativo e incremental es uno de los pilares fundamentales de la agilidad. Repasemos lo que logramos, al trabajar de esta manera:

**Crear un plan ágil**: como ya les comenté en el capítulo correspondiente, hacemos un plan liviano, sabiendo que aprenderemos y podremos incorporar ese conocimiento dentro del mismo. Trabajar de este modo nos ahorra análisis detallados, que no aportan valor.

**Recibir feedback temprano**: terminar incrementos funcionales rápidamente permite que el *product owner* se involucre en el desarrollo, brindando un feedback útil para moldear el producto de acuerdo a sus necesidades. Iterar [amplifica el aprendizaje](http://www.poppendieck.com/pdfs/AmplifyLearning.pdf) y maximiza el valor del producto final.

**Aumentar la calidad**: se brinda un feedback rápido acerca de la calidad a partir del testeo de cada incremento, en lugar de hacerlo al final. Incorporar la calidad buscada dentro del proceso de construcción resulta fundamental.

**Adaptarnos al cambio**: uno de los objetivos más importantes buscados por la agilidad es poder adaptarnos al cambio. Cuando trabajamos de este modo, podemos hacerlo eficientemente.

**Hacer releases parciales**: Finalmente, este modo de trabajo permite realizar *releases*, cuando completamos un conjunto de *user stories* que, juzgamos, representan un ciclo completo de funcionalidad.

¿Tiene alguna desventaja trabajar de este modo? La primera que puedo nombrarles es la eficiencia. Iterar sobre una funcionalidad implica retrabajo. Por otra parte, estos incrementos, desarrollados por un equipo multidisciplinario, generan una concurrencia alta con el consecuente costo de comunicación. En contrapartida, el desarrollo en cascada divide el trabajo en fases en las cuales no es necesario que todos trabajen, haciendo que la concurrencia sea menor y que, por ende, aumente la eficiencia. No considero que esta sea una ventaja válida, principalmente porque no redunda en un mejor producto. Además de perderse los beneficios anteriormente enumerados.



# Conclusión

Construimos el software gradualmente, a partir de incrementos funcionales pequeños con el objetivo de recibir feedback temprano. Trabajamos en iteraciones de duración fija para ganar foco, medir nuestra *velocity* y establecer una cadencia. El desarrollo iterativo e incremental es uno de los pilares fundamentales de la agilidad.

# Notas al Pie

1. Bake quality in [[Poppendieck00]](bibliografia.md#Poppendieck00)