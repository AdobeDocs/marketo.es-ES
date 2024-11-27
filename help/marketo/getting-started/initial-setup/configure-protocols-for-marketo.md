---
unique-page-id: 4720433
description: 'Configuración de protocolos para Marketo Engage: documentos de Marketo Engage: documentación del producto'
title: Configuración de protocolos para el Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ed42e3662dc1f9c3b3b27d86d1df816ce26e1076
workflow-type: tm+mt
source-wordcount: '2148'
ht-degree: 0%

---

# Configuración de protocolos para el Marketo Engage{#configure-protocols-for-marketo-engage}

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

Para obtener ayuda en la implementación de los protocolos siguientes, comparta este artículo con su departamento de TI. Si restringen el acceso a la web mediante una lista de permitidos, asegúrese de que agregan los siguientes dominios (incluido el asterisco) para permitir todos los recursos de Marketo Engage y los sockets web:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Paso 1: Crear registros DNS para páginas de aterrizaje y correo electrónico {#step-create-dns-records-for-landing-pages-and-email}

**CNAME de vínculo de seguimiento**

Su equipo de marketing debería haberle enviado dos solicitudes de nuevos registros CNAME. El primero es para las direcciones URL de la página de aterrizaje, de modo que las páginas de aterrizaje aparezcan en direcciones URL que reflejen el dominio y no el Marketo Engage (el host real). El segundo es para los vínculos de seguimiento incluidos en los correos electrónicos que envían del Marketo Engage.

`1` **Agregar CNAME para páginas de aterrizaje**

Agregue el CNAME de la página de aterrizaje que le enviaron a su registro DNS para que `[YourLandingPageCNAME]` apunte a la cadena de cuenta única asignada a sus páginas de aterrizaje de Marketo Engage. Inicie sesión en el sitio del registrador de dominios e introduzca el CNAME de la página de aterrizaje y la cadena de cuenta. Normalmente, esto implica tres campos:

* Alias: escriba `[YourLandingPageCNAME]` (proporcionado por marketing)
* Tipo: CNAME
* Apuntar a: Escriba `[MunchkinID].mktoweb.com` (proporcionado por marketing)

`2` **Agregar CNAME para los vínculos de seguimiento de correo electrónico**

Agregue el correo electrónico que le envió el equipo de marketing CNAME, de modo que `[YourEmailCNAME]` apunte a [MktoTrackingLink], el vínculo de seguimiento predeterminado que el Marketo Engage asignó, con el formato:\
`[YourEmailCNAME].[YourDomain].com` EN CNAME `[MktoTrackingLink]`

Por ejemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` debe ser el dominio de marca predeterminado.

`3` **Notificar al equipo de marketing**

Notifique a su equipo de marketing cuando haya completado este proceso.

`4` **Póngase en contacto con el [Soporte técnico del Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para iniciar el proceso de aprovisionamiento de un certificado SSL.**

Este proceso puede tardar hasta tres días hábiles en completarse.

## Paso 2: Lista de permitidos de direcciones IP de Marketo Engage {#step-allowlist-marketo-ips}

Cuando el grupo de marketing utiliza Marketo Engage para enviar correos electrónicos de prueba (una práctica recomendada antes de enviar correos electrónicos explosivos), los correos electrónicos de prueba a veces se bloquean mediante sistemas antispam que dependen de las direcciones IP del remitente para comprobar que el correo electrónico es válido. Para asegurarse de que estos correos electrónicos de prueba llegan, agregue Marketo Engage a la lista de permitidos.

Añada estas direcciones IP a la lista de permitidos corporativa:

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Algunos sistemas antispam utilizan el campo Return-Path de correo electrónico en lugar de la dirección IP para permitir el envío. En esos casos, el mejor enfoque es la lista de permitidos &#39;&#42;.mktomail.com&#39;, ya que el Marketo Engage utiliza varios subdominios de buzón. Lista de permitidos de otros sistemas de correo no deseado basada en la dirección De. En estas situaciones, asegúrese de incluir todos los dominios de envío (&quot;De&quot;) que utiliza su grupo de marketing para comunicarse con las personas o los posibles clientes.

>[!NOTE]
>
>Postini emplea una tecnología única y requiere rangos de IP de inclusión en la lista de permitidos. Ver [Inclusión en la lista de permitidos con Postini](https://nation.marketo.com/docs/DOC-1066).

## Paso 3: Configuración de SPF y DKIM {#step-set-up-spf-and-dkim}

Su equipo de marketing también debería haberle enviado información de DKIM (Domain Keys Identified Mail) para que se añada a su registro de recursos DNS (también mostrado a continuación). Siga los pasos para configurar correctamente DKIM y SPF (Entorno de políticas de remitentes) y, a continuación, notifique a su equipo de marketing que se ha actualizado.

1. Para configurar SPF, agregue la línea siguiente a las entradas DNS:

   `[CompanyDomain]` EN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Si ya tenemos un registro SPF en nuestra entrada DNS, simplemente agréguele lo siguiente:\
   incluir: mktomail.com

   Reemplace CompanyDomain por el dominio principal de su sitio web (por ejemplo: &quot;`(company.com/)`&quot;) y CorpIP por la dirección IP de su servidor de correo electrónico corporativo (por ejemplo: &quot;255.255.255.255&quot;). Si va a enviar correos electrónicos desde varios dominios a través de Marketo Engage, debe pedir al personal informático que añada esta línea a cada dominio (en una línea).

1. Para DKIM, cree Registros de recursos DNS para cada dominio que desee configurar. A continuación se muestran los registros de host y los valores TXT de cada dominio que firmaremos:

   `[DKIMDomain1]`: el registro de host es `[HostRecord1]` y el valor TXT es `[TXTValue1]`.

   `[DKIMDomain2]`: el registro de host es `[HostRecord2]` y el valor TXT es `[TXTValue2]`.

   Copie HostRecord y TXTValue para cada DKIMDomain configurado después de seguir las [instrucciones aquí](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. No olvide comprobar cada dominio en Administración > Correo electrónico > DKIM después de que el personal de TI haya completado este paso.

## Paso 4: Configuración de DMARC {#set-up-dmarc}

DMARC (Autenticación de mensajes, creación de informes y conformidad basados en dominio) es un protocolo de autenticación que se utiliza para ayudar a las organizaciones a proteger su dominio contra el uso no autorizado. DMARC amplía los protocolos de autenticación existentes, como SPF y DKIM, para informar a los servidores de destinatarios de qué acciones deben realizar si se produce un error de autenticación en su dominio. Aunque DMARC es opcional en la actualidad, se recomienda encarecidamente, ya que protegerá mejor la marca y la reputación de su organización. Los principales proveedores, como Google y Yahoo, exigirán el uso de DMARC para remitentes masivos a partir de febrero de 2024.

Para que DMARC funcione, debe tener al menos uno de los siguientes registros TXT DNS:

* Un SPF válido
* Un registro de DKIM válido para su FROM: Domain (recomendado para Marketo Engage)

Además, debe tener un registro TXT DNS específico de DMARC para su FROM: Domain. De forma opcional, se puede definir una dirección de correo electrónico de su elección para indicar a dónde deben ir los informes de DMARC dentro de su organización, de modo que pueda monitorizar los informes.

Como práctica recomendada, se recomienda implementar lentamente la implementación de DMARC escalando la directiva de DMARC de p=none, a p=quarantine, a p=reject para comprender el impacto potencial de DMARC y establecer la directiva de DMARC en una alineación relajada en SPF y DKIM.

### Flujo de trabajo de ejemplo de DMARC {#dmarc-example-workflow}

1. Si está configurado para recibir informes de DMARC, debe hacer lo siguiente...

   I. Analice los comentarios y los informes que recibe y utiliza (p=ninguno), lo que indica al destinatario que no realice ninguna acción contra los mensajes que no se autentican correctamente, pero que envíe informes por correo electrónico al remitente.

   II. Revise y corrija los problemas con SPF/DKIM si los mensajes legítimos fallan en la autenticación.

   III. Determine si SPF o DKIM están alineados y pasa la autenticación para todos los correos electrónicos legítimos.

   IV. Revise los informes para asegurarse de que los resultados son los esperados en función de las políticas de SPF/DKIM.

1. Ajuste la directiva a (p=quarantine), que indica al servidor de correo electrónico receptor que ponga en cuarentena el correo electrónico que falla en la autenticación (esto generalmente significa colocar esos mensajes en la carpeta de correo no deseado).

   I. Revise los informes para asegurarse de que los resultados son los esperados.

1. Si está satisfecho con el comportamiento de los mensajes en el nivel p=quarantine, puede ajustar la directiva a (p=reject). La directiva p=reject indica al destinatario que deniegue (devuelva) completamente cualquier correo electrónico del dominio que falle en la autenticación. Con esta directiva habilitada, solo los correos electrónicos verificados como 100 % autenticados por el dominio tendrán la oportunidad de colocarse en la bandeja de entrada.

>[!CAUTION]
>
>Utilice esta directiva con precaución y determine si es apropiada para su organización.

### Informes de DMARC {#dmarc-reporting}

DMARC ofrece la capacidad de recibir informes sobre los correos electrónicos que fallan en SPF/DKIM. Los proveedores de servicios de Internet generan dos informes diferentes como parte del proceso de autenticación que los remitentes pueden recibir a través de las etiquetas RUA/RUF en su directiva de DMARC.

* Informes agregados (RUA): no contiene ninguna PII (información de identificación personal) que sea sensible al RGPD (Reglamento general de protección de datos).

* Informes forenses (RUF): contiene direcciones de correo electrónico que son sensibles al RGPD. Antes de utilizar, es mejor comprobar internamente cómo tratar la información que necesita cumplir con el RGPD.

El uso principal de estos informes es recibir una descripción general de los correos electrónicos que se intentan suplantar. Se trata de informes muy técnicos que se digieren mejor con una herramienta de terceros.

### Ejemplo de registros de DMARC {#example-dmarc-records}

* Registro mínimo vacío: `v=DMARC1; p=none`

* Registro que dirige a una dirección de correo electrónico para recibir informes: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Etiquetas de DMARC y lo que hacen {#dmarc-tags-and-what-they-do}

Los registros de DMARC tienen varios componentes denominados etiquetas de DMARC. Cada etiqueta tiene un valor que especifica un aspecto determinado de DMARC.

<table>
<thead>
  <tr>
    <th>Nombre de etiqueta </th>
    <th>Obligatorio/Opcional </th>
    <th>Función </th>
    <th>Ejemplo </th>
    <th>Valor predeterminado </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Requerido</td>
    <td>Esta etiqueta de DMARC especifica la versión. De momento solo hay una versión, por lo que tendrá un valor fijo de v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Requerido</td>
    <td>Muestra la directiva de DMARC seleccionada y dirige al receptor a informar, poner en cuarentena o rechazar el correo que no supera las comprobaciones de autenticación.</td>
    <td>p=ninguno, cuarentena o rechazo</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Opcional</td>
    <td>Permite al propietario del dominio especificar las opciones de creación de informes.</td>
    <td>0: Generar informe si falla todo 
    <br>1: Generar informe si algo falla 
    <br>d: generar informe si falla DKIM 
    <br>s: generar informe si falla el SPF</td>
    <td>1 (recomendado para informes de DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Opcional</td>
    <td>Indica el porcentaje de mensajes sujetos al filtrado.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Opcional (recomendado)</td>
    <td>Identifica dónde se enviarán los informes agregados.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>tugurio</td>
    <td>Opcional (recomendado)</td>
    <td>Identifica dónde se enviarán los informes forenses.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Opcional</td>
    <td>Especifica la directiva de DMARC para los subdominios del dominio principal.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Opcional</td>
    <td>Puede ser Estricto (s) o ® relajado. La alineación relajada significa que el dominio utilizado en la firma de DKIM puede ser un subdominio de la dirección "De". Alineación estricta significa que el dominio utilizado en la firma de DKIM debe coincidir exactamente con el dominio utilizado en la dirección De.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Opcional</td>
    <td>Puede ser Estricto (s) o ® relajado. La alineación relajada significa que el dominio ReturnPath puede ser un subdominio de la dirección remitente. La alineación estricta significa que el dominio Return-Path debe coincidir exactamente con la dirección From.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Para obtener información detallada acerca de DMARC y todas sus opciones, visite [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC y MARKETO ENGAGE {#dmarc-and-marketo-engage}

Existen dos tipos de alineación para DMARC: alineación DKIM y alineación SPF.

>[!NOTE]
>
>Se recomienda realizar la alineación de DMARC en DKIM frente a SPF para Marketo Engage.

* DMARC alineado con DKIM: para configurar DMARC alineado con DKIM, debe:

   * Configure DKIM para el dominio FROM: del mensaje. Use las instrucciones [de este artículo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configure DMARC para el dominio FROM:/DKIM configurado anteriormente

* SPF alineado con DMARC: para configurar el SPF alineado con DMARC a través de una ruta de retorno de marca, debe:

   * Configuración del dominio de rutas de retorno de marca
      * Configurar el registro SPF adecuado
      * Cambie el registro MX para que vuelva al MX predeterminado del centro de datos desde el que se enviará el correo

   * Configuración de DMARC para el dominio de rutas de retorno de marca

* Si estás enviando correo desde Marketo Engage a través de una IP específica y aún no has implementado una ruta de retorno de marca, o no estás seguro si lo has hecho, abre un ticket con [Soporte de Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Si estás enviando correo de un Marketo Engage a través de un grupo compartido de IP, puedes ver si calificas para IP de confianza al [aplicar aquí](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. La ruta de retorno de marca se ofrece de forma gratuita a los que envían desde IP de confianza de Marketo Engage. Si se aprueba para este programa, póngase en contacto con Soporte técnico de Adobe para configurar una ruta de retorno de marca.

   * IP de confianza: grupo compartido de IP reservado para usuarios de menor volumen que envían &lt;75 000/mes y que no cumplen los requisitos para una IP dedicada. Estos usuarios también deben cumplir con los requisitos de las prácticas recomendadas.

* Si envía correo de un Marketo Engage a través de direcciones IP compartidas y no cumple los requisitos para obtener direcciones IP fiables y envía más de 100 000 mensajes al mes, deberá ponerse en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para adquirir una dirección IP dedicada.

* No se admite ni se recomienda una alineación SPF estricta dentro del Marketo Engage.

## Paso 5: Configurar registros MX para su dominio {#step-set-up-mx-records-for-your-domain}

Un registro MX le permite recibir correo electrónico en el dominio desde el que envía el correo electrónico para procesar las respuestas y los respondedores automáticos. Si envía desde su dominio corporativo, es probable que ya lo tenga configurado. Si no es así, normalmente puede configurarlo para que se asigne al registro MX de su dominio corporativo.

## Direcciones IP de salida {#outbound-ip-addresses}

Una conexión saliente es la que realiza el Marketo Engage a un servidor en Internet en su nombre. Algunos socios o proveedores con los que trabaja, o su propia organización de TI, pueden utilizar listas de permitidos para restringir el acceso a los servidores. Si es así, debe proporcionarles bloques de direcciones IP salientes de Marketo Engage para añadirlos a sus listas de permitidos.

**Webhooks**

El Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} es un mecanismo de integración saliente. Cuando se ejecuta una acción de flujo [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} como parte de una campaña inteligente, se realiza una solicitud HTTP a un servicio web externo. Si el editor del servicio web utiliza una lista de permitidos en el cortafuegos de la red en la que se encuentra el servicio web externo, el editor debe añadir a su lista de permitidos los bloques de direcciones IP que se indican a continuación.

**Sincronización CRM**

El Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} y [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} son mecanismos de integración que realizan solicitudes HTTP salientes a las API publicadas por el proveedor de CRM. Debe asegurarse de que su organización de TI no bloquee ninguno de los bloques de direcciones IP siguientes para acceder a las API de proveedor de CRM.

**Bloques de direcciones IP salientes de Marketo Engage**

Las siguientes tablas abarcan todos los servidores de Marketo Engage que realizan llamadas salientes. Utilice las siguientes listas si va a configurar una lista de permitidos IP, un servidor de, un cortafuegos, una lista de control de acceso, un grupo de seguridad o un servicio de terceros para recibir conexiones salientes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloque IP (Notación CIDR)</th>
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
   <td>13 237 155 207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34 247 24 245</td>
  </tr>
  <tr>
   <td>35 165 244 220</td>
  </tr>
  <tr>
   <td>44 235 171 179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54 160 246 246</td>
  </tr>
  <tr>
   <td>54 212 167 17</td>
  </tr>
  <tr>
   <td>54 220 138 65</td>
  </tr>
   <tr>
   <td>54 237 141 197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
