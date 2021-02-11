---
unique-page-id: 14746594
description: Configuración de un servidor SMTP - Documentos de marketing - Documentación del producto
title: Configuración de un servidor SMTP
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# Configuración de un servidor SMTP {#setting-up-an-smtp-server}

## Información general {#overview}

**¿Qué es un servidor SMTP?**

**** Simple  **** Mail  **** Transfer  **** Protocol, este es el servidor responsable de enviar su correo saliente. Cuando envía un correo electrónico desde el cliente de correo electrónico, está utilizando este mismo servicio para enviar el correo electrónico.

**¿Por qué deseo configurar mi servidor SMTP con Sales Connect?**

Le permite utilizar la reputación del dominio y la capacidad de entrega de su compañía, y no tener que depender de los demás. Nuestros servidores MSC predeterminados forman parte de un grupo de IP compartido, lo que significa que se envían desde una reputación compartida. Le recomendamos encarecidamente que su equipo configure su propio canal de envío con Sales Connect.

**¿Cómo envía Sales Connect con mi servidor SMTP?**

Siguiendo [estos pasos](http://docs.marketo.com/x/ZgPh).

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **¿Debo configurar algo en mi cliente de correo electrónico?**

En lo que respecta a un canal de envío, no. Una vez que haya instalado nuestro complemento, Sales Connect aprovechará el mismo canal de envío que configuró para enviar correos electrónicos.

## Obtención de las credenciales SMTP {#getting-the-smtp-credentials}

**¿Cómo puedo obtener mis credenciales SMTP?**

Póngase en contacto con su equipo de TI para averiguar qué canal de envío utiliza su compañía para enviar correos electrónicos y cómo obtener acceso a sus credenciales SMTP. Según la configuración del servidor, puede tener algunos valores personalizados para el nombre del servidor SMTP o el puerto del servidor. Si no dispone de un equipo de TI dedicado, póngase en contacto con su proveedor de correo electrónico.

**¿Cuáles son mis opciones si mi compañía utiliza Office365?**

Pros

* Fácil de configurar
* Cualquier usuario con una cuenta de Office365 tendrá acceso a este servidor SMTP

Cons

* Se puede producir una limitación
* Cada usuario debe configurarlo por sí mismo
* Si se cambia la contraseña de O365 de un usuario, se interrumpirá la conexión

Si utiliza Office365 o Exchange Online, puede conectarse al servidor SMTP mediante un conjunto estándar de credenciales. Tenga en cuenta que Office365 no es un servicio de envío de correo electrónico masivo, aunque esto funcionará bien para enviar correos electrónicos únicos. Al enviar correos electrónicos masivos, Office365 puede reducir los correos electrónicos, lo que puede provocar errores en el envío. Para obtener más información sobre este artículo de Microsoft sobre [cómo configurar el envío de cliente SMTP](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4).

&quot;Sólo puede enviar desde una dirección de correo electrónico a menos que el dispositivo pueda almacenar las credenciales de inicio de sesión para varios buzones de Office 365. Office 365 impone un límite de 30 mensajes enviados por minuto y un límite de 10.000 destinatarios por día&quot;.

Si decide utilizar Office365 como canal de envío, deberá introducir estas credenciales. No se pueden usar las mismas credenciales en todo el equipo porque Office365 utiliza el correo electrónico y la contraseña del usuario para conectarse.

Envío masivo y de Microsoft

[Haga clic ](https://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) aquí para conocer el envío masivo en Office365.

Los clientes de Exchange Online que necesitan enviar correo electrónico comercial masivo legítimo (por ejemplo, boletines informativos de clientes) deben utilizar proveedores de terceros que se especialicen en estos servicios&quot;.

**¿Y si mi compañía usa Gmail?**

No necesitará obtener las credenciales SMTP si su equipo desea utilizar Gmail como canal de envío con Sales Connect. Sales Connect permite a los usuarios acceder a su canal de envío de Gmail mediante nuestra integración con OAuth. Los usuarios pueden activar esta opción integrando su cuenta de Sales Connect con Gmail.

![](assets/2.png)

**¿Puedo compartir las mismas credenciales SMTP con todo mi equipo?**

Esto depende del canal de envío que utilice. Por ejemplo, los servicios como Sparkpost permiten que las credenciales estén basadas en dominios, de modo que cualquiera que envíe con un dominio específico se autentica para enviarlas a través de ese servidor. Si este es el caso, entonces sí, puede compartir las credenciales con el equipo.

Si se está conectando a Office365, las credenciales se basan en direcciones de correo electrónico. Esto significa que solo la dirección de correo electrónico que estableció la conexión se autenticará para enviar correos electrónicos a través de ese canal de envío, por lo que las credenciales deben **no** compartirse.

![](assets/3.png)
