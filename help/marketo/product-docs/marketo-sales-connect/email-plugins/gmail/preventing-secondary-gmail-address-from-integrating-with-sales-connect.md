---
unique-page-id: 14352546
description: Impedir que la dirección de Gmail secundaria se integre con Sales Connect - Marketo Docs - Documentación del producto
title: Impedir que la dirección de Gmail secundaria se integre con Sales Connect
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Impedir que la dirección de Gmail secundaria se integre con Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integración Gmail interrumpida (por qué mi Gmail personal envía correos electrónicos) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

El motivo más común de una conexión Gmail interrumpida es una integración accidental con la cuenta personal de un usuario. Esto puede suceder cuando un usuario hace clic en &quot;Conectar&quot; o cuando intenta enviar un correo electrónico desde su cuenta personal. Esto puede resultar muy tentador porque la opción existirá al acceder a su cuenta de Gmail en la misma instancia de Chrome que el correo electrónico de trabajo.

## ¿Por qué Sales Connect intenta integrarse con mi Gmail personal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect se integra con Gmail mediante una extensión instalada en el navegador Chrome. Siempre que la extensión detecta una instancia de Gmail abierta, oferta una opción para integrarla. Para evitar una integración con su cuenta personal de Gmail, le recomendamos una de las tres cosas...

Iniciar sesión como otro usuario de Chrome (recomendado)

Haga clic en [este vínculo](https://support.google.com/chrome/answer/2364824?hl=en) para leer cómo crear otro Perfil de Chrome.

**Ventajas**: Al iniciar sesión como otro usuario, se abrirá una nueva instancia de Chrome. Esta instancia es una ventana completamente nueva de Chrome y ninguna de sus extensiones antiguas existirá en esta. También guarda las cookies para que no tenga que iniciar sesión en Gmail cada vez.

**Contras**: Debe tener dos ventanas de Chrome abiertas.

Usar otro explorador

**Ventajas:** Usar otro navegador de Internet (IE o Firefox) que no tenga la extensión instalada impedirá que esto ocurra.

**Contras**: Usar varios navegadores puede ser molesto.

Utilizar Una Ventana Incognitiva

**Ventanillas:** Una ventana de incógnito es como abrir una versión desnuda de Chrome. Significa que no tendrá ninguna de sus extensiones instaladas y que Sales Connect no estará allí para conectarse.

**Contras**: Tendrás que iniciar sesión en Gmail cada vez que inicios tu día, y de nuevo si accidentalmente cierras la ventana.
