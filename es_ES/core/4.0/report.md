Esta página le permite ver todos los informes generados por la acción del informe (consulte la documentación del escenario).

# ¿Qué es un informe? ?

Un informe es una captura de pantalla de la interfaz Jeedom en un instante T (la captura está adaptada para no tomar la barra de menú y otro elemento inútil en este tipo de un).

Puede hacer esto en vistas, diseño, página de panel....

Se activa desde un escenario con el comando de informe, puede elegir que se le envíe este informe mediante un comando de mensaje (correo electrónico, telegrama, etc.)

# un

Su un es muy simple, selecciona si quieres ver :

-	ver informes
-	informes de degins
-	informes del panel de complementos
- Informes del equipo (para un resumen de la batería de cada módulo)

Luego selecciona el nombre del informe en cuestión y verá todas las fechas de los informes en la memoria

> **importante**
>
> La eliminación automática se realiza de forma predeterminada para informes de más de 30 días (puede configurar este período en la configuración de Jeedom)

Una vez que el informe seleccionado puede verlo aparecer, vuelva a descargarlo o elimínelo.

También puede eliminar todas las copias de seguridad de un informe determinado

# Preguntas frecuentes

> **Si tienes un error de Detalles : cutycapt: error al cargar bibliotecas compartidas: libEGL.n: no se puede abrir el archivo de objeto compartido: No existe tal archivo o directorio**
>
> Es necesario en ssh o en Administración -&gt; Configuración -&gt; OS / DB -&gt; Sistema -&gt; Administración para hacer :
>sudo ln -s /usr/lib/aarch64-linux-gnu/libGLESv2.n.2 /usr/lib/aarch64-linux-gnu/libGLESv2.n
>sudo ln -s /usr/lib/aarch64-linux-gnu/libEGL.n.1 /usr/lib/aarch64-linux-gnu/libEGL.n