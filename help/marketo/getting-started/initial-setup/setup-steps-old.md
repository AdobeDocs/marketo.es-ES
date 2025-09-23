---
unique-page-id: 2949469
description: 'Pasos de configuración, documentos de Marketo: documentación del producto'
title: Pasos de configuración
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '2086'
ht-degree: 1%

---

# Pasos de configuración {#setup-steps}

**Bienvenido a Adobe Marketo Engage!**

Antes de profundizar en el uso de Marketo, debe completar algunos pasos.

Estos pasos incluyen:

* Alguna configuración básica de la cuenta
* Personalizar la marca de las direcciones URL de la página de aterrizaje y los vínculos de correo electrónico para mejorar la confianza y la capacidad de envío
* Sincronización de CRM
* Añadir un código de seguimiento al sitio web corporativo

>[!NOTE]
>
>Solo debes seguir estos pasos si tu compañía es **nueva en Marketo**. Si no es así, es posible que ya se haya realizado la configuración.

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
>**Se requieren permisos de administración**

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
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada de inicio.

>[!NOTE]
>
>**Se requieren permisos de administración**

Elija un CNAME para las páginas de aterrizaje. Algunos ejemplos:

    * **listo**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>¡Manténgalo corto! Las direcciones URL más cortas son más fáciles de recordar. Sugerimos &quot;ir&quot; como dominio.

La primera parte (en negrita) es `[LandingPageCNAME]`. Lo necesitará en el paso 5.

Para recuperar el Munchkin ID que va a reemplazar con el CNAME de su página de aterrizaje, vaya al área de Administración.

![](assets/setup-steps-9.png)

Haga clic en **Mi cuenta**.

![](assets/setup-steps-10.png)

Copie la [!UICONTROL cadena de cuenta] de la configuración de la página de aterrizaje.

![](assets/setup-steps-11.png)

Este es el `[Munchkin ID]`. Guárdelo... Tendrá que darlo a TI en el paso 5.

Configure los ajustes de dominio para que las páginas de aterrizaje utilicen el dominio de su empresa en lugar del de Marketo (donde están alojadas).

## Garantizar entrega de correo electrónico {#ensure-email-deliverability}

>[!NOTE]
>
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada de inicio.

Hay varias medidas que puede tomar para garantizar que los correos electrónicos lleguen a la mayor cantidad de personas posible.

* **Marca tus vínculos de seguimiento**. Puede elegir un CNAME para utilizar su propio dominio (en lugar del de Marketo) en los vínculos que incluye en los correos electrónicos de Marketo. Esto refuerza la marca de su dominio y aumenta la confianza y la capacidad de envío con sus destinatarios.
* **Agregue Marketo a su lista de permitidos de correo electrónico corporativo.** Es una práctica recomendada común enviar correos electrónicos de prueba a sus cuentas de prueba antes de enviar correos electrónicos a personas reales. Mediante la inclusión en la lista de permitidos de Marketo, puede evitar que los correos electrónicos de prueba se bloqueen o marquen como correo no deseado.
* **Configure SPF y DKIM.** Estas tecnologías garantizan a los destinatarios que los correos electrónicos de Marketo no son correo no deseado. Para ayudar a evitar que los filtros de correo no deseado de los destinatarios rechacen sus correos electrónicos de Marketo, siga estos pasos para [Configurar un SPF y DKIM para sus envíos de correo electrónico](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configure un registro MX para su dominio.**: un registro MX permite recibir correo en el dominio desde el que envía el correo electrónico para procesar las respuestas y los respondedores automáticos. Si envía desde su dominio corporativo, es probable que ya lo tenga configurado. Si no es así, normalmente puede configurarlo para que se asigne al registro MX de su dominio corporativo.
* **Configuración recomendada para la dirección de origen.** Debe usar un dominio de correo electrónico válido, existente y de trabajo en la dirección De en todas las campañas de correo electrónico. Puede resultar beneficioso configurar un subdominio del dominio corporativo en lugar de enviar desde el dominio corporativo. Esto garantizará que los problemas del flujo de correo corporativo no afecten al flujo de correo de Marketo y viceversa. Además, si se envía correo desde `something@nonexistentdomain.com`, el correo electrónico se filtrará o bloqueará. Cualquier dominio utilizado en la dirección remitente del remitente debe tener una cuenta válida y activa postmaster@ y abuse@.

Si usas aplicaciones de Google para alojar tu correo electrónico corporativo, no podrás crear correos electrónicos de abuse@ o postmaster@ bajo tu dominio. Para evitar esto, debe crear grupos llamados &quot;abuso&quot; y &quot;administrador de correo&quot;. Los usuarios que sean miembros de estos grupos recibirán correos electrónicos enviados a esas direcciones (por ejemplo, <postmaster@domain.com>). Encontrará instrucciones detalladas para crear grupos [aquí](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Elija un CNAME para los vínculos de seguimiento de correo electrónico (elija uno que sea _diferente_ del CNAME de la página de aterrizaje que eligió en el paso 3). Algunos ejemplos:

* go2.[DominioCompañía].com
* em.[DominioCompañía].com
* vaya.[DominioCompañía].com

La primera parte es el CNAME de seguimiento de correo electrónico `[EmailTrackingCNAME]`. Deberá proporcionárselo a TI en el paso 5.

>[!CAUTION]
>
>Los CNAME de los correos electrónicos y las páginas de aterrizaje deben ser diferentes. Además, evite CNAME como &quot;seguimiento&quot; o &quot;vínculo&quot;. A menudo se marca como spam

Para encontrar el vínculo de seguimiento de Marketo, vaya al área de **[!UICONTROL Admin]**.

![](assets/setup-steps-12.png)

Haga clic en **[!UICONTROL Correo electrónico]**.

![](assets/setup-steps-13.png)

Copie el [!UICONTROL vínculo de seguimiento] de su configuración de correo electrónico.

El [!UICONTROL vínculo de seguimiento] tiene el siguiente formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Este es su `[MktoTrackingLink]`. Guárdelo... Tendrá que darlo a TI en el paso 5.

Recopilar dominios &quot;De&quot;. Haga una lista de todos los dominios &quot;De&quot; (como en, `[Sender]@[FromDomain].com`) que planea usar para enviar correos electrónicos desde Marketo. Para la mayoría, solo hay una.

Por ejemplo, &quot;marketo.com&quot;, &quot;info.marketo.com&quot;, &quot;&quot;. Estos son `[FromDomain1]`, `[FromDomain2]`, etc. Sálvalos... Tendrá que entregarlos a TI en el paso 5.

Ahora dispone de toda la información necesaria para enviar su solicitud a TI.

## Pedir a TI que configure protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>¿Es cliente de Launch Pack? Puede omitir este paso. Su asesor le proporcionará un documento de instrucciones de configuración de TI durante la llamada de inicio.

Una vez que haya recopilado toda la información necesaria, estará listo para enviar una solicitud a TI. Puede utilizar el texto siguiente como plantilla y reemplazar el texto en negrita por su propia información.

[Incluir un vínculo a este artículo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Pegue este texto en el correo electrónico y reemplace los marcadores de posición en negrita:

>[!NOTE]
>
>Consulte los pasos 3 y 4 anteriores para determinar el texto que reemplazará los marcadores de posición. Recuerde que `[LandingPageCNAME]` y `[EmailTrackingCNAME]` deben ser diferentes.

`----------------------------------------------`

Estimado administrador de TI increíble,

Nuestro equipo de marketing ahora utiliza la plataforma Marketo para comunicarse con nuestros empleados. Para garantizar una buena entrega de correos electrónicos, debemos realizar los siguientes cambios:

`1)` Para nuestras páginas de aterrizaje, agregue una entrada DNS (CNAME) para **[LandingPageCNAME]**.**[CompanyDomain]**.com, que señala a **[Munchkin ID]**.mktoweb.com.

`2)` Para nuestros vínculos de seguimiento en el correo electrónico, agregue una Entrada DNS (CNAME) para **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, que señala a **[MktoTrackingLink]**.

`3)` Lista de permitidos Marketo.

    * Si usamos direcciones IP en nuestra Lista de permitidos de correo electrónico, agregue las direcciones IP que se indican a continuación:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>Póngase en contacto con el Soporte de Marketo si desea una lista abreviada de direcciones IP para la lista de permitidos específica de su entorno.

    * Si nuestro sistema antispam utiliza los dominios De, agregue estos:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)`: necesitamos configurar el SPF y el DKIM para que Marketo pueda enviar correos electrónicos firmados en nuestro nombre.

`a.` Para configurar SPF, agregue la línea siguiente a nuestras entradas DNS:

EN TXT **[Desde el dominio]**: v=spf1 mx ip4:**[IP corporativas]**
<br/>incluir: mktomail.com ~todos

Si ya tenemos un registro SPF en nuestra entrada DNS, simplemente agréguele lo siguiente:

include:mktomail.com

`[`Reemplace **Del dominio** con su dominio de origen de correo electrónico (por ejemplo: company.com) y **CorpIP** con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo: 255.255.255.255).  Si va a enviar correo electrónico desde varios dominios a través de Marketo, el personal de TI debe agregar esta línea para cada dominio (en una línea).`]`

`b.` Para DKIM, cree Registros de recursos DNS para cada dominio que deseemos configurar. A continuación se muestran los registros de host y los valores TXT de cada dominio que firmaremos:

**`[DKIMDomain1]`**: el registro de host es **`[HostRecord1]`** y el valor TXT es **[TXTValue1]**.

**`[DKIMDomain2]`**: El registro de host es **`[HostRecord2]`** y el valor TXT es **`[TXTValue2]`**.

`[`Copie **HostRecord** y **TXTValue** para cada **DKIMDomain** que haya configurado después de seguir las [instrucciones aquí](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). No olvide comprobar cada dominio en **Administración > Correo electrónico > DKIM** después de que el personal de TI haya completado este paso.`]`

`5)` Necesitamos asegurarnos de que haya un registro MX válido para nuestros dominios FROM **[FromDomain1]**, **[FromDomain2]**, etc. ¿Puede confirmarlo? Si no es así, configúrelo para asignar a nuestro registro MX de dominio corporativo. Esto garantizará que podamos procesar las respuestas/respuestas automáticas a nuestros correos de Marketo.

Avíseme cuando haya completado estos pasos para que pueda completar el proceso de configuración con Marketo.

¡Gracias! ¡Eres el mejor!

Amor,

**`[Your Name]`**

`----------------------------------------------`

Envíe el correo electrónico a TI. Entendemos que el departamento de TI puede tardar algún tiempo en completar estas tareas. Puede continuar con el paso 7, pero recuerde que debe devolver el paso 6 para completar la configuración de Marketo.

## Complete la configuración de Marketo una vez finalizada la tecnología informática {#complete-your-marketo-setup-after-it-finishes}

Una vez que el departamento de TI haya completado sus tareas, siga estos pasos para agregar los CNAME de la página de aterrizaje y del correo electrónico, y para activar la firma de DKIM.

Vaya al área **[!UICONTROL Admin]** para agregar el CNAME de su página de aterrizaje

![](assets/setup-steps-15.png)

Seleccione Páginas de aterrizaje y haga clic en **[!UICONTROL Editar]** en el área de [!UICONTROL Configuración].

![](assets/setup-steps-16.png)

Escriba su nuevo nombre de dominio en el campo **[!UICONTROL Nombre de dominio para páginas de aterrizaje]**. Debe tener el siguiente formato:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

En el campo de página **[!UICONTROL Reserva]**, escribe la dirección URL a la que deseas que vayan los usuarios si una página de aterrizaje no está disponible. Puede utilizar la página principal de la empresa si no dispone de una página de reserva. En el campo **[!UICONTROL Página principal]**, ingrese el sitio web de la compañía.

![](assets/setup-steps-18.png)

En el área [!UICONTROL Administrador], seleccione **[!UICONTROL Correo electrónico]** para agregar su CNAME de correo electrónico

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
>Necesita la asistencia del administrador de CRM de su empresa para completar estos pasos.

## Añadir código de seguimiento a su sitio web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>¿Es cliente de [!DNL Launch Pack]? Puede omitir este paso. Su asesor le proporcionará [!DNL Munchkin] instrucciones de código en su documento de instrucciones de configuración de TI.

Marketo tiene un JavaScript de seguimiento personalizado (denominado [!DNL Munchkin]) que puede usar para rastrear las actividades de las personas en cualquier página web. [!DNL Munchkin] es necesario para integrar su sitio web en Marketo. Siga estos pasos para [agregar [!DNL Munchkin] código de seguimiento al sitio web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Experiencia con HTML necesaria para añadir el código de seguimiento.

## Expectativas de rendimiento {#performance-expectations}

¿Qué puede esperar en términos de rendimiento de Marketo? Puede variar según el tamaño y la complejidad de las campañas de marketing. Pero puede esperar niveles de rendimiento a la par con lo que se describe en la columna &quot;Estándar&quot; en varias de las tablas que se encuentran en la [descripción del producto Marketo Engage](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. Las columnas &quot;Rendimiento&quot; y &quot;Rendimiento avanzado&quot; hacen referencia a paquetes de niveles de rendimiento que proporcionan [niveles de rendimiento más altos](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Todos los pasos de configuración han finalizado. ¡Lo único que queda es sumergirse y usar Marketo!
