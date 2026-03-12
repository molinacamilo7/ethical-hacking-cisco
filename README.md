Ethical Hacking – Cisco
Resumen personal: Capítulos 1 y 2

# Ethical Hacking y Pruebas de Penetración

## Capítulo 1: Introducción

Cuando alguien dice "hacker", casi todos imaginamos lo mismo: un tipo con capucha, 
pantallas llenas de código verde, música de fondo. El estereotipo clásico. Y sí, 
existe por algo, pero es una versión bastante recortada de la realidad.

Lo que no se dice tan seguido es que hay profesionales que hacen exactamente lo mismo 
que un atacante, con la diferencia de que lo hacen con permiso, con un objetivo y 
dentro de reglas claras. Eso es, en esencia, el hacking ético.


### ¿Qué es?

Un hacker ético entra a un sistema para encontrar sus fallas antes de que alguien con 
malas intenciones lo haga. Simple. La clave no está solo en las habilidades técnicas, 
sino en el permiso y en la intención.

Para entender este mundo, se usan tres categorías que ya se han vuelto casi un lenguaje 
común:

- **Sombrero blanco** → trabajan de forma legal, protegiendo sistemas.
- **Sombrero negro** → actúan sin permiso, generalmente buscando hacer daño o sacar provecho.
- **Sombrero gris** → están en un punto medio raro: encuentran vulnerabilidades sin que 
  nadie se los haya pedido, sin querer causar daño necesariamente, pero tampoco con 
  autorización. No son héroes ni villanos, están en ese limbo incómodo.

Conocer estas diferencias sirve para algo concreto: entender que hackear no es sinónimo 
de delinquir, y que tener buenas intenciones tampoco te hace automáticamente ético si 
estás operando sin permiso.


### Pruebas de penetracion

Una prueba de penetración, o **pentesting**, no es algo que se improvisa. Existen 
metodologías estructuradas precisamente para no saltarse pasos que después se convierten 
en problemas.

Las más conocidas son:

- **OWASP** → se especializa en aplicaciones web.
- **PTES** → cubre todo el proceso de principio a fin, incluyendo el reporte final.
- **NIST** → enfoque más amplio sobre cómo las organizaciones gestionan su seguridad.

También varía según cuánta información maneja el evaluador:

| Tipo | Descripción |
|------|-------------|
| **Caja negra** | Sin información previa. Entrar sin saber qué hay adentro. |
| **Caja blanca** | Acceso total a la información del sistema. |
| **Caja gris** | Información parcial. La más parecida a escenarios reales. |


Antes de operar en sistemas reales, hay que poder equivocarse sin consecuencias.

Para eso sirven herramientas como VirtualBox** o VMware, que permiten correr 
sistemas operativos dentro del propio computador sin afectar nada externo. Con eso 
se puede instalar Kali Linux, que ya viene cargada con herramientas de seguridad, 
junto con máquinas intencionalmente vulnerables diseñadas para practicar ataques de 
forma controlada.

No es un lujo ni un extra. Si se quiere aprender en serio, este espacio es el punto 
de partida.


## Capítulo 2: Planificación y Alcance

Si el capítulo anterior era el *qué es*, este es el *cómo se prepara todo* antes de 
tocar una sola cosa. Uno de los errores más comunes de quienes empiezan es subestimar 
la planificación porque no parece tan interesante como ejecutar un ataque. El problema 
es que sin esto bien hecho, todo lo demás puede descarrilarse, incluso con las mejores 
intenciones.


### Contexto antes de acción

Para trabajar en seguridad, no basta con saber usar herramientas. Hay que entender el 
entorno, y eso implica tres conceptos que siempre van juntos:

- **Gobernanza** → las políticas internas de la organización. El reglamento de cómo 
  manejan su propia seguridad.
- **Riesgo** → la probabilidad de que algo salga mal y qué tan grave sería si ocurre.
- **Cumplimiento** → normas externas como **ISO 27001** o **PCI-DSS** que la 
  organización está obligada a respetar.

Estos tres conceptos se mezclan constantemente. Entenderlos permite saber qué le 
preocupa realmente al cliente y dónde tiene sentido enfocar el trabajo.


### El alcance:

Definir el alcance es lo que más consecuencias tiene si se hace mal. Establece 
exactamente qué sistemas se pueden analizar, en qué momentos, con qué herramientas 
y hasta dónde se puede llegar.

Sin esto claro, una prueba de penetración puede convertirse en un problema legal de 
un momento a otro, aunque el pentester haya actuado de buena fe. No es exageración, 
es algo que ha pasado.

Para evitarlo, existen documentos concretos:

- **Reglas de Compromiso** → establecen qué está permitido y qué no.
- **Acuerdo de confidencialidad** → protege la información sensible que aparece durante 
  la prueba.
- **Carta de autorización** → el respaldo escrito de que la organización dio su 
  consentimiento.

> El alcance no es el mismo para todos los entornos. No es igual trabajar sobre 
> servidores físicos que sobre infraestructura en la nube.
> Cada escenario tiene sus propias reglas.


### Actitud y comportamiento: lo que nadie enseña explícitamente

Ser un buen profesional en este campo no depende solo de conocer herramientas o 
vulnerabilidades. Depende del criterio con el que se toman decisiones en el camino.

Algunas cosas que parecen obvias pero vale decir:

- Cualquier información que aparezca durante una prueba (contraseñas, datos personales, 
  configuraciones internas) **no se comparte, no se guarda para uso propio, no se 
  menciona fuera del proyecto**.
- Los hallazgos se reportan como son: ni inflados para parecer más útil, ni minimizados 
  para no incomodar.
- Si algo sale mal durante la prueba, se comunica de inmediato.

La diferencia entre un hacker ético y uno que no lo es no pasa únicamente por tener 
un permiso firmado. Pasa por la actitud con la que enfrenta el trabajo cada vez.


## Resumen

Estos dos capítulos hablan algo que va más allá de lo técnico. No son solo 
definiciones o listas de pasos, es una forma de entrar a este campo con criterio.

Antes de aprender a usar cualquier herramienta, hay que tener claro:

1. Quién se es dentro de este trabajo.
2. Qué se puede hacer y qué no.
3. Cómo se hace correctamente.
4. Con qué valores se opera.
