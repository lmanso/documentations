Esta página le permite configurar la visualización de toda su domótica
muy bien. Lleva tiempo pero su único límite es
tu imaginación.

Es accesible por Inicio → Diseño

> **punta**
>
> Es posible ir directamente a un diseño gracias al submenú.

> **importante**
>
> Todas las acciones se realizan haciendo clic derecho en esta página, atención
> hacerlo bien en diseño. Durante la creación, por lo tanto, es necesario
> hacer en el medio de la página (para asegurarse de estar en el diseño).

En el menú (clic derecho, por lo tanto), encontramos el
siguientes acciones :

-   **diseños** : Muestra la lista de sus diseños y le permite acceder a ellos.

-   **edición** : Cambiar al modo de edición

-   **Pantalla completa** : Le permite usar toda la página web, que
    eliminará el menú Jeedom de la parte superior

-   **Añadir gráfico** : Agregar un gráfico

-   **Añadir texto / html** : Le permite agregar texto o código
    html / javascript

-   **Agregar escenario** : Agregar un escenario

-   **Agregar enlace**

    -   **Hacia una vista** : Agregar un enlace a una vista

    -   **Hacia un diseño** : Agregar un enlace a otro
        diseño

-   **Agregar equipo** : Agrega equipo

-   **Añadir pedido** : Agregar un pedido

-   **Añadir imagen / cámara** : Le permite agregar una imagen o transmisión
    de una camara

-   **Agregar área** : Agregar un área transparente en la que se pueda hacer clic
    quién puede ejecutar una serie de acciones con un clic (dependiendo
    o no el estado de otro pedido)

-   **Agregar resumen** : Agrega información de un resumen de objeto o
    general

-   **Viendo**

    -   **no** : No muestra ninguna cuadrícula

    -   **10x10** : Muestra una cuadrícula de 10 por 10

    -   **15x15** : Muestra una cuadrícula de 15 por 15

    -   **20x20** : Muestra una cuadrícula de 20 por 20

    -   **Magnetizar los elementos** : Añadir una magnetización entre
        elementos para que sea más fácil pegarlos

    -   **Imán en la rejilla** : Agregue una magnetización de los elementos a
        la cuadrícula (atención : dependiendo del zoom del artículo esto
        la funcionalidad puede funcionar más o menos)

    -   **Ocultar elemento resaltado** : Ocultarlo
        resaltar alrededor de elementos

-   **Eliminar diseño** : eliminar diseño

-   **Crea un diseño** : permite agregar un nuevo diseño

-   **Diseño duplicado** : duplicar el diseño actual

-   **Configura el diseño** : acceso a la configuración de diseño

-   **Guardar** : permite guardar el diseño (atención, hay
    también copias de seguridad automáticas durante ciertas acciones)

> **importante**
>
> La configuración de los elementos de diseño se realiza haciendo clic en
> estos.

Configuración de diseño 
=======================

Encontrado aquí :

-   **general**

    -   **apellido** : El nombre de su diseño

    -   **Fondo transparente** : hace que el fondo sea transparente. Tenga cuidado si el
        la casilla está marcada, no se utiliza el color de fondo

    -   **Color de fondo** : diseño de color de fondo (blanco
        por defecto)

    -   **código** : Código de acceso a su diseño (si está vacío, sin código
        no es solicitado)

    -   **icono** : Un icono para ello (aparece en el menú
        elección de diseño)

    -   **imagen**

        -   **enviar a** : permite agregar una imagen de fondo al diseño

        -   **Eliminar imagen** : borrar imagen

-   **tamaños**

    -   **Tamaño (WxH)** : Le permite fijar el tamaño de su diseño.
        (marco gris en modo edición)

Configuración general de elementos. 
===================================

> **nota**
>
> Dependiendo del tipo de elemento, las opciones pueden cambiar.

> **nota**
>
> El elemento seleccionado se resalta en rojo (en lugar de verde
> para todos los demás).

Ajuste de la pantalla 
---------------------

-   **profundidad** : permite elegir el nivel de profundidad

-   **Posición X (%)** :

-   **Posición Y (%)** :

-   **Ancho (px)** :

-   **Altura (px)** :

remove 
---------

Eliminar elemento

duplicado 
---------

Le permite duplicar el elemento.

cerradura 
-----------

Bloquea el elemento para que ya no sea móvil o
de tamaño variable.

gráfico 
=========

Configuraciones de pantalla 
---------------------

-   **período** : le permite elegir el período de visualización

-   **Mostrar subtítulo** : mostrar leyenda

-   **Mostrar navegador** : mostrar el navegador (segundo gráfico
    más claro debajo del primero)

-   **Mostrar selector de período** : muestra el selector
    periodo arriba a la izquierda

-   **Mostrar barra de desplazamiento** : muestra la barra de desplazamiento

-   **Fondo transparente** : hace que el fondo sea transparente

-   **frontera** : agregue un borde, tenga cuidado con la sintaxis
    HTML (tenga cuidado, debe usar la sintaxis CSS, por ejemplo :
    sólido 1px negro)

Configuración avanzada 
---------------------

Le permite elegir los comandos para graficar

Text / html 
=========

-   **icono** : Icono para mostrar en frente

-   **Color de fondo** : le permite cambiar el color de fondo o
    poner transparente, no olvide pasar &quot;Predeterminado&quot; en NO

-   **Color del texto** : le permite cambiar el color de los íconos y
    textos (tenga cuidado de pasar Predeterminado a No)

-   **Alrededor de los ángulos** : le permite redondear los ángulos (no
    olvide poner%, ex 50%)

-   **frontera** : agregue un borde, tenga cuidado con la sintaxis
    HTML (use la sintaxis CSS, por ejemplo : sólido
    1px negro)

-   **Tamaño de fuente** : le permite cambiar el tamaño de fuente
    (ex 50%, debe poner el signo%)

-   **Alineación de texto** : le permite elegir la alineación de
    texto (izquierda / derecha / centrado)

-   **grasa** : texto en negrita

-   **texto** : Texto en código HTML que estará en el elemento

> **importante**
>
> Si coloca código HTML (especialmente Javascript), tenga cuidado
> para comprobarlo antes porque puedes hacerlo si hay un error
> o si sobrescribe un componente de Jeedom que bloquea completamente el diseño y
> todo lo que tienes que hacer es eliminarlo directamente de la base de datos

guión 
========

Configuraciones de pantalla 
---------------------

No hay configuraciones de visualización específicas

enlace 
====

Configuraciones de pantalla 
---------------------

-   **apellido** : apellidobre del enlace (texto mostrado)

-   **enlace** : Enlace al diseño o vista en cuestión

-   **Color de fondo** : le permite cambiar el color de fondo o
    poner transparente, no olvide pasar &quot;Predeterminado&quot; en NO

-   **Color del texto** : le permite cambiar el color de los íconos y
    textos (tenga cuidado de pasar Predeterminado a No)

-   **Redondee los ángulos (no olvide poner%, ex 50%)** :
    le permite redondear los ángulos, no olvide poner el%

-   **Borde (sintaxis CSS de atención, ej. : sólido 1px negro)** : permite
    agregue un borde, tenga cuidado con la sintaxis es HTML

-   **Tamaño de fuente (ex 50%, debe poner el signo%)** :
    le permite cambiar el tamaño de fuente

-   **Alineación de texto** : le permite elegir la alineación de
    texto (izquierda / derecha / centrado)

-   **grasa** : texto en negrita

equipo 
==========

Configuraciones de pantalla 
---------------------

No hay configuraciones de visualización específicas

Configuración avanzada 
---------------------

Muestra la ventana de configuración avanzada del equipo (ver
documentación Resumen de automatización del hogar (&quot;pantalla&quot;))

orden 
========

Configuraciones de pantalla 
---------------------

No hay configuraciones de visualización específicas

Configuración avanzada 
---------------------

Muestra la ventana de configuración avanzada del comando (ver
documentación Resumen de automatización del hogar (&quot;pantalla&quot;))

imagenn / Cámara 
============

Configuraciones de pantalla 
---------------------

-   **visualización** : define lo que desea mostrar, imagen fija o
    transmitir desde una cámara

-   **imagen** : le permite enviar la imagen en cuestión (si tiene
    elige una imagen)

-   **cámara** : cámara para mostrar (si elige cámara)

zona 
====

Configuraciones de pantalla 
---------------------

-   **puntao de area** : Aquí es donde eliges el tipo de área :
    Macro individual, macro binaria o widget al pasar el mouse

### Macro individual 

En este modo, un clic en la zona realiza una o más acciones.

Aquí solo debe indicar la lista de acciones que debe hacer al hacer clic
en la zona

### Macro binaria 

En este modo, Jeedom ejecutará las acciones de encendido o apagado en
dependiendo del estado del pedido que da. ex : si el pedido
es 0, entonces Jeedom ejecutará la (s) acción (es) On (s) de lo contrario se ejecutará
la (s) acción (es) Off

-   **Información binaria** : Comando que da el estado a verificar
    decidir qué acción tomar (activar o desactivar)

Solo tiene que poner las acciones a realizar para
para el apagado

### Widget de desplazamiento 

En este modo, al pasar el mouse o al hacer clic en el área Jeedom, usted
mostrar el widget en cuestión

-   **equipo** : widget para mostrar al pasar el mouse o al hacer clic

-   **Mostrar en paso elevado** : si está marcado, muestra el widget al pasar el mouse

-   **Ver en un clic** : si está marcado, el widget se muestra en
    clic

-   **posición** : le permite elegir la ubicación donde
    widget (predeterminado abajo a la derecha)

resumen 
======

-   **enlace** : Se utiliza para indicar el resumen que se mostrará (General para
    global si no indica el objeto)

-   **Color de fondo** : le permite cambiar el color de fondo o
    poner transparente, no olvide pasar &quot;Predeterminado&quot; en NO

-   **Color del texto** : le permite cambiar el color de los íconos y
    textos (tenga cuidado de pasar Predeterminado a No)

-   **Redondee los ángulos (no olvide poner%, ex 50%)** :
    le permite redondear los ángulos, no olvide poner el%

-   **Borde (sintaxis CSS de atención, ej. : sólido 1px negro)** : permite
    agregue un borde, tenga cuidado con la sintaxis es HTML

-   **Tamaño de fuente (ex 50%, debe poner el signo%)** :
    le permite cambiar el tamaño de fuente

-   **grasa** : texto en negrita


Preguntas frecuentes 
======

>**Ya no puedo editar mi diseño**
>
>Si ha colocado un widget o una imagen que toma casi todo el diseño, debe hacer clic fuera del widget o imagen para acceder al menú haciendo clic con el botón derecho.

>**Eliminar un diseño que ya no funciona**
>
>En la parte de administración y luego en OS / DB, &quot;seleccione * de planHeader&quot;, obtenga la identificación del diseño en cuestión y haga una &quot;eliminación de planHeader donde id = # TODO #&quot; y &quot;eliminar del plan donde planHeader_id = # todo # &quot;reemplazando # TODO # con la identificación de diseño encontrada previamente.
