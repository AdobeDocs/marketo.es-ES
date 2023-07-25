---
unique-page-id: 4720433
description: 'Configuración de protocolos para Marketo: documentos de Marketo: documentación del producto'
title: Configuración de protocolos para Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 3%

---

# Configuración de protocolos para Marketo {#configure-protocols-for-marketo}

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

## Páginas de aterrizaje de campañas de marca y correos electrónicos {#branded-campaign-landing-pages-and-emails}

Su grupo de marketing utiliza Marketo para crear páginas de aterrizaje de campañas de marca y correos electrónicos. Para garantizar que esas páginas de aterrizaje y correos electrónicos funcionen, necesitan un poco de ayuda del departamento de TI. Configure los siguientes protocolos, con la información que su grupo de marketing debería haberle enviado por correo electrónico.

Este artículo debe compartirse con el departamento de TI de la empresa que desee implementar estos protocolos.

Si su equipo de TI restringe el acceso a la web mediante una lista de permitidos, pídale que añada los siguientes dominios (incluido el asterisco) para permitir todos los recursos y sockets web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`

## Paso 1: Crear registros DNS para páginas de aterrizaje y correo electrónico {#step-create-dns-records-for-landing-pages-and-email}

**CNAME de vínculo de seguimiento**

Su equipo de marketing debería haberle enviado dos solicitudes de nuevos registros CNAME. El primero es para las direcciones URL de la página de aterrizaje, de modo que las páginas de aterrizaje aparezcan en direcciones URL que reflejen el dominio y no Marketo (el host real). El segundo es para los vínculos de seguimiento incluidos en los correos electrónicos que envían desde Marketo.

`1` **Añadir CNAME para páginas de destino**

Añada el CNAME de la página de aterrizaje que le enviaron a su registro DNS para que `[YourLandingPageCNAME]` apunta a la cadena de cuenta única asignada a las páginas de aterrizaje de Marketo. Inicie sesión en el sitio del registrador de dominios e introduzca el CNAME de la página de aterrizaje y la cadena de cuenta. Normalmente, esto implica tres campos:

* Alias: Entrar `[YourLandingPageCNAME]` (proporcionado por marketing)
* Tipo: CNAME
* Apuntar a: Entrar `[MunchkinID].mktoweb.com` (proporcionado por marketing)

`2` **Añadir CNAME para vínculos de seguimiento de correo electrónico**

Añada el correo electrónico que le ha enviado marketing CNAME para que `[YourEmailCNAME]` apunta a [MktoTrackingLink], el vínculo de seguimiento predeterminado que Marketo asignó, con el formato:\
`[YourEmailCNAME].[YourDomain].com` EN CNAME `[MktoTrackingLink]`

Por ejemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` debe ser el dominio de marca predeterminado.

`3` **Notifique A Su Equipo De Marketing**

Notifique a su equipo de marketing cuando haya completado este proceso.

`4` **Contacto [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para iniciar el proceso de aprovisionamiento de un certificado SSL.**

Este proceso puede tardar hasta tres días hábiles en completarse.

## Paso 2: Lista de permitidos de direcciones IP de Marketo {#step-allowlist-marketo-ips}

Cuando su grupo de marketing utiliza Marketo para enviar correos electrónicos de prueba (una práctica recomendada antes de enviar correos electrónicos explosivos), los correos electrónicos de prueba a veces se bloquean mediante sistemas antispam que dependen de las direcciones IP del remitente para comprobar que el correo electrónico es válido. Para asegurarse de que llegan los correos electrónicos de prueba, añada Marketo a la lista de permitidos.

Añada estas direcciones IP a la lista de permitidos corporativa:

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Algunos sistemas antispam utilizan el campo Return-Path de correo electrónico en lugar de la dirección IP para permitir el envío. En estos casos, el mejor enfoque es la lista de permitidos &#39;&#42;.mktomail.com&#39;, ya que Marketo utiliza varios subdominios de buzón. Lista de permitidos de otros sistemas de correo no deseado basada en la dirección De. En estas situaciones, asegúrese de incluir todos los dominios de envío (&quot;De&quot;) que utiliza su grupo de marketing para comunicarse con las personas o los posibles clientes.

>[!NOTE]
>
>Postini emplea una tecnología única y requiere rangos de IP de inclusión en la lista de permitidos. Consulte [Inclusión en la lista de permitidos con Postini](https://nation.marketo.com/docs/DOC-1066).

## Paso 3: Configuración de SPF y DKIM {#step-set-up-spf-and-dkim}

Su equipo de marketing también debería haberle enviado información DKIM para añadirla a su registro de recursos DNS (también mostrado a continuación). Siga los pasos para configurar correctamente DKIM y SPF y, a continuación, notifique a su equipo de marketing que se ha actualizado.

1. Para configurar SPF, agregue la línea siguiente a las entradas DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Si ya tenemos un registro SPF en nuestra entrada DNS, simplemente agréguele lo siguiente:\
   incluir: mktomail.com

   Sustituya CompanyDomain por el dominio principal de su sitio web (por ejemplo: &quot;`(company.com/)`&quot;) y CorpIP con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo, &quot;255.255.255.255&quot;). Si va a enviar correos electrónicos desde varios dominios a través de Marketo, debe pedir al personal informático que añada esta línea a cada dominio (en una línea).

1. Para DKIM, cree Registros de recursos DNS para cada dominio que desee configurar. A continuación se muestran los registros de host y los valores TXT de cada dominio que firmaremos:

   `[DKIMDomain1]`: el registro de host es `[HostRecord1]` y el valor TXT es `[TXTValue1]`.

   `[DKIMDomain2]`: el registro de host es `[HostRecord2]` y el valor TXT es `[TXTValue2]`.

   Copie HostRecord y TXTValue para cada DKIMDomain configurado después de seguir el [instrucciones aquí](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. No olvide verificar cada dominio en Administración > Correo electrónico > DKIM después de que su personal de TI haya completado este paso.

## Paso 4: Configurar registros MX para su dominio {#step-set-up-mx-records-for-your-domain}

Un registro MX le permite recibir correo electrónico en el dominio desde el que envía el correo electrónico para procesar las respuestas y los respondedores automáticos. Si envía desde su dominio corporativo, es probable que ya lo tenga configurado. Si no es así, normalmente puede configurarlo para que se asigne al registro MX de su dominio corporativo.

## Direcciones IP de salida {#outbound-ip-addresses}

Una conexión saliente es la que realiza el Marketo Engage a un servidor en Internet en su nombre. Algunos socios o proveedores con los que trabaja, o su propia organización de TI, pueden utilizar listas de permitidos para restringir el acceso a los servidores. Si es así, debe proporcionarles bloques de direcciones IP salientes de Marketo Engage para añadirlos a sus listas de permitidos.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} La acción de flujo se ejecuta como parte de una campaña inteligente y se realiza una solicitud HTTP a un servicio web externo. Si el editor del servicio web utiliza una lista de permitidos en el cortafuegos de la red en la que se encuentra el servicio web externo, el editor debe añadir a su lista de permitidos los bloques de direcciones IP que se indican a continuación.

**Sincronización de CRM**

Marketo Engage [Sincronización de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} son mecanismos de integración que realizan solicitudes HTTP salientes a las API publicadas por su proveedor de CRM. Debe asegurarse de que su organización de TI no bloquee ninguno de los bloques de direcciones IP siguientes para acceder a las API de proveedor de CRM.

**Bloques de direcciones IP salientes de Marketo Engage**

Las siguientes tablas abarcan todos los servidores de Marketo Engage que realizan llamadas salientes. Utilice las siguientes listas si va a configurar una lista de permitidos IP, un servidor de, un cortafuegos, una lista de control de acceso, un grupo de seguridad o un servicio de terceros para recibir conexiones salientes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloque IP (Notación CIDR)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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

<table>
 <tbody>
  <tr>
   <th>Dirección IP individual</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>

