---
unique-page-id: 4720433
description: Configurar protocolos para el marketing - Documentos de marketing - Documentación del producto
title: Configuración de protocolos para el marketing
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 1%

---


# Configuración de protocolos para el marketing {#configure-protocols-for-marketo}

Su grupo de marketing está usando Marketing para crear páginas de aterrizaje de campaña de marca y correos electrónicos. Para garantizar que esas páginas de aterrizaje y correos electrónicos funcionen, necesitan un poco de ayuda de TI. Configure los siguientes protocolos con la información que su grupo de mercadotecnia debería haberle enviado por correo electrónico.

>[!NOTE]
>
>Este artículo específico debe ser consultado por el departamento de TI de la compañía que desee implementar estos protocolos.

## Paso 1: Crear registros DNS para Páginas de aterrizaje y correo electrónico {#step-create-dns-records-for-landing-pages-and-email}

**CNAME de vínculo de seguimiento**

Su equipo de mercadotecnia debería haberle enviado dos solicitudes de nuevos registros CNAME. El primero es para las direcciones URL de página de aterrizaje, de modo que las páginas de aterrizaje aparezcan en direcciones URL que reflejen su dominio y no en Marketing (el host real). El segundo es para los vínculos de seguimiento que se incluyen en los correos electrónicos que envían desde Marketing.

1 - **Añadir CNAME para Páginas de aterrizaje**

Añada el CNAME de página de aterrizaje que le han enviado al registro DNS, de modo que `[YourLandingPageCNAME]` apunte a la cadena de cuenta única asignada a sus páginas de aterrizaje de marketing. Inicie sesión en el sitio del registrador de dominios e introduzca el CNAME de página de aterrizaje y la cadena de cuenta. Generalmente, esto incluye tres campos:

・ Alias: Escriba `[YourLandingPageCNAME]` (proporcionado por la mercadotecnia) ・ Tipo: CNAME\
・ Apunte a: Intro `[MarketoAccountString].mktoweb.com` (proporcionado por marketing)

2 - **Añadir CNAME para vínculos de Seguimiento del correo electrónico**

Añada el correo electrónico que le envió la mercadotecnia CNAME, de modo que `[YourEmailCNAME]` apunte a [MktoTrackingLink], el vínculo de seguimiento predeterminado asignado por Marketing, en el formato:\
`[YourEmailCNAME].[YourDomain].com` EN CNAME `[MktoTrackingLink]`

Por ejemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

3 - **Notificar a su equipo de mercadotecnia**

Notifique al equipo de mercadotecnia cuando haya completado este proceso.

## Paso 2: IP de mercadotecnia de lista de permitidos {#step-allowlist-marketo-ips}

Cuando su grupo de marketing utiliza Marketing para enviar correos electrónicos de prueba (una práctica recomendada antes de enviar mensajes de correo electrónico), los mensajes de correo electrónico de prueba a veces son bloqueados por sistemas antispam que dependen de las direcciones IP del remitente para verificar que el correo electrónico es válido. Para asegurarse de que esos mensajes de correo electrónico de prueba llegan, agregue Marketo a la lista de permitidos.

Añada estas direcciones IP a su lista de permitidos corporativa:

199.15.212.0/22\
192.28.144.0/20\
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Algunos sistemas antispam utilizan el campo de ruta de retorno de correo electrónico en lugar de la dirección IP para permitir el envío. En estos casos, el mejor enfoque es la lista de permitidos ‘*.mktomail.com’, ya que Marketing utiliza varios subdominios de buzón. Otra lista de permitidos de sistemas antispam basada en la dirección De. En estas situaciones, asegúrese de incluir todos los dominios de envío (&quot;Desde&quot;) que su grupo de marketing utiliza para comunicarse con personas o leads.

>[!NOTE]
>
>Postini emplea una tecnología única y requiere intervalos de IP de inclusión en la lista de permitidos. Consulte [Inclusión en la lista de permitidos con Postini](http://nation.marketo.com/docs/DOC-1066).

## Paso 3: Configuración de SPF y DKIM {#step-set-up-spf-and-dkim}

Su equipo de mercadotecnia también debería haberle enviado información de DKIM para agregarla al registro de recursos DNS (también se enumera a continuación). Siga los pasos para configurar correctamente DKIM y SPF, luego notifique a su equipo de mercadotecnia que se ha actualizado.

1. Para configurar SPF, agregue la línea siguiente a nuestras entradas DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   incluir: [mktomail.com](http://mktomail.com/) ~all

   Si ya tenemos un registro SPF existente en nuestra entrada DNS, simplemente agregue lo siguiente:\
   incluir: [mktomail.com](http://mktomail.com)

   Reemplazar CompanyDomain por el dominio principal del sitio web (por ejemplo: &quot;`(company.com/)`&quot;) y CorpIP con la dirección IP de su servidor de correo electrónico corporativo (por ejemplo: &quot;255.255.255.255&quot;). Si va a enviar correos electrónicos desde varios dominios a través de Marketing, debe hacer que el personal de TI agregue esta línea para cada dominio (en una línea).

1. Para DKIM, cree registros de recursos DNS para cada dominio que desee configurar. A continuación se muestran los registros de host y los valores TXT de cada dominio para el que firmaremos:

   `[DKIMDomain1]`:: El registro de host es `[HostRecord1]` y el valor de TXT es `[TXTValue1]`.

   `[DKIMDomain2]`:: El registro de host es `[HostRecord2]` y el valor de TXT es `[TXTValue2]`.

   Copie HostRecord y TXTValue para cada DKIMDomain que haya configurado después de seguir las [instrucciones aquí](https://docs.marketo.com/display/public/DOCS/Set+up+a+Custom+DKIM+Signature). No olvide comprobar cada dominio en Administración > Correo electrónico > DKIM después de que su personal de TI haya completado este paso.

## Paso 4: Configurar registros MX para su dominio {#step-set-up-mx-records-for-your-domain}

Un registro MX permite recibir correo al dominio desde el que se envía un correo electrónico para procesar las respuestas y los respondedores automáticos. Si va a enviar desde su dominio corporativo, es probable que ya tenga esto configurado. Si no es así, normalmente puede configurarlo para asignarlo al registro MX del dominio corporativo.
