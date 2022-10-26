# MANUAL DE MARKDOWN
### ÍNDICE
1. [ELEMENTOS DE BLOQUE](#Encabezado1)
    1. [PÁRRAFOS Y SALTOS DE LÍNEA](#Encabezado11)
    2. [ENCABEZADOS](#Encabezado12)
    3. CITAS
    4. LISTAS
    5. CÓDIGOS DE BLOQUE
    6. REGLAS HORIZONTALES
2. ELEMENTOS DE LÍNEA
    1. ÉNFASIS
    2. LINKS O ENLACES
    3. CÓDIGO
    4. IMÁGENES 
3. ELEMENTOS VARIOS
    1. LINKS AUTOMÁTICOS
    2. OMITIR MARKDOWN
4. MULTIMARKDOWN (MMD)
    1. ABREVIACIONES
    2. DEFINICIONES
    3. METADATOS
    4. NOTAS AL PIE DE PÁGINA
    5. REFERENCIAS CRUZADAS
    6. TABLAS

### ELEMENTOS DE BLOQUE<a name="Encabezado1"></a>
#### PÁRRAFOS Y SALTOS DE LÍNEA<a name="Encabezado11"></a>
Para generar un nuevo párrafo en Markdown simplemente separa el texto mediante una línea en blanco **(pulsando dos veces intro)**

Al igual que sucede con HTML, **Markdown no soporta dobles líneas en blanco**, así que si intentas generarlas estas se convertirán en una sola al procesarse.

Para realizar un salto de línea y empezar **una frase en una línea siguiente dentro del mismo párrafo**, tendrás que pulsar **dos veces la barra espaciadora antes de pulsar una vez intro**.

Por ejemplo si quisieses escribir un poema Haiku quedaría tal que así:

*"Andando con sus patitas mojadas,  
el gorrión  
por la terraza de madera"*

Donde cada verso tiene dos espacios en blanco al final.

#### ENCABEZADOS<a name="Encabezado12"></a>

Las # almohadillas son uno de los métodos utilizados en Markdown para crear encabezados. Debes usarlos añadiendo uno por cada nivel.

Es decir,
~~~
# Encabezado 1
## Encabezado 2 
### Encabezado 3
#### Encabezado 4
##### Encabezado 5 
###### Encabezado 6
~~~
Se corresponde con  
# Encabezado 1  
## Encabezado 2  
### Encabezado 3  
#### Encabezado 4  
##### Encabezado 5  
###### Encabezado 6
También puedes cerrar los encabezados con el mismo número de almohadillas, por ejemplo escribiendo ### Encabezado 3 ###. Pero la única finalidad de esto es un **motivo estético**.

Existe otra manera de generar encabezados, aunque este método está **limitado a dos niveles**.

Consiste en subrayar los encabezados con el símbolo = (para el encabezado 1), o con guiones - para el encabezado 2

Es decir, 

Esto sería el encabezado 1
=
Esto sería el encabezado 2
-

No existe un número concreto = o - que necesites escribir para que esto funcione, ¡incluso bastaría con uno!

#### CITAS
Las citas se generar utilizando el carácter mayor que > al comienzo del bloque de texto.

> Un país, una civilización se puede juzgar por la forma en que trata a sus animales.  — Mahatma Gandhi

Si la cita en cuestión se compone de varios párrafos, deberás añadir el mismo símbolo > al comienzo de cada uno de ellos.

> Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma extraordinariamente peligrosa el sano intelecto animal.  
> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora, al animal infeliz. — Friedrich Nietzsche

Incluso puedes concatenar varios símbolos >> para crear citas anidadas.

> Esto sería una cita como la que acabas de ver.
> 
>> Dentro de ella puedes anidar otra cita.
> 
> La cita principal llegaría hasta aquí. 

Recuerda separar los saltos de línea con >, o >> si te encuentras dentro de la cita anidada; para crear párrafos dentro del mismo bloque de cita.


#### LISTAS

En markdown existen 2 tipos de listas.

##### LISTAS DESORDENADAS
Para crear listas desordenadas utiliza * **asteriscos**, - **guiones**, o + **símbolo de suma**.  
\* Elemento 1  
\- Elemento 2  
\+ Elemento 3  

Da igual qué elemento escojas, incluso puedes intercambiarlos. Todos se verán igual al procesarse.
* Elemento 1
- Elemento 2
+ Elemento 3

Para generar **listas anidadas** dentro de otras, simplemente tendrás que identar el texto pulsado la tecla tabulador antes de *, - o +.

* Elemento 1
    *  Elemento 2
        * Elemento 3

##### LISTAS ORDENADAS
Para crear listas ordenadas debes utilizar la sintaxis de tipo: *"número."* 1.. Al igual que ocurre con las listas desordenadas, también podrás **anidarlas** o **combinarlas**.
1. Elemento 1
    1. Elemento 2
        1. Elemento 3
#### CÓDIGOS DE BLOQUE
Si quieres crear un bloque entero que contenga código. Lo único que tienes que hacer es encerrar dicho párrafo entre dos líneas formadas por tres ~ virgulillas.

Tal que así:

\~~~  
Creando códigos de bloque.  
Puedes añadir tantas líneas y párrafos como quieras.  
\~~~


~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.  
~~~
#### REGLAS HORIZONTALES
Las reglas horizontales se utilizan para separar secciones de una manera visual. Las estás viendo constantemente en este artículo ya que las estoy utilizando para separar los diferentes elementos de sintaxis de Markdown.

Para crearlas, en una línea en blanco deberás incluir **tres de los siguientes elementos**: asteriscos, guiones, o guiones bajos.

Es decir

~~~
***
---
___
~~~
También puedes separarlos mediante un espacio en blanco por pura estética.
~~~
* * *
- - -
_ _ _
~~~
***
### ELEMENTOS DE LÍNEA
#### ÉNFASIS (NEGRITAS Y CURSIVAS)
Markdown utiliza asteriscos o guiones bajos para enfatizar.

Simplemente tendrás que envolver palabras o textos en éstos símbolos para conseguir *cursivas* o **negritas**.

|Markdown|Resultado|
|--|--|
|\*cursiva*|*cursiva*|
|\_cursiva_|_cursiva_|
|\*\*negrita\*\*|**negrita**|
|\_\_negrita\_\_|__negrita__|
|\~\~tachado\~\~|~~tachado~~|

Por supuesto si quieres utilizar los dos tipos de énfasis no tienes más que combinar la sintaxis, envolviendo la palabra entre tres asteriscos o tres guiones bajos.
|Markdown|Resultado|
|--|--|
|\*\*\*cursiva y negrita\*\*\*|***cursiva y negrita***|
|\_\_\_cursiva y negrita\_\_\_|___cursiva y negrita___|

Este *texto* contiene varios **formatos**, incluso puedo ~~***combinar***~~ distintos formatos.
#### LINKS O ENLACES
Añadir enlaces a una publicación, más que común, hoy en día es algo casi obligatorio. Con Markdown tendrás varias formas de hacerlo.
##### LINKS O ENLACES EN LÍNEA
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] **corchetes**, y el link en cuestión entre () **paréntesis**.

[Enlace de ejemplo](https://markdown.es/)

##### LINKS O ENLACES COMO REFERENCIA
La desventaja del método anterior, es que si utilizas links demasiado complejos o largos pueden dificultarte la lectura de tu texto.

Para solucionarlo y crear tu contenido de una manera más ordenada puedes generar enlaces de referencia.

Esto quiere decir que en tu texto enlazarás ***palabras o códigos concretos*** (formados por letras y/o números), que en otro lugar más apartado de tu documento tendrás definidos como determinadas URL.

Esto se ve más claro en este ejemplo.

~~~
Una de la principales ayudas para las personas que empiezan en el mundo de la programación es esta [web][link].  
Esta [web][link] contiene información sobre el tipado de distintos lenguajes de programación.  
[link]: https://www.w3schools.com/
~~~
Una de la principales ayudas para las personas que empiezan en el mundo de la programación es esta [web][link].  
Esta [web][link] contiene información sobre el tipado de distintos lenguajes de programación.  

[link]: https://www.w3schools.com/

``<html><body><p>Este es un texto en html</p></body></html>``

|Columna1|Columna2|
|--|--|
|1|2|
|3|4|

Para más info pulsa [aquí](https://markdown.es/)

![Logo](https://es.wikipedia.org/wiki/Markdown#/media/Archivo:Markdown-mark.svg "Logo")



## Encabezado en el documento {#EncabezadoReferencia}
En un texto cuaquiera se añade [un enlace al encabezado](#EncabezadoReferencia) definido en el ejemplo anterior.



[def]: REFERENCIA12