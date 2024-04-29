---
description: 'Configuración de protocolos para Marketo: documentos de Marketo: documentación del producto'
title: Configuración de protocolos para Marketo
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: f9bf2082968737277b3c976659802992f975ec9a
workflow-type: tm+mt
source-wordcount: '2178'
ht-degree: 0%

---

# Tareas de configuración iniciales para el Marketo Engage{#initial-setup-tasks-for-marketo-engage}

Al configurar por primera vez la nueva instancia de Adobe Marketo Engage, hay que realizar algunas tareas, que recomendamos encarecidamente, para ponerse en marcha.

Cuando haya completado todas las tareas que se indican a continuación, vaya a nuestra [Configuración de usuario](/help/marketo/getting-started-2/initial-setup/user-setup.md) para realizar algunos pasos básicos para el uso continuo de su instancia.

## Tarea 1: Dominios de Lista de permitidos {#allowlist-domains}

Si usted o su organización utilizan una configuración restrictiva del servidor de seguridad o del servidor proxy, es posible que usted o el administrador de la red tengan que realizar una lista de permitidos de ciertos dominios e intervalos de direcciones IP para garantizar que Adobe Marketo Engage funciona según lo esperado.

Para obtener ayuda en la implementación de los protocolos siguientes, comparta este artículo con su departamento de TI. Si restringen el acceso a la web mediante una lista de permitidos, asegúrese de que agregan los siguientes dominios (incluido el asterisco) para permitir todos los recursos y sockets web de Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Tarea 2: Creación de registros DNS para páginas de aterrizaje y correo electrónico {#step-create-dns-records-for-landing-pages-and-email}

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

## Tarea 3: Lista de permitidos de direcciones IP de Marketo {#step-allowlist-marketo-ips}

Cuando su grupo de marketing utiliza Marketo para enviar correos electrónicos de prueba (una práctica recomendada antes de enviar correos electrónicos explosivos), los correos electrónicos de prueba a veces se bloquean mediante sistemas antispam que dependen de las direcciones IP del remitente para comprobar que el correo electrónico es válido. Para asegurarse de que llegan los correos electrónicos de prueba, añada Marketo a la lista de permitidos.

Añada estas direcciones IP a la lista de permitidos corporativa:

94,236.119.0/26

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

## Tarea 4: Configuración de SPF y DKIM {#step-set-up-spf-and-dkim}

Su equipo de marketing también debería haberle enviado información de DKIM (Domain Keys Identified Mail) para que se añada a su registro de recursos DNS (también mostrado a continuación). Siga los pasos para configurar correctamente DKIM y SPF (Marco de políticas del remitente) y, a continuación, notifique a su equipo de marketing que se ha actualizado.

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

## Tarea 5: Configuración de DMARC {#set-up-dmarc}

DMARC (Autenticación de mensajes, creación de informes y conformidad basados en dominio) es un protocolo de autenticación que se utiliza para ayudar a las organizaciones a proteger su dominio contra el uso no autorizado. DMARC amplía los protocolos de autenticación existentes, como SPF y DKIM, para informar a los servidores de destinatarios de qué acciones deben realizar si se produce un error de autenticación en su dominio. Aunque DMARC es actualmente opcional, se recomienda encarecidamente, ya que protegerá mejor la marca y la reputación de su organización. Los principales proveedores, como Google y Yahoo, exigirán el uso de DMARC para remitentes masivos a partir de febrero de 2024.

Para que DMARC funcione, debe tener al menos uno de los siguientes registros TXT DNS:

* Un SPF válido
* Un registro DKIM válido para su dominio FROM: (recomendado para el Marketo Engage)

Además, debe tener un registro TXT DNS específico de DMARC para su FROM: Domain. De forma opcional, se puede definir una dirección de correo electrónico de su elección para indicar adónde deben ir los informes DMARC dentro de su organización, de modo que pueda monitorizar los informes.

Como práctica recomendada, se recomienda implementar lentamente la implementación de DMARC escalando la política de DMARC de p=none, p=quarantine, p=reject a medida que se comprende el impacto potencial de DMARC y establecer la política de DMARC para una alineación relajada en SPF y DKIM.

### Flujo de trabajo de ejemplo DMARC {#dmarc-example-workflow}

1. Si está configurado para recibir informes DMARC, debe hacer lo siguiente...

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

### Informes DMARC {#dmarc-reporting}

DMARC ofrece la capacidad de recibir informes sobre correos electrónicos que fallan en SPF/DKIM. Existen dos informes diferentes generados por los proveedores de servicios de Internet como parte del proceso de autenticación que los remitentes pueden recibir a través de las etiquetas RUA/RUF en su política DMARC.

* Informes agregados (RUA): no contiene ninguna PII (información de identificación personal) que sea sensible al RGPD (Reglamento general de protección de datos).

* Informes forenses (RUF): contiene direcciones de correo electrónico que son sensibles al RGPD. Antes de utilizar, es mejor comprobar internamente cómo tratar la información que necesita cumplir con el RGPD.

El uso principal de estos informes es recibir una descripción general de los correos electrónicos que se intentan suplantar. Se trata de informes muy técnicos que se digieren mejor con una herramienta de terceros.

### Ejemplo de registros DMARC {#example-dmarc-records}

* Registro mínimo vacío: `v=DMARC1; p=none`

* Registre la dirección a una dirección de correo electrónico para recibir informes: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Etiquetas DMARC y lo que hacen {#dmarc-tags-and-what-they-do}

Los registros DMARC tienen varios componentes llamados etiquetas DMARC. Cada etiqueta tiene un valor que especifica un determinado aspecto de DMARC.

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
    <td>Obligatorio</td>
    <td>Esta etiqueta DMARC especifica la versión. De momento, solo hay una versión, por lo que tendrá un valor fijo de v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obligatorio</td>
    <td>Muestra la directiva DMARC seleccionada y dirige al receptor a informar, poner en cuarentena o rechazar correo que no supere las comprobaciones de autenticación.</td>
    <td>p=ninguno, cuarentena o rechazo</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>opcional</td>
    <td>Permite al propietario del dominio especificar las opciones de creación de informes.</td>
    <td>0: Generar informe si falla todo 
    <br>1: Generar un informe si algo falla 
    <br>d: Generar informe si falla DKIM 
    <br>s: Generar informe si falla el SPF</td>
    <td>1 (recomendado para informes DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>opcional</td>
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
    <td>opcional</td>
    <td>Especifica la directiva DMARC para los subdominios del dominio principal.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>opcional</td>
    <td>Puede ser Estricto (s) o ® relajado. La alineación relajada significa que el dominio utilizado en la firma DKIM puede ser un subdominio de la dirección "Desde". Alineación estricta significa que el dominio utilizado en la firma DKIM debe coincidir exactamente con el dominio utilizado en la dirección De.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>opcional</td>
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
>Se recomienda realizar la alineación de DMARC en DKIM frente a SPF para Marketo.

* DMARC alineada con DKIM: para configurar DMARC alineada con DKIM debe:

   * Configure DKIM para el dominio FROM: del mensaje. Siga las instrucciones [en este artículo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configure DMARC para el dominio FROM:/DKIM configurado anteriormente

* SPF alineado con DMARC: para configurar el SPF alineado con DMARC a través de una trayectoria de retorno de marca, debe:

   * Configuración del dominio de rutas de retorno de marca
      * Configurar el registro SPF adecuado
      * Cambie el registro MX para que vuelva al MX predeterminado del centro de datos desde el que se enviará el correo

   * Configuración de DMARC para el dominio de rutas de retorno de marca

* Si envía correo desde Marketo a través de una IP dedicada y aún no ha implementado una ruta de retorno de marca, o no está seguro de haberlo hecho, abra una incidencia con [Asistencia de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Si envía correo electrónico desde Marketo a través de un grupo compartido de direcciones IP, puede comprobar si cumple los requisitos para obtener direcciones IP fiables de [aplicar aquí](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. La ruta de retorno de marca se ofrece de forma gratuita a quienes envíen desde las IP de confianza de Marketo. Si se aprueba para este programa, póngase en contacto con el Soporte técnico de Marketo para configurar una ruta de retorno de marca.

   * IP de confianza: grupo compartido de IP reservado para usuarios de menor volumen que envían &lt;75 000/mes y que no cumplen los requisitos para una IP dedicada. Estos usuarios también deben cumplir con los requisitos de las prácticas recomendadas.

* Si envía correo desde Marketo a través de direcciones IP compartidas y no cumple los requisitos para obtener direcciones IP fiables y envía más de 100 000 mensajes al mes, deberá ponerse en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para adquirir una dirección IP dedicada.

* No se admite ni se recomienda una alineación SPF estricta en Marketo.

## Tarea 6: Configuración de Registros MX para su Dominio {#step-set-up-mx-records-for-your-domain}

Un registro MX le permite recibir correo electrónico en el dominio desde el que envía el correo electrónico para procesar las respuestas y los respondedores automáticos. Si envía desde su dominio corporativo, es probable que ya lo tenga configurado. Si no es así, normalmente puede configurarlo para que se asigne al registro MX de su dominio corporativo.

## Direcciones IP de salida {#outbound-ip-addresses}

Una conexión saliente es la que realiza el Marketo Engage a un servidor en Internet en su nombre. Algunos socios o proveedores con los que trabaja, o su propia organización de TI, pueden utilizar listas de permitidos para restringir el acceso a los servidores. Si es así, debe proporcionarles bloques de direcciones IP salientes de Marketo Engage para añadirlos a sus listas de permitidos.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} La acción de flujo se ejecuta como parte de una campaña inteligente y se realiza una solicitud HTTP a un servicio web externo. Si el editor del servicio web utiliza una lista de permitidos en el cortafuegos de la red en la que se encuentra el servicio web externo, el editor debe añadir a su lista de permitidos los bloques de direcciones IP que se indican a continuación.

**Sincronización CRM**

Marketo Engage [Sincronización de Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} son mecanismos de integración que realizan solicitudes HTTP salientes a las API publicadas por su proveedor de CRM. Debe asegurarse de que su organización de TI no bloquee ninguno de los bloques de direcciones IP siguientes para acceder a las API de proveedor de CRM.

**Bloques de direcciones IP salientes de Marketo Engage**

Las siguientes tablas abarcan todos los servidores de Marketo Engage que realizan llamadas salientes. Utilice las siguientes listas si va a configurar una lista de permitidos IP, un servidor de, un cortafuegos, una lista de control de acceso, un grupo de seguridad o un servicio de terceros para recibir conexiones salientes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloque IP (Notación CIDR)</th>
  </tr>
  <tr>
   <td>94,236.119.0/26</td>
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
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
 </tbody>
</table>
