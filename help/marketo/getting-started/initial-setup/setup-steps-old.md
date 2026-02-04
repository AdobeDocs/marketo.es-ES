---
unique-page-id: 2949469
description: 'Pasos de configuración, documentos de Marketo: documentación del producto'
title: Pasos de configuración
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2086'
ht-degree: 69%

---

# Pasos de configuración {#setup-steps}

**Le damos la bienvenida a Adobe Marketo Engage.**

Antes de profundizar en el uso de Marketo, debe completar algunos pasos.

Estos pasos incluyen lo siguiente:

* Alguna configuración básica de la cuenta
* Personalizar la marca de las direcciones URL de la página de aterrizaje y los vínculos de correo electrónico para mejorar la confianza y la capacidad de envío
* Sincronizar su CRM
* Añadir un código de seguimiento al sitio web corporativo

>[!NOTE]
>
>Solo debe seguir estos pasos si su compañía es **nueva en Marketo**. Si no es así, es posible que la configuración ya esté lista.

Algunos pasos requieren la ayuda de su equipo de TI.

>[!TIP]
>
>Si [imprime esta lista de comprobación](/help/marketo/getting-started/initial-setup/setup-checklist.md){target="_blank"}, puede quitar elementos a medida que los complete.

## Inicie sesión y cree usuarios de Marketo adicionales {#log-in-and-create-additional-marketo-users}

>[!IMPORTANT]
>
>Si tu suscripción a Marketo se creó el 31 de julio de 2023 o después, o ya se ha migrado a [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}, no se te aplicarán los pasos para agregar un usuario que se describen a continuación. Consulte [este artículo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"} en su lugar.

Inicie sesión en Marketo [aquí](https://app.marketo.com/){target="_blank"} con las credenciales que recibió por correo electrónico.

![](assets/setup-steps-1.png)

¡Felicidades! Ahora está en Marketo y puede empezar a explorar. Es posible que desee invitar a sus compañeros del equipo de marketing para que se unan a usted. Para ello, agregue nuevos usuarios.

Vaya al área de **[!UICONTROL Admin]**.

>[!TIP]
>
>Mientras estás aquí, puedes hacer clic en **[!UICONTROL Mi cuenta]** para cambiar la configuración de la cuenta y la ubicación, así como para establecer un nuevo nombre de suscripción.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Se requieren permisos de administrador**

Haga clic en **[!UICONTROL Usuarios y funciones]**.

![](assets/setup-steps-3.png)

Haga clic en **[!UICONTROL Invitar nuevo usuario]**.

![](assets/setup-steps-4.png)

Rellene la dirección de correo electrónico, el nombre y los apellidos de sus compañeros. _Establecer una fecha de caducidad para el acceso es opcional_. Haga clic en **[!UICONTROL Siguiente]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Una fecha de caducidad es ideal para partes interesadas externas o consultores a corto plazo que solo necesitan acceso a Marketo durante un breve periodo.

>[!NOTE]
>
>Cuando llega la fecha de caducidad, el usuario recibe una notificación de caducidad y la cuenta se bloquea.

Seleccione un rol y haga clic en **[!UICONTROL Siguiente]**. Los usuarios estándar tienen acceso a todas las áreas excepto a la de Administración.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Además de las cinco funciones integradas, también puede crear funciones personalizadas. Más información acerca de [Administrar roles de usuario y permisos](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

No dude en modificar el texto de la invitación. Haga clic en **Enviar**.

![](assets/setup-steps-7.png)

El nuevo usuario aparece ahora en la ficha **[!UICONTROL Usuarios]** y debería recibir un correo electrónico con un vínculo para crear una contraseña y un inicio de sesión. ¡Siguiente paso!

![](assets/setup-steps-8.png)

## Configure Los Contactos De Soporte Autorizados {#set-up-your-authorized-support-contacts}

Es posible que el Soporte de Marketo le haya enviado un correo electrónico en el que se indica que es el administrador de Soporte al cliente de Marketo de su empresa. Si es así, puedes configurar **contactos de soporte autorizados** para tu equipo. Solo los contactos de asistencia autorizados pueden ponerse en contacto con la Asistencia al cliente de Marketo directamente a través del [Portal de asistencia de Marketo](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>El número de contactos de asistencia que puede crear está determinado por el paquete que ha adquirido. Este límite se especifica en el correo electrónico del Soporte técnico de Marketo.

Los documentos de contacto de asistencia autorizados se han trasladado a la Comunidad de Marketo. Consulte [este artículo](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>En la lista solo aparecen las personas que han iniciado sesión en la Comunidad de Marketo. Si no encuentra a la persona, asegúrese de que inicia sesión en la comunidad primero.

## Personalización de las direcciones URL de su página de destino con un CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada inicial.

>[!NOTE]
>
>**Se requieren permisos de administrador**

Elija un CNAME para las páginas de aterrizaje. Algunos ejemplos:

    * **go**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>Procure que sean cortas. Las direcciones URL más cortas son más fáciles de recordar. Sugerimos “go” como dominio.

La primera parte (en negrita) es `[LandingPageCNAME]`. Lo necesitará en el Paso 5.

Para recuperar el Munchkin ID que va a reemplazar con el CNAME de su página de aterrizaje, vaya al área de Administración.

![](assets/setup-steps-9.png)

Haga clic en **Mi cuenta**.

![](assets/setup-steps-10.png)

Copie la [!UICONTROL Cadena de cuenta] de la configuración de la página de aterrizaje.

![](assets/setup-steps-11.png)

Esta es el `[Munchkin ID]`. Guárdelo. Tendrá que proporcionárselo a TI en el Paso 5.

Configure la configuración de dominio para que las páginas de destino utilicen el dominio de su compañía en lugar del de Marketo (donde están alojadas).

## Garantizar la entregabilidad del correo electrónico {#ensure-email-deliverability}

>[!NOTE]
>
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada inicial.

Hay varias medidas que puede tomar para garantizar que los correos electrónicos lleguen al mayor número de personas posible.

* **Marcar sus vínculos de seguimiento**. Puede elegir un CNAME para utilizar su propio dominio (en lugar del de Marketo) en los vínculos que incluye en los correos electrónicos de Marketo. Esto refuerza la promoción de la marca de su dominio y aumenta la confianza y la entregabilidad con sus destinatarios.
* **Agregue Marketo a su lista de permitidos de correo electrónico corporativo.** Es una práctica recomendada común enviar correos electrónicos de prueba a sus cuentas de prueba antes de enviar correos electrónicos a personas reales. Al incluir Marketo en la lista de permitidos, puede evitar el bloqueo de esos correos electrónicos de prueba o que se marquen como spam.
* **Configure SPF y DKIM.** Estas tecnologías garantizan a los destinatarios que los correos electrónicos de Marketo no son correo no deseado. Para evitar que los filtros de spam de los destinatarios rechacen sus correos electrónicos de Marketo, siga estos pasos para [Configurar SPF y DKIM para la entregabilidad de correo electrónico](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configurar un registro MX para su dominio.** Un registro MX le permite recibir correo en el dominio desde el que envía los correos electrónicos para procesar los correos de respuesta y de respuestas automáticas. Si realiza el envío desde su dominio corporativo, es probable que ya lo tenga configurado. Si no es así, puede configurarlo para que se asigne al registro MX de su dominio corporativo.
* **Configuración recomendada para la dirección De.** Debe usar un dominio de correo electrónico válido, existente y activo en la dirección De en todas las campañas de correo electrónico. Puede resultar útil configurar un subdominio del dominio corporativo en lugar de realizar los envíos desde el dominio corporativo. Esto garantizará que los posibles problemas del flujo de correo corporativo no afecten al flujo de correo de Marketo, ni viceversa. Además, el envío de correos desde `something@nonexistentdomain.com` hará que el correo electrónico se filtre o bloquee. Cualquier dominio utilizado en la dirección De del remitente debe tener una cuenta postmaster@ y abuse@ válida y activa.

Si usa aplicaciones de Google para alojar su correo electrónico corporativo, no podrá crear correos electrónicos de abuse@ o postmaster@ en su dominio. Para evitar esto, cree grupos con los nombres “abuse” y “postmaster”. Los usuarios que sean miembros de estos grupos recibirán los correos electrónicos enviados a esas direcciones (por ejemplo, <postmaster@domain.com>). Puede encontrar instrucciones detalladas para crear grupos [aquí](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Elija un CNAME para los vínculos de seguimiento de correo electrónico (elija uno que sea _diferente_ del CNAME de la página de aterrizaje que eligió en el Paso 3). Algunos ejemplos:

* go2.[CompanyDomain].com
* em.[CompanyDomain].com
* wow.[CompanyDomain].com

La primera parte es el CNAME de seguimiento del correo electrónico, `[EmailTrackingCNAME]`. Deberá proporcionárselo a TI en el paso 5.

>[!CAUTION]
>
>Los CNAME de los correos electrónicos y las páginas de destino deben ser diferentes. Además, evite CNAME como “seguimiento” o “vínculo”. Se suele marcar como spam

Para encontrar el vínculo de seguimiento de Marketo, vaya al área de **[!UICONTROL Administración]**.

![](assets/setup-steps-12.png)

Haga clic en **[!UICONTROL Correo electrónico]**.

![](assets/setup-steps-13.png)

Copie el [!UICONTROL Vínculo de seguimiento] de su configuración de correo electrónico.

El [!UICONTROL vínculo de seguimiento] tiene el siguiente formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Este es su `[MktoTrackingLink]`. Guárdelo. Tendrá que proporcionárselo a TI en el Paso 5.

Recopilar dominios “De”. Haga una lista de todos los dominios “De” (como en `[Sender]@[FromDomain].com`) que planea usar para enviar correos electrónicos desde Marketo. En la mayoría de los casos solo hay uno.

Por ejemplo, “marketo.com” o “info.marketo.com”. Son `[FromDomain1]`, `[FromDomain2]`, etc. Guárdelos. Tendrá que proporcionárselos a TI en el Paso 5.

Ahora dispone de toda la información necesaria para enviar su solicitud a TI.

## Pedir a TI que configure protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada inicial.

Una vez que haya recopilado toda la información necesaria, estará listo para enviar una solicitud a TI. Puede utilizar el texto siguiente como plantilla y sustituir en ella el texto en negrita por su información específica.

[Incluir un vínculo en este artículo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Pegue este texto en el correo electrónico y sustituya los marcadores de posición en negrita:

>[!NOTE]
>
>Consulte los pasos 3 y 4 anteriores para determinar el texto que sustituirá los marcadores de posición. Recuerde que `[LandingPageCNAME]` y `[EmailTrackingCNAME]` deben ser diferentes.

`----------------------------------------------`

Estimado administrador de TI increíble,

Nuestro equipo de marketing ha empezado a utilizar la plataforma de Marketo para comunicarse con nuestros empleados. Para garantizar una buena entregabilidad de los correos electrónicos, debemos realizar los siguientes cambios:

`1)` Para nuestras páginas de aterrizaje, añadir una entrada de DNS (CNAME) para **[LandingPageCNAME]**.**[CompanyDomain]**.com, que señale a **[ID de Munchkin]**.mktoweb.com.

`2)` Para nuestros vínculos de seguimiento en el correo electrónico, añadir una entrada de DNS (CNAME) para **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, que señale a **[MktoTrackingLink]**.

`3)` Incluir Marketo en la lista de permitidos.

    *Si usa las direcciones IP en nuestra Lista de permitidos de correo electrónico, añada las direcciones IP que se indican a continuación:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    94.236.119.0/26

>[!NOTE]
>
>Póngase en contacto con el Soporte técnico de Marketo si desea una lista abreviada de direcciones IP para la lista de permitidos específica de su entorno.

    *Si nuestro sistema antispam utiliza dominios de origen, añada lo siguiente:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Necesitamos configurar SPF y DKIM para que Marketo esté autorizado para enviar correos electrónicos firmados en nuestro nombre.

`a.` Para configurar SPF, añada la línea siguiente a nuestras entradas de DNS:

En TXT **[Dominio de origen]**: v=spf1 mx ip4:**[IP corporativas]**
<br/>include: mktomail.com ~all

Si ya tiene un registro SPF existente en la entrada de DNS, simplemente añada lo siguiente:

include:mktomail.com

`[`Sustituir el **Dominio de origen** con el dominio de origen de su correo electrónico (por ejemplo: company.com) y **CorpIP** con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo: 255.255.255.255).  Si va a enviar correo electrónico desde varios dominios a través de Marketo, pídale al personal de TI que añada esta línea para cada dominio (en una línea).`]`

`b.` Para DKIM, cree registros de recursos DNS para cada dominio que se desee configurar. A continuación se muestran los registros de host y los valores TXT de cada dominio que firmaremos:

**`[DKIMDomain1]`**: el registro de host es **`[HostRecord1]`** y el valor TXT es **[TXTValue1]**.

**`[DKIMDomain2]`**: El registro de host es **`[HostRecord2]`** y el valor TXT es **`[TXTValue2]`**.

`[`Copie el **HostRecord** y el **TXTValue** para cada **DKIMDomain** que haya configurado después de seguir las [instrucciones indicadas aquí](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). No olvide comprobar cada dominio en **Administración > Correo electrónico > DKIM** después de que el personal de TI haya completado este paso.`]`

`5)` Necesitamos asegurarnos de que haya un registro MX válido para nuestros dominios FROM **[FromDomain1]**, **[FromDomain2]**, etc. ¿Puede confirmarlo? Si no es así, es necesario configurarlo para que se asigne a nuestro registro MX de dominio corporativo. Esto garantizará que podamos procesar las respuestas/respuestas automáticas a nuestros correos de Marketo.

Deseo que me avisen cuando se hayan completado estos pasos para que pueda completar el proceso de configuración con Marketo.

¡Gracias! Son extraordinarios.

Amor,

**`[Your Name]`**

`----------------------------------------------`

Envíe el correo electrónico a TI. Entendemos que el departamento de TI puede tardar algún tiempo en completar estas tareas. Puede continuar con el paso 7, pero recuerde que debe devolver el paso 6 para completar la configuración de Marketo.

## Complete la configuración de Marketo cuando TI termine {#complete-your-marketo-setup-after-it-finishes}

Una vez que el departamento de TI haya completado sus tareas, siga estos pasos para añadir los CNAME de la página de destino y del correo electrónico, y para activar la firma DKIM.

Vaya al área de **[!UICONTROL Administración]** para añadir el CNAME de su página de aterrizaje

![](assets/setup-steps-15.png)

Seleccione Páginas de aterrizaje y haga clic en **[!UICONTROL Editar]** en el área de [!UICONTROL Configuración].

![](assets/setup-steps-16.png)

Escriba el nombre del dominio nuevo en el campo **[!UICONTROL Nombre de dominio para páginas de aterrizaje]**. Debe tener el siguiente formato:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

En el campo de página **[!UICONTROL Reserva]**, escriba la dirección URL a la que desea redirigir a los usuarios si no hay una página de aterrizaje disponible. Puede utilizar la página principal de la compañía si no dispone de una página de reserva. En el campo **[!UICONTROL Página principal]**, introduzca el sitio web de la compañía.

![](assets/setup-steps-18.png)

En el área de [!UICONTROL Administración], seleccione **[!UICONTROL Correo electrónico]** para añadir su CNAME de correo electrónico

![](assets/setup-steps-19.png)

Desplácese hacia abajo hasta [!UICONTROL Dominios de marca]. Seleccione su dominio y haga clic en **[!UICONTROL Editar]**.

![](assets/setup-steps-20.png)

En el campo Dominio, introduzca el dominio de seguimiento de correo electrónico. Debe tener el siguiente formato:

`[EmailTrackingCNAME].[CompanyDomain].com`. Haga clic en **[!UICONTROL Guardar]**.

![](assets/setup-steps-21.png)

## Integración de su CRM {#integrate-your-crm}

Este es probablemente el paso más emocionante de su configuración: es hora de rellenar Marketo con todos esos posibles clientes y contactos que ha almacenado en su CRM.

Elija entre las siguientes opciones, según el CRM que utilice su compañía.

    * [Integrar Marketo con [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrar Marketo con [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Necesita la asistencia del administrador de CRM de su compañía para completar estos pasos.

## Añadir el código de seguimiento a su sitio web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>¿Es cliente de [!DNL Launch Pack]? Puede omitir este paso. Su asesor le proporcionará las instrucciones de código de [!DNL Munchkin] en el documento de instrucciones de configuración de TI.

Marketo tiene un JavaScript de seguimiento personalizado (denominado [!DNL Munchkin]) que puede usar para rastrear las actividades de las personas en cualquier página web. [!DNL Munchkin] es necesario para integrar su sitio web en Marketo. Siga estos pasos para [Añadir código de seguimiento de [!DNL Munchkin]  al sitio web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Experiencia con HTML necesaria para añadir el código de seguimiento.

## Expectativas de rendimiento {#performance-expectations}

¿Qué puede esperar en cuando a rendimiento de Marketo? El rendimiento puede variar según el tamaño y la complejidad de las campañas de marketing. Pero puede esperar unos niveles de rendimiento similares a los descritos en la columna “Estándar” en varias de las tablas que se encuentran en la [descripción del producto Marketo Engage](https://helpx.adobe.com/es/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. Las columnas “Rendimiento” y “Rendimiento avanzado” hacen referencia a paquetes de niveles de rendimiento que proporcionan [niveles de rendimiento más altos](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Todos los pasos de configuración han finalizado. ¡Lo único que queda es sumergirse y usar Marketo!
