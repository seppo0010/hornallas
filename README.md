# Preferencias de Hornallas

Por Valeria Edelsztein y Sebastian Waisbrot

Siempre que voy a calendar algo en una hornalla uso la misma. No sé cuándo
elegí cuál usar, pero ahora no me veo usando otra. Lo que es más importante, no
sé por qué elegí la que elegí.

Nos embarcamos en este estudio para entender esa motivación. Cabe destacar que
la encuesta es voluntaria y la muestra autoseleccionada po lo que no es
necesariamente representativa de la población en general.

## ¿Cuál es la hornalla favorita?

Podríamos decir que la hornalla favorita es la que más gente prefiere.

![Hornalla favorita. Adelante derecha: 1790 votos, Adelante izquierda: 1657,
Atrás derecha: 826, Atrás izquierda: 666](hornallas.png)

Sin embargo esto no nos ayuda a entender por qué esto es así. Para eso vamos a
desarrollar hipótesis, es decir ideas de comportamiento que esperamos, y
veremos si esto se da en la práctica o no

## Hipótesis

### Se usa más la correspondiente a la mano hábil

¿Los diestros usan más las hornallas derechas y los zurdos más las izquierdas?
La respuesta es sí, pero muy poco.
![
Hornalla favorita por mano hábil.
Diestros que prefieren hornalla izquierda: 2042,
Diestros que prefieren hornalla derecha: 2352,
Zurdos que prefieren hornalla izquierda: 278,
Zurdos que prefieren hornalla derecha: 261
](manohabil.png)

### Se usa más la que tiene del lado de la mesada

¿Se usan más las hornallas del lado de la mesada? Para eso nos quedamos sólo
con quienes tienen mesada a un costado y vemos que es significativa la
diferencia.

![
Hornalla favorita por lado de mesada.
Mesada a la derecha, hornalla favorita a la derecha: 1094,
Mesada a la derecha, hornalla favorita a la izquierda: 516,
Mesada a la izquierda, hornalla favorita a la izquierda: 980,
Mesada a la izquierda, hornalla favorita a la derecha: 617
](ladomesada.png)

### Se usa más la de atrás si se tienen niñes

¿La gente con niñes teme que toquen accidentalmente las hornallas delanteras
y por eso usan más las de atrás? Sí, pasa bastante, aunque no pasan a ser
mayoría. También varias personas comentaron que les quedó la costumbre aún
cuando ya no tiene a pequeñes.

![
Hornalla favorita según presencia de niñes menores.
Gente con niñes que prefiere una hornalla adelante: 670,
Gente con niñes que prefiere una hornalla atrás: 524,
Gente sin niñes que prefiere una hornalla adelante: 2773,
Gente sin niñes que prefiere una hornalla atrás: 966
](ninyes.png)

### Se usan más las hornallas de atrás si la persona es alta

¿La gente alta prefiere las hornallas más atrás que la gente más baja? Sí, poco.
La gente que prefiere las hornallas de atrás son en general 2 cm más alta.

![
Preferencia de hornalla por altura.
Hornalla delantera Q1: 1.60,
Hornalla delantera Q2: 1.67,
Hornalla delantera Q3: 1.74,
Hornalla trasera Q1: 1.62,
Hornalla trasera Q2: 1.69,
Hornalla trasera Q3: 1.76,
](altura.png)

### Se usa más la de adelante si se prende con encendedor

Sería más cómodo usar el encendedor más "cerca".

![
Hornalla favorita según uso de encendedor.
Usa encendedor, prefiere hornalla delantera: 831,
Usa encendedor, prefiere hornalla trasera: 289,
No usa encendedor, prefiere hornalla delantera: 2045,
No usa encendedor, prefiere hornalla trasera: 1009
](encendedor.png)

### Se usa más la hornalla más fuerte

Las hornallas más fuertes suelen ser preferida a las demás.

![
Hornallas de intensidad alta favoritas.
Proporción de hornallas de intensidad alta 3/4: 0.81,
Proporción de hornallas de intensidad alta 2/3: 0.85,
Proporción de hornallas de intensidad alta 1/2 o 2/4: 0.67,
Proporción de hornallas de intensidad alta 1/3: 0.59,
Proporción de hornallas de intensidad alta 1/4: 0.47,
](intensidad.png)

### La edad no es predictora de la hornalla favorita

A priori la edad parece predecir una preferencia por hornallas traseras.

![
Preferencia de hornalla por edad
Hornalla delantera Q1: 24,
Hornalla delantera Q2: 28,
Hornalla delantera Q3: 35,
Hornalla trasera Q1: 25,
Hornalla trasera Q2: 31,
Hornalla trasera Q3: 39,
](edad0.png)

Pero una vez que nos quedamos sólo con gente que no tiene hijes menores, esta
diferencia desaparece.

![
Preferencia de hornalla por edad (sin hijes)
Hornalla delantera Q1: 23,
Hornalla delantera Q2: 27,
Hornalla delantera Q3: 33,
Hornalla trasera Q1: 24,
Hornalla trasera Q2: 28,
Hornalla trasera Q3: 35,
](edad1.png)

### Los hombres tienen más preferencia de la hornalla de mayor intensidad

No encontramos diferencia sustanciales entre ambos géneros en este aspecto.

### El género no predice la preferencia de la hornalla

Los hombres demuestran usar más las hornallas traseras. Sin embargo, al
controlar por niñes la tendencia desaparece.

## Modelo explicativo

Si queremos ver qué hay que considerar para determinar la hornalla favorita de
alguien podemos dividir el problema en dos partes.

Usamos un modelo sencillo de aprendizaje automático para determinar reglas.

### Profundidad

Se prefiere una hornalla delantera siempre y cuando la hornalla de mayor
intensidad no esté atrás y no hayan niñes en la casa.

### Lateralidad

En este caso el modelo fue más "creativo", por decirlo de alguna manera.

Se prefiere una hornalla de la izquierda si ocurre cualquiera de las siguientes
condiciones:

* La hornalla de mayor intensidad está a la izquierda y hay mesada hacia la
izquierda.
* La hornalla de mayor intensidad está adelante y hay mesada hacia la izquierda
pero no hacia la derecha.
