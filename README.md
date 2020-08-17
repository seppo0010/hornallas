# Análisis de preferencias de hornallas

Por Valeria Edelsztein y Sebastian Waisbrot

- Hola. Mi nombre es Sebastián.
- Hola, Sebastián.
- Siempre que voy a calentar algo en una hornalla uso la misma. No sé cuándo
elegí cuál usar, pero ahora no me veo usando otra. Y lo que es más importante, no
sé por qué elegí la que elegí.
- No te preocupes, acá podemos ayudarte.

¿Por qué elegimos lo que elegimos? ¿Existe el libre albedrío? ¿Somos conscientes de nuestras elecciones? No tenemos ni idea. Pero nos embarcamos en este estudio para tratar de entender si existe alguna motivación para tener una hornalla favorita. Miles de respuestas, horas de debate, ríos de tinta (electrónica), toneladas de análisis después llegamos a algunas conclusiones y acá se las compartimos.

## Muestra

A lo largo de dos días, una increíble cantidad de 4949 personas respondieron a la encuesta anónima que preparamos. Eso nos indica (1) que nos encanta responder encuestas, (2) que el tema de las hornallas favoritas es de interés poblacional y/o (3) que preferimos dedicar tiempo a estos menesteres en lugar de a otras cuestiones más urgentes. No somos quiénes para juzgar.

Es importante tener en cuenta que la encuesta fue voluntaria (¿por qué obligaríamos a alguien a decirnos cuál es su hornalla favorita siendo un tema tan personal?) y la muestra autoseleccionada así que no es necesariamente representativa de la población en general.

Para el análisis de datos "limpiamos" previamente la muestra eliminando aquellas respuestas que no tenían sentido. Por ejemplo, personas que habían puesto que su altura era 3.1416. Sin duda, quienes somos seres del bien amamos a pi, pero definitivamente no puede ser la altura de una persona.

Hecha esta limpieza, la muestra final consistió en las respuestas de 4939 personas.

## Análisis estadístico (AHRE)

Debido al amplio compromiso de la población con la resolución de la encuesta, decidimos realizar un análisis estadístico de los resultados a conciencia.
Para eso, en muchos casos aplicamos el coeficiente de correlación de Pearson para analizar la dependencia entre dos variables, también usamos p-valores para decidir si había diferencias significativas entre distintas poblaciones, en un caso aplicamos una distribución binomial e, incluso, hicimos un test con nombre de Vodka:Kolmogorov–Smirnov.

## ¿Cuál es la hornalla favorita?

Podríamos decir que la hornalla favorita de la población que analizamos es la que más gente prefiere.
En este caso (suenen trompetas): adelante y a la derecha seguida muy, muy de cerca por adelante y a la izquierda.

Datos, no opinión. No nos vengan con pucheritos si no ganó su favorita.

![Hornalla favorita. Adelante derecha: 1790 votos, Adelante izquierda: 1657,
Atrás derecha: 826, Atrás izquierda: 666](hornallas.png)

Más allá de este resultado, algo más interesante es tratar de entender si existen razones para que esto sea así. 
Para intentar dilucidarlo, desarrollamos algunas hipótesis, es decir ideas de comportamiento que esperamos, e intentamos validarlas (o no) a partir de los datos que recolectamos. 

## Hipótesis

### Se usa más la hornalla correspondiente a la mano hábil

¿Los diestros usan más las hornallas derechas y los zurdos más las izquierdas?
La respuesta es sí, pero muy poco. La lateralidad no parecería influir en nuestro favoritismo hornallil (de ahora en más, FH).

![
Hornalla favorita por mano hábil.
Diestros que prefieren hornalla izquierda: 2042,
Diestros que prefieren hornalla derecha: 2352,
Zurdos que prefieren hornalla izquierda: 278,
Zurdos que prefieren hornalla derecha: 261
](manohabil.png)

### Se usa más la hornalla que está del lado de la mesada

Para saber si la posición de las hornallas respecto de la mesada es una variable importante a la hora de discernir el FH, nos quedamos sólo
con los datos de quienes tienen mesada a uno de los costados. En este caso encontramos que sí hay diferencias significativas. ¡Alegría!

![
Hornalla favorita por lado de mesada.
Mesada a la derecha, hornalla favorita a la derecha: 1094,
Mesada a la derecha, hornalla favorita a la izquierda: 516,
Mesada a la izquierda, hornalla favorita a la izquierda: 980,
Mesada a la izquierda, hornalla favorita a la derecha: 617
](ladomesada.png)

### Se usa más la hornalla de atrás si se tienen criaturas

¿La gente con criaturas teme que toquen accidentalmente las hornallas delanteras
y por eso usan más las de atrás? Aparentemente sí. Vemos que es algo que pasa bastante. Sin embargo, no llega a ser la mayoría de los casos. 
Evidentemente la seguridad infantil no parecería ser prioridad a la hora de elegir una hornalla favorita. POLÉMICO.

Es de destacar que varias personas comentaron que les quedó la costumbre de usar hornallas traseras aún
cuando sus criaturas ya han dejado el hogar hace rato. Sabemos que anécdota no es evidencia, pero no perdamos de vista que estamos analizando una encuesta sobre hornallas.

![
Hornalla favorita según presencia de niñes menores.
Gente con niñes que prefiere una hornalla adelante: 670,
Gente con niñes que prefiere una hornalla atrás: 524,
Gente sin niñes que prefiere una hornalla adelante: 2773,
Gente sin niñes que prefiere una hornalla atrás: 966
](ninyes.png)

### Se usan más las hornallas de atrás si la persona es alta

¿La gente alta prefiere las hornallas más atrás que la gente más baja? Sí, un poco.
La gente cuyo FH se inclina por las de atrás es, en promedio, 2 cm más alta.

¡Atención! No es cierto que elegir las hornallas de atrás a partir de ahora te agregará 2 cm. Parece obvio pero es importante aclararlo. Tampoco tomen lavandina, por el amor de Bohr.

![
Preferencia de hornalla por altura.
Hornalla delantera Q1: 1.60,
Hornalla delantera Q2: 1.67,
Hornalla delantera Q3: 1.74,
Hornalla trasera Q1: 1.62,
Hornalla trasera Q2: 1.69,
Hornalla trasera Q3: 1.76,
](altura.png)

### Se usa más la hornalla de adelante si se usa encendedor para prenderla

Supusimos que, de usar un encendedor, sería más cómodo prender la hornalla más "cercana" así que decidimos validar esta hipótesis y parece que sí, hay una correlación significativa en este sentido.

![
Hornalla favorita según uso de encendedor.
Usa encendedor, prefiere hornalla delantera: 831,
Usa encendedor, prefiere hornalla trasera: 289,
No usa encendedor, prefiere hornalla delantera: 2045,
No usa encendedor, prefiere hornalla trasera: 1009
](encendedor.png)

### Se usa más la hornalla más fuerte

Somos gente intensa. Y los datos lo validan: las hornallas más fuertes suelen ser preferidas a las demás.

Para llegar a esta conclusión primero tuvimos que analizar cuál era la probabilidad aleatoria de elegir esa hornalla. Entonces, por ejemplo, si las 4 hornallas funcionan y solamente una es alta, la probabilidad de elegirla al azar es 1/4 (0,25) pero si hay dos hornallas altas, se convierte en 2/4, es decir 0,5. En el gráfico se muestra la probabilidad esperada (aleatoria) en barras blancas y la ocurrencia según nuestros datos en verde. Vemos que, para todos los casos, la probabilidad de elegir la hornalla con más intensidad es mayor que la esperada por azar.

![
Hornallas de intensidad alta favoritas.
Proporción de hornallas de intensidad alta 3/4: 0.81,
Proporción de hornallas de intensidad alta 2/3: 0.85,
Proporción de hornallas de intensidad alta 1/2 o 2/4: 0.67,
Proporción de hornallas de intensidad alta 1/3: 0.59,
Proporción de hornallas de intensidad alta 1/4: 0.47,
](intensidad.png)

### La edad no es predictora de la hornalla favorita

Nuestra primera hipótesis era que la edad no tenía nada que ver con el FH. Pero cuando analizamos los datos, el resultado fue sorprendente: a priori la edad parecía predecir una preferencia por hornallas traseras. MISTERIO Y ESTUPOR.

![
Preferencia de hornalla por edad
Hornalla delantera Q1: 24,
Hornalla delantera Q2: 28,
Hornalla delantera Q3: 35,
Hornalla trasera Q1: 25,
Hornalla trasera Q2: 31,
Hornalla trasera Q3: 39,
](edad0.png)

¿Cómo explicar esto? Pensamos que, quizás, la gente de más edad tenía o había tenido (recordemos que somos animales de costumbre) criaturas. 
Por eso, decidimos controlar por esa variable. 
Una vez que nos quedamos sólo con gente que no tiene criaturas, vimos que la preferencia desaparecía. AHORA SÍ.

![
Preferencia de hornalla por edad (sin hijes)
Hornalla delantera Q1: 23,
Hornalla delantera Q2: 27,
Hornalla delantera Q3: 33,
Hornalla trasera Q1: 24,
Hornalla trasera Q2: 28,
Hornalla trasera Q3: 35,
](edad1.png)

### Los hombres tienen más preferencia por la hornalla de mayor intensidad

Era una linda hipótesis, pero no encontramos diferencias significativas entre géneros en este aspecto.

### El género no predice el FH

Los hombres demuestran usar más las hornallas traseras. Pensamos que esto podía deberse a cuestiones de altura y presencia de criaturas en el hogar.
De hecho, al controlar por niñes, la tendencia desaparece.

## Modelo explicativo

Y acá es donde se pone divertido (?).

Si quisiéramos saber qué características hay que considerar para determinar la hornalla favorita de
una persona de la cual no conocemos su FH, podríamos dividir el problema en dos partes: 
- Profundidad: adelante/atrás
- Lateralidad: izquierda/derecha.

Sobre esta base, construimos un modelo sencillo de aprendizaje automático para determinar reglas que nos permitieran predecir los dos componentes del FH en función de los datos de una persona. Las reglas que encontramos fueron las siguientes.

### Profundidad

Se prefiere una hornalla delantera siempre y cuando la hornalla de mayor
intensidad no esté atrás y no haya criaturas en la casa.

### Lateralidad

En este caso el modelo fue, por decirlo de alguna manera, más "creativo".

Se prefiere una hornalla de la izquierda si ocurre cualquiera de las siguientes
condiciones:

* La hornalla de mayor intensidad está a la izquierda y hay mesada hacia la
izquierda.
* La hornalla de mayor intensidad está adelante y hay mesada hacia la izquierda
pero no hacia la derecha.

### Calidad del modelo

¿Cuánto entendemos ahora acerca de nuestra preferencia de hornallas? Un poco más que
antes. Con las reglas que propuso el modelo, pudimos asignar correctamente el FH un 34% de las veces, mientras
que al azar sólo lo hubiesemos logrado un 25%.

Se podrían intentar obtener mejores resultados con estos datos usando modelos más
complejos, o preparando los datos de otra forma, o quizás sea necesario hacer
una encuesta más profunda para entender el subconsciente humano. Pero tampoco
podemos descartar la alternativa de que muchas personas tengan un FH caprichoso
y arbitrario, que no pueda ser explicado por la ciencia.

## FIN - APLAUSOS - CAEN LOS CRÉDITOS  

Si llegaron hasta acá es porque realmente tenían interés en el tema. Como valoramos profundamente ese compromiso, y a la manera de recompensa pixareana, he aquí el bonus track post-créditos.

## Descubrimientos

### Hornallas mixtas o combinadas

Tres personas cada mil respondieron que tenían
hornallas mixtas, es decir algunas a gas y otras eléctricas. Algunas de ellas
también nos avisaron que su horno era eléctrico, lo cual escapa al objeto de
estudio de esta encuesta, pero es bueno saberlo.

### Hornallas que no respetan el clásico cuadrado

Ciertas personas señalaron que su disposición hornallística no se acomodaba a las especificaciones de la encuesta. 
Aparentemente hay hornallas ubicadas en forma de cruz ("No tengo 2 hornallas delante y 2 detrás, están en las esquinas de un rombo. Una delante, dos al centro, una detrás") e, incluso, hornallas quíntuples donde una de ellas está en el centro. 
¿Qué decir? La búsqueda estilística tiene sus desventajas. Por ejemplo, no poder responder adecuadamente este dispositivo metodológico de indagación. 
Es el precio a pagar.

### Vitrocerámico

Aprendimos que las [cocinas vitrocerámicas](https://es.wikipedia.org/wiki/Cocina_vitrocer%C3%A1mica)
se consideran hornallas eléctricas.

### Encendido

¡Mucha gente prende las hornallas con encendedores!

![¿Con qué encendés las hornallas?. Encendedor: 1879. Fósforos: 1730. Botón de
la cocina: 1220. Magiclik: 812. Es automático: 456](conqueencendes.png)

Pero lo que es más extraño, varias de estas personas lo hacen con encendedores
sin gas o rotos. 
Y, más extraño aún, esas personas sintieron una fuerte necesidad de compartirlo, nos imaginamos con
orgullo. Algunos comentarios simpáticos a esta pregunta -y otros que nos hacen dudar acerca de cómo la humanidad sigue viva- fueron:

* Palitos o papel
* Pedernal o chispero (el que se usa para prender las soldadoras)
* Con las velitas largas del súper, que enciendo en el piloto del calefón
* Se me rompió el magiclick cuando compré el repuesto de gas, antes de la cuarentena
* Lo que encuentre primero
* Una vez corri desde el living con un papelito encendido
* Papel prendido fuego con el piloto del calefón
* Una servilleta prendida por la llama del calefón cuando algún gil me roba el encendedor

También hubo gente que nos abrió su corazón:

* Botón pero ta roto entonces uso mi hornalla no favorita 🥺

¡Ah! Y aprendimos algo fundamental: no hay que poner opción "Otros" porque después ponen esas respuestas y ordenar los datos es un lío. Se los dejamos como moraleja de la historia. Después de todo, es importante compartir la sabiduría.
