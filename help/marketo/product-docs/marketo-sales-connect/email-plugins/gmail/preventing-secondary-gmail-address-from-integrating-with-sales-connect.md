---
unique-page-id: 14352546
description: Impedir que la dirección de Gmail secundaria se integre con Sales Connect - Marketo Docs - Documentación del producto
title: Impedir que la dirección de Gmail secundaria se integre con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Impedir que la dirección de Gmail secundaria se integre con Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integración de Gmail rota (por qué mi Gmail envía correos electrónicos personales) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

El motivo más común de una conexión de Gmail interrumpida es una integración accidental con la cuenta personal de un usuario. Esto puede ocurrir cuando un usuario hace clic en &quot;Conectar&quot; o cuando intenta enviar un correo electrónico desde su cuenta personal. Esto puede ser muy tentador porque la opción existirá al acceder a su cuenta de Gmail en la misma instancia de Chrome que el correo electrónico de trabajo.

## ¿Por qué Sales Connect incluso intenta integrarse con mi Gmail personal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect se integra con Gmail a través de una extensión instalada en el explorador Chrome. Siempre que la extensión detecta una instancia de Gmail abierta, ofrece una opción para integrarla. Para evitar una integración con su cuenta personal de Gmail, le recomendamos una de tres cosas...

Iniciar sesión como otro usuario de Chrome (recomendado)

Haga clic en [este vínculo](https://support.google.com/chrome/answer/2364824?hl=en) para leer cómo crear otro perfil de Chrome.

**Pros**: Iniciar sesión como otro usuario abrirá una nueva instancia de Chrome. Esta instancia es una ventana completamente nueva de Chrome y ninguna de sus extensiones antiguas existirá en esta. También conserva las cookies para que no tenga que iniciar sesión en su Gmail cada vez.

**Contras**: Debe tener dos ventanas de Chrome abiertas.

Usar otro navegador

**Ventajas:** Usar otro navegador de Internet (IE o Firefox) que no tenga la extensión instalada evitará que esto ocurra.

**Contras**: Usar varios navegadores puede ser molesto.

Utilizar Una Ventana Incognitiva

**Ventajas:** Una ventana de incógnito es como abrir una versión desnuda de Chrome. Esto significa que no tendrá ninguna de sus extensiones instaladas y Sales Connect no estará allí para conectarse.

**Contras**: Tendrá que iniciar sesión en Gmail cada vez que inicie su día, y de nuevo si accidentalmente cierra la ventana.
