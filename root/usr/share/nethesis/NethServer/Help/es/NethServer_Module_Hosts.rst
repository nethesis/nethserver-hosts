==========
DNS y DHCP
==========

Gestión de alias de servidor, nombres de host y el servidor DHCP.

Servidor de alias
=================

Los alias son nombres alternativos para este servidor. Por ejemplo , si el nombre del servidor es *server.mycompany.com*, un alias puede ser *mail.mycompany.com*. El servidor utilizará su propia dirección IP para el nombre alias.

Crear / Modificar
-----------------

Permite crear un nuevo alias para este servidor.

Nombre del Host
    El nombre de host que desea agregar o modificar. Puede contener sólo letras, números y guiones y deben comenzar con una letra o un número.

Descripción
    Una descripción opcional útil para identificar el alias.

.. raw:: html

   {{{INCLUDE NethServer_Module_Hosts_*.html}}}


DNS
===

El DNS (Domain Name System) es responsable de la resolución de nombres de dominio (por ejemplo www.nethesis.it) en sus direcciones IP numéricas correspondientes (Ej. 10.11.12.13 ), y viceversa. Los delegados del servidor resolucionan los nombres a los servidores DNS configurados, pero usted puede especificar las direcciones de los nombres seleccionados arbitrarias. Por ejemplo, se puede configurar el sistema para responder a las solicitudes de facebook.com con la dirección IP 0.0.0.0 logrando el efecto de hacer que el sitio Facebook sea inalcanzable.

Configure
---------

Haga clic en Configurar para ingresar las direcciones de los servidores DNS que pondrá en contacto con el servidor para resolver nombres. 

DNS primario
    La dirección del servidor primario de contacto para la resolución de nombres (obligatorio).

DNS secundario
    La dirección del servidor secundario para ser contactado en caso de que el principal no este respondiendo (opcional). 

Crear / Modificar
-----------------

Haga clic en Crear para asignar un nombre de host a una dirección IP. El servidor devolverá la dirección IP configurada para solicitudes de su nombre. 


Nombre de host
    El nombre de dominio, por ejemplo www.nethesis.it . Es posible crear nombres para el dominio local, que es útil para dar un nombre nemotécnico para  dispositivos configurados con IP estática o para cualquier dominio, que prevalecen sobre el servidor DNS del ISP (véase facebook.com ejemplo anterior).

Dirección IP
    La dirección IP del nombre de host.

Descripción
    Un comentario opcional para el nombre de host (ejemplo: "Bloquear facebook" o "servidor de video").
