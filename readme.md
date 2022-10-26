# MANUAL DE MARKDOWN (CHEAT SHEET)
### ÍNDICE
1. [ELEMENTOS DE BLOQUE](#Encabezado1)
    1. [PÁRRAFOS Y SALTOS DE LÍNEA](#Encabezado11)
    2. [ENCABEZADOS](#Encabezado12)
    3. [CITAS](#Encabezado13)
    4. [LISTAS](#Encabezado14)
        1. [LISTAS DESORDENADAS](#Encabezado141)
        2. [LISTAS ORDENADAS](#Encabezado142)
    5. [CÓDIGOS DE BLOQUE](#Encabezado15)
    6. [REGLAS HORIZONTALES](#Encabezado16)
2. [ELEMENTOS DE LÍNEA](#Encabezado2)
    1. [ÉNFASIS](#Encabezado21)
    2. [LINKS O ENLACES](#Encabezado22)
        1. [LINKS O ENLACES EN LÍNEA](#Encabezado221)
        2. [LINKS O ENLACES COMO REFERENCIA](#Encabezado222)
        3. [LINKS AUTOMÁTICOS](#Encabezado223)
    3. [CÓDIGO](#Encabezado23)
        1. [CODIGO PURO `<code>`](#Encabezado231)
        2. [TEXTO PREFORMATEADO `<pre>`](#Encabezado232)
    4. [IMÁGENES](#Encabezado24)
3. [OMITIR MARKDOWN](#Encabezado3)
4. [MULTIMARKDOWN (MMD)](#Encabezado4)
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

#### CITAS<a name="Encabezado13"></a>
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


#### LISTAS<a name="Encabezado14"></a>

En markdown existen 2 tipos de listas.

##### LISTAS DESORDENADAS<a name="Encabezado141"></a>
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

##### LISTAS ORDENADAS<a name="Encabezado142"></a>
Para crear listas ordenadas debes utilizar la sintaxis de tipo: *"número."* 1.. Al igual que ocurre con las listas desordenadas, también podrás **anidarlas** o **combinarlas**.
1. Elemento 1
    1. Elemento 2
        1. Elemento 3
#### CÓDIGOS DE BLOQUE<a name="Encabezado15"></a>
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
#### REGLAS HORIZONTALES<a name="Encabezado16"></a>
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
### ELEMENTOS DE LÍNEA<a name="Encabezado2"></a>
#### ÉNFASIS (NEGRITAS Y CURSIVAS)<a name="Encabezado21"></a>
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
#### LINKS O ENLACES<a name="Encabezado22"></a>
Añadir enlaces a una publicación, más que común, hoy en día es algo casi obligatorio. Con Markdown tendrás varias formas de hacerlo.
##### LINKS O ENLACES EN LÍNEA<a name="Encabezado221"></a>
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] **corchetes**, y el link en cuestión entre () **paréntesis**.

[Enlace de ejemplo](https://markdown.es/)

##### LINKS O ENLACES COMO REFERENCIA<a name="Encabezado222"></a>
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
##### LINKS AUTOMÁTICOS<a name="Encabezado223"></a>
Estos son necesarios cuando lo que quieres es **mostrar una URL completa**, y no un enlace enmascarado bajo una palabra o frase como ocurre con los links en línea.

Para generar links automáticos tan solo tendrás que rodearlos con los símbolos < >
~~~
<https://www.w3schools.com/>
~~~
<https://www.w3schools.com/>
#### CÓDIGO<a name="Encabezado23"></a>
En según que tipo de publicaciones (sobre todo las de carácter técnico), necesitarás añadir pequeñas secciones donde mostrar código de otro lenguaje, atajos de teclado, o demás contenido que no debería ser tratado como tal.

Para ello tienes disponible dos alternativas.
##### CÓDIGO PURO `<code>`<a name="Encabezado231"></a>
La forma más sencilla de escribir código en Markdown es envolver el texto entre dos comillas sencillas \`. Esto se corresponde con la etiqueta HTML `<code>`
~~~
`<script src="script.js"></script>`
~~~
Asi se verá el codigo
`<script src="script.js"></script>`

Como ves, es muy útil para introducir código dentro de la misma línea o párrafo, algo que no permite el método siguiente
##### TEXTO PREFORMATEADO `<pre>`<a name="Encabezado232"></a>
La otra manera de añadir código en Markdown es **comenzar el párrafo con cuatro espacios en blanco**. Esto se corresponde con la etiqueta HTML `<pre>`
~~~
    <script src="script.js"></script>
~~~
Esto se convierte en

    <script src="script.js"></script>
Estos espacios deberás incluirlos **en cada línea que escribas**. Para añadir código en bloque es mejor utilizar la sintaxis que viste anteriormente: códigos de bloque.
#### IMÁGENES
Insertar una imagen con Markdown se realiza de una manera prácticamente idéntica a insertar [links](#Encabezado221).

Solo que en este caso, deberás añadir un símbolo de ! **exclamación** al principio y el **enlace** no será otro que **la ubicación de la imagen**.
~~~
![Texto alternativo](/ruta/a/la/imagen.jpg)
~~~
El *texto alternativo* es lo que se mostraría si la carga de la imagen fallase.
También podrás añadir un **título alternativo** entrecomillándolo al final de la ruta. Esto sería el título mostrado al dejar el cursor del ratón sobre la imagen.
~~~
![Texto alternativo](/ruta/a/la/imagen.jpg "Título alternativo")
~~~
Ya que al añadir imágenes también estás tratando con URLs, puedes utilizar el método que viste anteriormente para }}**incluir links mediante referencias**, solo que en este caso **los enlaces de referencia serán aquellos donde se encuentre tu imagen**.

De esta forma podrias insertar una imagen
~~~
![nombre de la imagen][img1]
O dos, sin ensuciar tu espacio de escritura.
![nombre de la imagen2][img2] 
[img1]: /ruta/a/la/imagen.jpg "Título alternativo"
[img2]: /ruta/a/la/imagen2.jpg "Título alternativo"
~~~
### OMITIR MARKDOWN<a name="Encabezado3"></a>
 En Markdown **es posible escribir ciertos símbolos** como * asteriscos o _ guiones bajos, sin que los interprete para convertirlos en negritas, cursivas…

Esto es muy sencillo, ya que en este lenguaje existe un elemento estrella para especificar que todo lo que escribas a continuación, no se interprete como Markdown.

Se trata de la barra invertida \\.

**Escribiéndola justo delante** de cualquiera de los elementos que verás a continuación, los mismos **no tendrán efecto** a la hora de convertirse en negritas, cursivas, links…
~~~
\  barra invertida
`  acento invertido
*  asterisco
_  guión bajo
{} llaves
[] corchetes
() paréntesis
#  almohadilla
+  símbolo de suma
-  guión
.  punto
!  exclamación
~~~
### MULTIMARKDOWN (MMD)<a name="Encabezado4"></a>
Multimarkdown (también conocido como MMD), nació de la necesidad de **Fletcher Penney** de escribir documentos académicos utilizando Markdown.

Así que este lenguaje no solo incluye todas las características que has visto anteriormente en la sintaxis de Markdown, sino que **vitamina** esta última añadiendo la capacidad de escribir **notas al pie de página, tablas, o metadatos**.

**No todas las aplicaciones soportan Multimarkdown**.

Así que si intentas utilizar este tipo de sintaxis y no obtienes los resultados esperados, comprueba que la aplicación/servicio donde estás escribiendo ofrece dicho soporte.
#### ABREVIACIONES<a name="Encabezado41"></a>
Si en tus artículos utilizas muchas abreviaciones, puede ser un incordio tener que explicarlas siempre (por ejemplo, entre paréntesis) a nuevos lectores.

Para evitarlo, puedes definir abreviaciones en Multimarkdown utilizando la siguiente sintaxis.
~~~
MMD ofrece muchas más posibilidades que MD.
*[MMD]: Abreviación para Multimarkdown
*[MD]: Abreviación para Markdown
~~~
Si te fijas, es igual que cuando creabas links de referencia, solo que en este caso precedidos por un asterisco.

*[MMD]: Abreviación para Multimarkdown
*[MD]: Abreviación para Markdown

Para descubrir cuál es el resultado final, no tienes más que **dejar el puntero del ratón sobre la palabra [MMD] o [MD]**.
[MMD] ofrece muchas más posibilidades que [MD].
|Columna1|Columna2|
|--|--|
|1|2|
|3|4|

Para más info pulsa [aquí](https://markdown.es/)

![Logo](https://es.wikipedia.org/wiki/Markdown#/media/Archivo:Markdown-mark.svg "Logo")




[def]: REFERENCIA12