---
unique-page-id: 4720433
description: 'Configuración de protocolos para Marketo: Documentos de Marketo: Documentación del producto'
title: Configuración de protocolos para Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# Configuración de protocolos para Marketo {#configure-protocols-for-marketo}

Si usted o su organización utilizan cortafuegos restrictivo o configuración del servidor proxy, es posible que usted o el administrador de la red tengan que realizar la lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funcione correctamente.

## Páginas de aterrizaje y correos electrónicos de campañas con marca {#branded-campaign-landing-pages-and-emails}

El grupo de marketing usa Marketo para crear páginas de aterrizaje y correos electrónicos de campañas con marca. Para garantizar que esas páginas de aterrizaje y correos electrónicos funcionen, necesitan un poco de ayuda de TI. Configure los siguientes protocolos con la información que su grupo de marketing debería haberle enviado por correo electrónico.

Este artículo debe compartirse con el departamento de TI de la empresa que desee implementar estos protocolos.

>[!NOTE]
>
>Si su equipo de TI restringe el acceso web mediante una lista de permitidos, pídale que añada los siguientes dominios (incluido el asterisco) para permitir todos los recursos y portalámparas web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`

## Paso 1: Creación de registros DNS para páginas de aterrizaje y correo electrónico {#step-create-dns-records-for-landing-pages-and-email}

**CNAME de vínculo de seguimiento**

Su equipo de marketing debería haberle enviado dos solicitudes para nuevos registros CNAME. El primero es para las direcciones URL de la página de aterrizaje, de modo que las páginas de aterrizaje aparezcan en direcciones URL que reflejen su dominio y no Marketo (el host real). El segundo es para los vínculos de seguimiento que se incluyen en los correos electrónicos que envían desde Marketo.

`1` **Agregar CNAME para páginas de aterrizaje**

Agregue el CNAME de la página de aterrizaje que le enviaron al registro DNS para que `[YourLandingPageCNAME]` apunta a la cadena de cuenta única asignada a sus páginas de aterrizaje de Marketo. Inicie sesión en el sitio del registrador de dominios e introduzca el CNAME de la página de aterrizaje y la cadena de cuenta. Normalmente, esto implica tres campos:

* Alias: Entrar `[YourLandingPageCNAME]` (proporcionado por marketing)
* Tipo: CNAME
* Apunte a: Entrar `[MarketoAccountString].mktoweb.com` (proporcionado por marketing)

`2` **Añadir CNAME para vínculos de seguimiento de correo electrónico**

Añada el correo electrónico CNAME de marketing que le ha enviado, para que `[YourEmailCNAME]` señala a [MktoTrackingLink], el vínculo de seguimiento predeterminado asignado por Marketo, con el formato :\
`[YourEmailCNAME].[YourDomain].com` EN CNAME `[MktoTrackingLink]`

Por ejemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Notificar a su equipo de marketing**

Informe a su equipo de marketing cuando haya completado este proceso.

`4` **Contacto [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} para iniciar el proceso de aprovisionamiento de un certificado SSL.**

Este proceso puede tardar hasta 3 días hábiles en completarse.

## Paso 2: Lista de permitidos de IP de Marketo {#step-allowlist-marketo-ips}

Cuando su grupo de marketing utiliza Marketo para enviar correos electrónicos de prueba (una práctica recomendada antes de enviar correos electrónicos), los sistemas antispam que dependen de las direcciones IP del remitente bloquean a veces los mensajes de prueba para verificar que el correo electrónico sea válido. Para asegurarse de que llegan esos correos electrónicos de prueba, agregue Marketo a la lista de permitidos .

Añada estas direcciones IP a la lista de permitidos corporativa:

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Algunos sistemas antispam utilizan el campo Return-Path de correo electrónico en lugar de la dirección IP para permitirlo. En estos casos, el mejor enfoque es la lista de permitidos &quot;&#42;.mktomail.com’, ya que Marketo utiliza varios subdominios de buzón. Lista de permitidos de otros sistemas antispam basada en la dirección De . En estas situaciones, asegúrese de incluir todos los dominios de envío (&quot;De&quot;) que su grupo de marketing utilice para comunicarse con personas o posibles clientes.

>[!NOTE]
>
>Postini emplea una tecnología única y requiere rangos de IP de inclusión en la lista de permitidos. Consulte [Inclusión en la lista de permitidos con Postini](https://nation.marketo.com/docs/DOC-1066).

## Paso 3: Configuración de SPF y DKIM {#step-set-up-spf-and-dkim}

El equipo de marketing también debería haberle enviado información de DKIM para que la agregue al registro de recursos DNS (también se enumera a continuación). Siga los pasos para configurar correctamente DKIM y SPF y, a continuación, notifique a su equipo de marketing que se ha actualizado.

1. Para configurar SPF, agregue la línea siguiente a nuestras entradas DNS:

   `[CompanyDomain]` EN TXT v=spf1 mx ip4:`[CorpIP]`\
   incluir: mktomail.com ~all

   Si ya tenemos un registro SPF existente en nuestra entrada DNS, simplemente agregue lo siguiente:\
   incluir: mktomail.com

   Sustituya CompanyDomain por el dominio principal de su sitio web (por ejemplo: &quot;`(company.com/)`&quot;) y CorpIP con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo, &quot;255.255.255.255&quot;). Si va a enviar correos electrónicos de varios dominios a través de Marketo, debe hacer que su personal de TI agregue esta línea para cada dominio (en una línea).

1. Para DKIM, cree Registros de recursos DNS para cada dominio que desee configurar. A continuación, se muestran los registros de host y los valores TXT de cada dominio para el que se firmará:

   `[DKIMDomain1]`: El registro de host es `[HostRecord1]` y el valor TXT es `[TXTValue1]`.

   `[DKIMDomain2]`: El registro de host es `[HostRecord2]` y el valor TXT es `[TXTValue2]`.

   Copie el HostRecord y TXTValue para cada DKIMDomain que haya configurado después de seguir la [instrucciones aquí](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target=&quot;_blank&quot;}. No olvide verificar cada dominio en Administración > Correo electrónico > DKIM después de que su personal de TI haya completado este paso.

## Paso 4: Configuración de registros MX para su dominio {#step-set-up-mx-records-for-your-domain}

Un registro MX le permite recibir correo al dominio desde el que envía el correo electrónico para procesar las respuestas y los respondedores automáticos. Si está enviando desde su dominio corporativo, probablemente ya lo haya configurado. Si no es así, normalmente puede configurarlo para asignarlo al registro MX de su dominio corporativo.

## Direcciones IP salientes {#outbound-ip-addresses}

Una conexión saliente es una que realiza el Marketo Engage a un servidor de Internet en su nombre. Algunos socios o proveedores con los que trabaje, o su propia organización de TI, pueden utilizar listas de permitidos para restringir el acceso a los servidores. Si es así, debe proporcionarles bloques de direcciones IP salientes de Marketo Engage para añadirlos a sus listas de permitidos.

**Enlaces web**

Marketo Engage [Enlaces web](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;} son un mecanismo de integración saliente. Cuando [Llamar a Weblock](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md)La acción de flujo {target=&quot;_blank&quot;} se ejecuta como parte de una campaña inteligente; se realiza una solicitud HTTP a un servicio web externo. Si el editor de servicios web utiliza una lista de permitidos en el cortafuegos de la red en la que se encuentra el servicio web externo, el editor debe añadir los bloques de direcciones IP que se enumeran a continuación a su lista de permitidos.

**Sincronización de CRM**

Marketo Engage [Sincronización de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;} y [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;} son mecanismos de integración que realizan solicitudes HTTP salientes a las API publicadas por su proveedor de CRM. Debe asegurarse de que su organización de TI no bloquee ninguno de los bloques de direcciones IP siguientes para acceder a las API de proveedor de CRM.

**Bloques de direcciones IP salientes del Marketo Engage**

La siguiente tabla abarca todos los servidores de Marketo Engage que realizan llamadas salientes. Utilice esta lista si está configurando cualquier lista de permitidos IP, servidor de seguridad, firewall, lista de control de acceso, grupo de seguridad o servicio de terceros para recibir conexiones salientes del Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloque IP (Notación CIDR)</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>
