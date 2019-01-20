
# Resumen general

* Pablo trabaja con equipos que no saben cómo escribir código mantenible y tiene que formarlos. Habló de cómo formar en grupo en vez de 1 a 1, buscar ejemplos reales y concretos y visualizar el dolor (cuantos bugs hay ahora...) para que vean cómo mejora la situación.
* Néstor plantea una arquitectura (hexagonal + testing outside-in) para no vincularte a un framework concreto y permitir centrarte en negocio.
* Acero comenta cómo cambiaron la plataforma de pago (parallel changes), cómo lo harían actualmente y qué problemas se han encontrado.
* Javier habló de los problemas de un producto con sus APIs públicas y cómo aplicar prácticas para poder evolucionarlas sin que sufran los desarrolladores que las están usando.
* Beñat comentó su experiencia al desarrollar un módulo propio en vez de utilizar el aportado por el framework, lo que implicó mucho tiempo de desarrollo y complicar enormemente el mantenimiento.
* Apa se enfrenta al problema de poner al día a un miembro nuevo del equipo en un nuevo lenguaje/framework y propone hacer "Practica con tu propia comida", inspirado en katas/pet projects.

# Conclusiones del grupo

Todas las experiencias están relacionadas con prácticas técnicas y la mayoría son similares (la experiencia de APA es la más diferente) pero hay un par de patrones comunes:

## Relacionadas con gestión del cambio. 

En general todas las experiencias están relacionadas con gestión del cambio, específicamente, cambios en requisitos de negocio:

* Pablo: querer soportar evolución de un proyecto
* Nestor: querer tener una app que soporte cambios, que me permita tomar el mínimo número de decisiones posibles de partida
* Acero: cambio en plataforma de pago que implica muchos cambios en el código y crear abstracciones
* Javier: cambios en APIs
* Beñat: decisiones ante una nueva funcionalidad, que condicionan el desarrollo y la flexibilidad/evolución de hacer cambios futuros. La flexibilidad implica costes disparados dependiendo de la decisión.
* Apa: nuevo miembro del equipo con un nuevo lenguaje

## Reflexiones sobre la aplicación de una práctica

Las experiencias comentaban las ventajas e inconvenientes de aplicar diferentes prácticas, generalmente técnicas a un equipo/proyecto.

* Buscar casos prácticos sobre los que todo el equipo pueda cambiarlo, en vez de katas ideales alejadas del negocio.
* Las prácticas son útiles pero lo que deberíamos buscar es cambiar el equipo (concepto de equipo legado, no código legado) para que intente mejorar.

# Ideas

* Las decisiones de negocio producen cambios. En general son el principal factor de cambio (o el más importante).
* Tomar decisiones al principio determina el peso del cambio, condicionan facilidad de cambio y coste. 
* Dualidad flexibilidad/coste. Más flexibilidad implica más coste.
* Justificar la decisión de tener una flexibilidad. Haberla creado desde el principio es mucho más barato pero añadirla después es caro.
* Cuando diseñas/desarrollas deberías intentar tomar la decisión que te comprometa menos.
* Decisiones deliberadas y conscientes. Tomamos muchas decisiones no deliberadas ni conscientes... simplemente el hecho de pensar: "Elijo esta pasarela de pago porque no va a cambiar en los próximos 5 años" implica que escribiremos código de forma diferente.
* **Escribir el software para intentar minimizar el coste de añadir flexibilidad más adelante**.
* Pain driven development. Visualizar el dolor para poder cambiarlo.
* Objetivos medibles sobre lo que quieres medir.

Todo esto tiene sentido sólo en algunos casos. La importancia del objetivo del proyecto (producto, consultoría). Hemos escrito algunas ideas para ayudar a aclarar este problema (quién se va a comer el proyecto?...)
