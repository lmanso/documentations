Ce plugin permet de piloter les modules Wattcubes de Wattlet via le
Wattcube Web.

configuración del plugin
=======================

Après téléchargement du plugin, il vous suffit juste d’activer celui-ci,
puis de configurer l’adresse IP du Wattcube Web.

![wattlet](../images/wattlet.png)

Configuración del dispositivo
=============================

La synchronisation des équipements Wattlets est accessible à partir du
menu Plugins :

![wattlet2](../images/wattlet2.png)

Une fois que vous cliquez sur l’un d’eux, vous obtenez :

![wattlet3](../images/wattlet3.png)

Aquí encontrará toda la configuración de su dispositivo:

-   **Nom de l’équipement Wattlet** : nom de votre équipement Wattlet
    sur le dashboard,

-   **Objeto padre** : especifica el objeto padre al que pertenece
    equipos,

-   ** ** Activar: para que su equipo activo,

-   ** ** visible hace que su equipo visible en el salpicadero,

-   **Catégorie** : catégorie de votre équipement Wattlet

Ainsi que les informations suivantes :

-   **Adresse** : Adresse du module,

-   **Type** : Type de module Wattlet,

-   **Version Software** : Version du logiciel interne du module
    Wattlet,

-   **Version Hardware** : Version du matériel

> **Note**
>
> Les commandes sont automatiquement créées, il n’est pas nécessaire de
> les rajouter manuellement.

Configuration du Wattcube Web 
=============================

Afin de récupérer les retours d’états, il est nécessaire de configurer
les notifications Push dans le Wattcube Web.

Dans l’interface du Wattcube Web, se rendre dans l’onglet "Préférences"
puis menu "Personnalisation de la commande"
image::../images/wattlet4.png\[\]

Dans la zone "Notification PUSH", entrer l’adresse de la Jeedom sous la
forme :

**IP\_JEEDOM/plugins/wattlet/core/php/jeeWattlet.php?id=~id~&cmd=~cmd~&state=~state~**

puis enregistrer.

![wattlet5](../images/wattlet5.png)
